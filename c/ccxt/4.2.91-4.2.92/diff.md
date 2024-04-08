# Comparing `tmp/ccxt-4.2.91.tar.gz` & `tmp/ccxt-4.2.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ccxt-4.2.91.tar", last modified: Sun Apr  7 17:15:45 2024, max compression
+gzip compressed data, was "dist/ccxt-4.2.92.tar", last modified: Mon Apr  8 17:32:45 2024, max compression
```

## Comparing `ccxt-4.2.91.tar` & `ccxt-4.2.92.tar`

### file list

```diff
@@ -1,572 +1,572 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.595788 ccxt-4.2.91/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2024-04-07 17:14:30.000000 ccxt-4.2.91/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      101 2024-04-07 16:43:56.000000 ccxt-4.2.91/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)   114404 2024-04-07 17:15:45.599789 ccxt-4.2.91/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)   102253 2024-04-07 16:43:56.000000 ccxt-4.2.91/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.387772 ccxt-4.2.91/ccxt/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15656 2024-04-07 17:14:28.000000 ccxt-4.2.91/ccxt/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.451777 ccxt-4.2.91/ccxt/abstract/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/abstract/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1448 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10382 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11394 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/ascendex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4895 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    91751 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    91751 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    98471 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    91751 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15876 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/bingx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2830 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2735 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5820 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4082 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7605 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19194 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    89841 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3443 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14031 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10774 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3295 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9379 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4025 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27231 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3478 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/bitteam.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2024 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2638 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3978 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/blofin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1380 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      849 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3690 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1777 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48391 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3311 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14395 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4770 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/coinbaseinternational.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7162 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3417 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34678 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6538 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/coinlist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6842 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3864 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/coinmetro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8291 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8007 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2707 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18475 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7563 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5107 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15499 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11452 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6177 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41994 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41994 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6915 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2906 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    99311 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/htx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    99311 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14331 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      240 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/hyperliquid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4165 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2488 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5877 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3537 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25491 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27937 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24579 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7168 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8675 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3373 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2960 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25902 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11878 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3093 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1721 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9414 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45891 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/onetrading.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2054 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/p2b.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2843 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15203 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8073 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5219 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/poloniexfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1969 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5875 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4094 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1372 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/tradeogre.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19631 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2782 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8029 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10216 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1339 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3935 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5820 2024-04-07 16:45:53.000000 ccxt-4.2.91/ccxt/abstract/zonda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41420 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46908 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   151300 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/ascendex.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.539784 ccxt-4.2.91/ccxt/async_support/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15409 2024-04-07 17:14:28.000000 ccxt-4.2.91/ccxt/async_support/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41644 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47120 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   152088 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/ascendex.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.539784 ccxt-4.2.91/ccxt/async_support/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    91193 2024-04-07 17:14:28.000000 ccxt-4.2.91/ccxt/async_support/base/exchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1847 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/base/throttler.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.543784 ccxt-4.2.91/ccxt/async_support/base/ws/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1791 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/base/ws/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5751 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/base/ws/aiohttp_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8100 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/base/ws/cache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7289 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/base/ws/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3864 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/base/ws/fast_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1499 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/base/ws/functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2067 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/base/ws/future.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2894 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/base/ws/order_book.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6478 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/base/ws/order_book_side.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1188 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92639 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   597430 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1683 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9177 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2518 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   182980 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/bingx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37113 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41949 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      492 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48385 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      516 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71968 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   158863 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41694 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   409327 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45564 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   200023 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   125968 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68685 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      485 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   136831 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71115 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92342 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   102163 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/bitteam.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    91855 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20460 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    49180 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    99698 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/blofin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36828 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23535 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51678 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36724 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   403300 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    70003 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   179388 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87677 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/coinbaseinternational.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    78883 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35719 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   248969 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   103489 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/coinlist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46056 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80729 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/coinmetro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46987 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    90866 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23615 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   128712 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87181 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   151045 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   159951 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   170709 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   114835 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/flowbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1250 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   316838 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      459 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80359 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   153853 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      469 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76327 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   420760 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/htx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      452 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88457 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92896 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/hyperliquid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    73285 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32284 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    52087 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   122568 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   116143 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   215759 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   119121 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    96396 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    79256 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   115876 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45981 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51143 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35425 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   237552 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   108892 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    64473 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38180 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   151629 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   350154 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88409 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/onetrading.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    54316 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/p2b.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24391 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   219437 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   102496 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    77756 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/poloniexfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76610 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71498 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   123364 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23955 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/tradeogre.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    82082 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   113950 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51493 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   101482 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   127108 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    53350 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28134 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80866 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/async_support/zonda.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.543784 ccxt-4.2.91/ccxt/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1320 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6634 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/base/decimal_to_precision.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4099 2024-04-07 16:58:52.000000 ccxt-4.2.91/ccxt/base/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   253647 2024-04-07 17:14:28.000000 ccxt-4.2.91/ccxt/base/exchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8565 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/base/precise.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7690 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/base/types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1174 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92185 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   594870 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1645 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9163 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2480 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   181968 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/bingx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36901 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41689 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      478 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48131 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      502 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71528 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   158129 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41386 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   407793 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45334 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   199103 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   125408 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68281 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      471 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   136173 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    70729 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    91842 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   101831 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/bitteam.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    91421 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20332 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48788 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    99114 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/blofin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36550 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23341 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51328 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36506 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   401556 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69653 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   178431 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87123 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/coinbaseinternational.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    78377 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35513 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   247699 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   103001 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/coinlist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45790 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80409 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/coinmetro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46745 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    90432 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23463 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   128158 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    86759 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   150437 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   159181 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   169739 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   114203 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1169 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/flowbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1236 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   315184 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      445 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    79846 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   152807 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      455 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75893 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   418422 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/htx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      438 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87957 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92412 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/hyperliquid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    72809 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32024 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51779 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   121984 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   115673 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   214705 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   118519 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    95980 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    78780 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   115164 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45643 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    50829 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35183 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   236392 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   108368 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    64105 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37860 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   151105 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   348729 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87957 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/onetrading.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    54074 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/p2b.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24203 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   218625 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   101948 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    77370 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/poloniexfutures.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.563786 ccxt-4.2.91/ccxt/pro/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6999 2024-04-07 17:14:28.000000 ccxt-4.2.91/ccxt/pro/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27167 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35432 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/ascendex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   136416 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      976 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2321 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1357 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42110 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/bingx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1181 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24826 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42744 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71862 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16799 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62382 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68956 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18724 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      415 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16448 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20886 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    56143 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29560 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75022 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    58370 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22578 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25428 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/coinbaseinternational.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38945 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7789 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45042 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15652 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42643 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22355 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41035 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24527 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    52489 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      391 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36641 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    56285 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21957 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    95779 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/htx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      385 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23174 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20613 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/hyperliquid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28282 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11063 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    56274 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    60165 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    50271 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46006 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35100 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12348 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42551 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22643 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30385 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68821 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    54634 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/onetrading.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17877 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/p2b.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    61032 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51236 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41480 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/poloniexfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22822 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9654 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30004 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35021 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37022 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/pro/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76218 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/probit.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.567786 ccxt-4.2.91/ccxt/static_dependencies/
--rw-rw-r--   0 travis    (2000) travis    (2000)       84 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.567786 ccxt-4.2.91/ccxt/static_dependencies/ecdsa/
--rw-rw-r--   0 travis    (2000) travis    (2000)      594 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ecdsa/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18461 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ecdsa/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ecdsa/curves.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6942 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ecdsa/der.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11336 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ecdsa/ecdsa.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5517 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ecdsa/ellipticcurve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14201 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ecdsa/keys.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13468 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ecdsa/numbertheory.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2572 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ecdsa/rfc6979.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10037 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ecdsa/util.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.567786 ccxt-4.2.91/ccxt/static_dependencies/ethereum/
--rw-rw-r--   0 travis    (2000) travis    (2000)      171 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.571786 ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/
--rw-rw-r--   0 travis    (2000) travis    (2000)      276 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      490 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/abi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4861 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6871 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/codec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       51 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16828 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/decoding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20162 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/encoding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12358 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/grammar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      387 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/packed.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/py.typed
--rw-rw-r--   0 travis    (2000) travis    (2000)    19329 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/registry.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.571786 ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/tools/
--rw-rw-r--   0 travis    (2000) travis    (2000)       65 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/tools/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5742 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.571786 ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2097 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/utils/numeric.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      426 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/utils/padding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      436 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/utils/string.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.571786 ccxt-4.2.91/ccxt/static_dependencies/ethereum/account/
--rw-rw-r--   0 travis    (2000) travis    (2000)       48 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/account/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.571786 ccxt-4.2.91/ccxt/static_dependencies/ethereum/account/encode_typed_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)       80 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/account/encode_typed_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7126 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      982 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10588 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/account/messages.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/account/py.typed
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.575787 ccxt-4.2.91/ccxt/static_dependencies/ethereum/hexbytes/
--rw-rw-r--   0 travis    (2000) travis    (2000)       60 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/hexbytes/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1687 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/hexbytes/_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1768 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/hexbytes/main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/hexbytes/py.typed
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.575787 ccxt-4.2.91/ccxt/static_dependencies/ethereum/typing/
--rw-rw-r--   0 travis    (2000) travis    (2000)      913 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/typing/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       85 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/typing/abi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      191 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/typing/bls.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       71 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/typing/discovery.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      117 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/typing/encoding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      458 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/typing/enums.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      173 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/typing/ethpm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      546 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/typing/evm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20845 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/typing/networks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/typing/py.typed
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.583787 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2162 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2123 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/abi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4364 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/address.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4342 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/applicators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5498 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/conversions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3021 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/currency.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.583787 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/curried/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6398 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/curried/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      499 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/debug.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3997 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/decorators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      199 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/encoding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      110 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/functional.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1826 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/hexadecimal.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4137 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/humanize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5155 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/logging.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      842 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/module_loading.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1190 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/numeric.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/py.typed
--rw-rw-r--   0 travis    (2000) travis    (2000)     1001 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/toolz.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1074 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/types.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.583787 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/typing/
--rw-rw-r--   0 travis    (2000) travis    (2000)      325 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/typing/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      189 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/typing/misc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1757 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/units.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.583787 ccxt-4.2.91/ccxt/static_dependencies/keccak/
--rw-rw-r--   0 travis    (2000) travis    (2000)       45 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/keccak/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6934 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/keccak/keccak.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.583787 ccxt-4.2.91/ccxt/static_dependencies/msgpack/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1077 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/msgpack/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/msgpack/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5629 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/msgpack/ext.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33175 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/msgpack/fallback.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.583787 ccxt-4.2.91/ccxt/static_dependencies/parsimonious/
--rw-rw-r--   0 travis    (2000) travis    (2000)      385 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/parsimonious/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3603 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/parsimonious/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16864 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/parsimonious/expressions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19190 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/parsimonious/grammar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13084 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/parsimonious/nodes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1087 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/parsimonious/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.587788 ccxt-4.2.91/ccxt/static_dependencies/toolz/
--rw-rw-r--   0 travis    (2000) travis    (2000)      374 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/toolz/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20555 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/toolz/_signatures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18447 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/toolz/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      997 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/toolz/compatibility.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.587788 ccxt-4.2.91/ccxt/static_dependencies/toolz/curried/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2226 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/toolz/curried/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      344 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/toolz/curried/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      525 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/toolz/curried/operator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8955 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/toolz/dicttoolz.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29821 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/toolz/functoolz.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27612 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/toolz/itertoolz.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1256 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/toolz/recipes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/static_dependencies/toolz/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.587788 ccxt-4.2.91/ccxt/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)      141 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/test/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.595788 ccxt-4.2.91/ccxt/test/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1889 2024-04-07 16:58:57.000000 ccxt-4.2.91/ccxt/test/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      978 2024-04-07 17:00:20.000000 ccxt-4.2.91/ccxt/test/base/test_account.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2931 2024-04-07 17:00:20.000000 ccxt-4.2.91/ccxt/test/base/test_balance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1808 2024-04-07 17:00:20.000000 ccxt-4.2.91/ccxt/test/base/test_borrow_interest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1500 2024-04-07 17:00:20.000000 ccxt-4.2.91/ccxt/test/base/test_borrow_rate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1177 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/test/base/test_calculate_fee.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7702 2024-04-07 16:58:54.000000 ccxt-4.2.91/ccxt/test/base/test_crypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4472 2024-04-07 17:00:20.000000 ccxt-4.2.91/ccxt/test/base/test_currency.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5235 2024-04-07 16:58:53.000000 ccxt-4.2.91/ccxt/test/base/test_datetime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20934 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/test/base/test_decimal_to_precision.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1402 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/test/base/test_deep_extend.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2452 2024-04-07 17:00:20.000000 ccxt-4.2.91/ccxt/test/base/test_deposit_withdrawal.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3592 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/test/base/test_exchange_datetime_functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2024-04-07 17:00:20.000000 ccxt-4.2.91/ccxt/test/base/test_funding_rate_history.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1332 2024-04-07 17:00:20.000000 ccxt-4.2.91/ccxt/test/base/test_last_price.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2283 2024-04-07 17:00:20.000000 ccxt-4.2.91/ccxt/test/base/test_ledger_entry.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2154 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/test/base/test_ledger_item.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1656 2024-04-07 17:00:20.000000 ccxt-4.2.91/ccxt/test/base/test_leverage_tier.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      869 2024-04-07 17:00:20.000000 ccxt-4.2.91/ccxt/test/base/test_margin_mode.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1730 2024-04-07 17:00:20.000000 ccxt-4.2.91/ccxt/test/base/test_margin_modification.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11632 2024-04-07 17:00:20.000000 ccxt-4.2.91/ccxt/test/base/test_market.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22083 2024-04-07 16:58:53.000000 ccxt-4.2.91/ccxt/test/base/test_number.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2036 2024-04-07 17:00:20.000000 ccxt-4.2.91/ccxt/test/base/test_ohlcv.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1547 2024-04-07 17:00:20.000000 ccxt-4.2.91/ccxt/test/base/test_open_interest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3964 2024-04-07 17:00:21.000000 ccxt-4.2.91/ccxt/test/base/test_order.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3586 2024-04-07 17:00:21.000000 ccxt-4.2.91/ccxt/test/base/test_order_book.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3884 2024-04-07 17:00:21.000000 ccxt-4.2.91/ccxt/test/base/test_position.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19998 2024-04-07 17:00:21.000000 ccxt-4.2.91/ccxt/test/base/test_shared_methods.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      722 2024-04-07 17:00:21.000000 ccxt-4.2.91/ccxt/test/base/test_status.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3123 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/test/base/test_throttle.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5810 2024-04-07 17:00:21.000000 ccxt-4.2.91/ccxt/test/base/test_ticker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2336 2024-04-07 17:00:21.000000 ccxt-4.2.91/ccxt/test/base/test_trade.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1066 2024-04-07 17:00:21.000000 ccxt-4.2.91/ccxt/test/base/test_trading_fee.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1434 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/test/base/test_transaction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    77013 2024-04-07 16:58:57.000000 ccxt-4.2.91/ccxt/test/test_async.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75994 2024-04-07 16:58:57.000000 ccxt-4.2.91/ccxt/test/test_sync.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71136 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   123002 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23761 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/tradeogre.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    81600 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   113400 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51191 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   100934 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   126326 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    53066 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27952 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80552 2024-04-07 16:43:56.000000 ccxt-4.2.91/ccxt/zonda.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-07 17:15:45.391772 ccxt-4.2.91/ccxt.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)   114404 2024-04-07 17:15:45.000000 ccxt-4.2.91/ccxt.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    15741 2024-04-07 17:15:45.000000 ccxt-4.2.91/ccxt.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-07 17:15:45.000000 ccxt-4.2.91/ccxt.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      218 2024-04-07 17:15:45.000000 ccxt-4.2.91/ccxt.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2024-04-07 17:15:45.000000 ccxt-4.2.91/ccxt.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    12515 2024-04-07 17:14:29.000000 ccxt-4.2.91/package.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      205 2024-04-07 17:15:45.599789 ccxt-4.2.91/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3071 2024-04-07 16:43:56.000000 ccxt-4.2.91/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.175138 ccxt-4.2.92/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2024-04-08 17:31:28.000000 ccxt-4.2.92/LICENSE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      101 2024-04-08 16:59:48.000000 ccxt-4.2.92/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)   114404 2024-04-08 17:32:45.179138 ccxt-4.2.92/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)   102253 2024-04-08 16:59:48.000000 ccxt-4.2.92/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:44.987124 ccxt-4.2.92/ccxt/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15656 2024-04-08 17:31:27.000000 ccxt-4.2.92/ccxt/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.019126 ccxt-4.2.92/ccxt/abstract/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/abstract/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1448 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10382 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11394 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/ascendex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4895 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91751 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91751 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    98471 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91751 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15876 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/bingx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2830 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2735 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5820 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4082 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7605 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19194 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    89841 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3443 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14031 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10774 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3295 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9379 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4025 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27231 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3478 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/bitteam.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2024 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2638 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3978 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/blofin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1380 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      849 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3690 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1777 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48599 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3311 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14395 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4770 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/coinbaseinternational.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7162 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3417 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34678 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6538 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/coinlist.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6842 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3864 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/coinmetro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8291 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8007 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2707 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18475 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7563 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5107 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15499 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11452 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6177 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41994 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41994 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6915 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2906 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    99311 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/htx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    99311 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14331 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      240 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/hyperliquid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4165 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2488 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5877 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3537 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25491 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27937 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24579 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7168 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8675 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3373 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2960 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25902 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11878 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3093 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1721 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9414 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45891 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/onetrading.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2054 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/p2b.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2843 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15203 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8073 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5219 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/poloniexfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1969 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5875 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4094 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1372 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/tradeogre.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19631 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2782 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8029 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10216 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1339 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3935 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5820 2024-04-08 17:01:45.000000 ccxt-4.2.92/ccxt/abstract/zonda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41420 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46908 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   151300 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/ascendex.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.087131 ccxt-4.2.92/ccxt/async_support/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15409 2024-04-08 17:31:27.000000 ccxt-4.2.92/ccxt/async_support/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41644 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47120 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   152088 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/ascendex.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.095132 ccxt-4.2.92/ccxt/async_support/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91193 2024-04-08 17:31:27.000000 ccxt-4.2.92/ccxt/async_support/base/exchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1847 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/base/throttler.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.095132 ccxt-4.2.92/ccxt/async_support/base/ws/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1791 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/base/ws/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5751 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/base/ws/aiohttp_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8100 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/base/ws/cache.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7289 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/base/ws/client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3864 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/base/ws/fast_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1499 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/base/ws/functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2067 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/base/ws/future.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2894 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/base/ws/order_book.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6478 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/base/ws/order_book_side.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1188 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92639 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   597430 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1683 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9177 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2518 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   182980 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/bingx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37113 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41949 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      492 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48385 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      516 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71968 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   158863 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41694 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   409327 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45564 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   200023 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   125968 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68685 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      485 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   136831 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71115 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92342 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   102163 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/bitteam.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91855 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20460 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    49180 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    99698 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/blofin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36828 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23535 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51678 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36724 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   403379 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    70003 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   179388 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87677 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/coinbaseinternational.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    78883 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35719 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   248969 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   103489 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/coinlist.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46056 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80729 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/coinmetro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46987 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    90866 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23615 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   128712 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87181 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   151045 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   160915 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   170709 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   114835 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/flowbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1250 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   316838 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      459 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80359 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   153853 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      469 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76327 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   420760 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/htx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      452 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88457 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92896 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/hyperliquid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    73285 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32284 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    52087 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   124519 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   116143 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   215759 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119121 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    96396 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    79256 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   115876 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45981 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51143 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35425 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   237552 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   108892 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    64473 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38180 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   151629 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   350154 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88409 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/onetrading.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    54316 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/p2b.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24391 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   219437 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   102496 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    77756 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/poloniexfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76610 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/async_support/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71498 2024-04-08 16:59:49.000000 ccxt-4.2.92/ccxt/async_support/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   123364 2024-04-08 16:59:49.000000 ccxt-4.2.92/ccxt/async_support/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23955 2024-04-08 16:59:49.000000 ccxt-4.2.92/ccxt/async_support/tradeogre.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    82082 2024-04-08 16:59:49.000000 ccxt-4.2.92/ccxt/async_support/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   113950 2024-04-08 16:59:49.000000 ccxt-4.2.92/ccxt/async_support/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51493 2024-04-08 16:59:49.000000 ccxt-4.2.92/ccxt/async_support/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   101482 2024-04-08 16:59:49.000000 ccxt-4.2.92/ccxt/async_support/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   127108 2024-04-08 16:59:49.000000 ccxt-4.2.92/ccxt/async_support/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53350 2024-04-08 16:59:49.000000 ccxt-4.2.92/ccxt/async_support/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28134 2024-04-08 16:59:49.000000 ccxt-4.2.92/ccxt/async_support/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80866 2024-04-08 16:59:49.000000 ccxt-4.2.92/ccxt/async_support/zonda.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.111133 ccxt-4.2.92/ccxt/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1320 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6634 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/base/decimal_to_precision.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4099 2024-04-08 17:15:13.000000 ccxt-4.2.92/ccxt/base/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   253791 2024-04-08 17:31:27.000000 ccxt-4.2.92/ccxt/base/exchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8565 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/base/precise.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7690 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/base/types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1174 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92185 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   594870 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1645 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9163 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2480 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   181968 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/bingx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36901 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41689 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      478 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48131 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      502 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71528 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   158129 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41386 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   407793 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45334 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   199103 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   125408 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68281 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      471 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   136173 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    70729 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91842 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   101831 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/bitteam.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91421 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20332 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48788 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    99114 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/blofin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36550 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23341 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51328 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36506 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   401635 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69653 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   178431 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87123 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/coinbaseinternational.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    78377 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35513 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   247699 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   103001 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/coinlist.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45790 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80409 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/coinmetro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46745 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    90432 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23463 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   128158 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    86759 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   150437 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   160139 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   169739 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   114203 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1169 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/flowbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1236 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   315184 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      445 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    79846 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   152807 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      455 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75893 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   418422 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/htx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      438 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87957 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92412 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/hyperliquid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    72809 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32024 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51779 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   123935 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   115673 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   214705 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   118519 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95980 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    78780 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   115164 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45643 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50829 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35183 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   236392 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   108368 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    64105 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37860 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   151105 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   348729 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87957 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/onetrading.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    54074 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/p2b.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24203 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   218625 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   101948 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    77370 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/poloniexfutures.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.139135 ccxt-4.2.92/ccxt/pro/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6999 2024-04-08 17:31:27.000000 ccxt-4.2.92/ccxt/pro/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27167 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35432 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/ascendex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   136416 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      976 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2321 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1357 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42110 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/bingx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1181 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24826 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42744 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71862 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16799 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62382 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68956 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18724 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      415 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16448 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20886 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    56143 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29560 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75022 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    58370 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22578 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25428 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/coinbaseinternational.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38945 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7789 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45042 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15652 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42643 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22355 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41035 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24527 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    52489 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      391 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36641 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    56285 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21957 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95779 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/htx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      385 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23174 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20613 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/hyperliquid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28282 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11063 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    56274 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    60165 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50271 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46006 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35100 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12348 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42551 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22643 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30385 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68821 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    54634 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/onetrading.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17877 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/p2b.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    61032 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51236 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41480 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/poloniexfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22822 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9654 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30004 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35021 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37022 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/pro/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76218 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/probit.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.139135 ccxt-4.2.92/ccxt/static_dependencies/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       84 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.143135 ccxt-4.2.92/ccxt/static_dependencies/ecdsa/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      594 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ecdsa/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18461 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ecdsa/_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ecdsa/curves.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6942 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ecdsa/der.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11336 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ecdsa/ecdsa.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5517 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ecdsa/ellipticcurve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14201 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ecdsa/keys.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13468 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ecdsa/numbertheory.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2572 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ecdsa/rfc6979.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10037 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ecdsa/util.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.143135 ccxt-4.2.92/ccxt/static_dependencies/ethereum/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      171 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.147136 ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      276 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      490 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/abi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4861 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6871 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/codec.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       51 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16828 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/decoding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20162 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/encoding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12358 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/grammar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      387 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/packed.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/py.typed
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19329 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/registry.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.147136 ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/tools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       65 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/tools/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5742 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.147136 ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2097 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/utils/numeric.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      426 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/utils/padding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      436 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/utils/string.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.147136 ccxt-4.2.92/ccxt/static_dependencies/ethereum/account/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       48 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/account/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.151136 ccxt-4.2.92/ccxt/static_dependencies/ethereum/account/encode_typed_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       80 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/account/encode_typed_data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7126 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      982 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10588 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/account/messages.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/account/py.typed
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.151136 ccxt-4.2.92/ccxt/static_dependencies/ethereum/hexbytes/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       60 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/hexbytes/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1687 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/hexbytes/_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1768 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/hexbytes/main.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/hexbytes/py.typed
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.155136 ccxt-4.2.92/ccxt/static_dependencies/ethereum/typing/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      913 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/typing/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       85 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/typing/abi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      191 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/typing/bls.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       71 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/typing/discovery.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      117 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/typing/encoding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      458 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/typing/enums.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      173 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/typing/ethpm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      546 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/typing/evm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20845 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/typing/networks.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/typing/py.typed
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.159136 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2162 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2123 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/abi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4364 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/address.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4342 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/applicators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5498 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/conversions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3021 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/currency.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.159136 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/curried/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6398 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/curried/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      499 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/debug.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3997 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/decorators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      199 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/encoding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      110 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/functional.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1826 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/hexadecimal.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4137 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/humanize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5155 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/logging.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      842 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/module_loading.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1190 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/numeric.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/py.typed
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1001 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/toolz.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1074 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/types.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.159136 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/typing/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      325 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/typing/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      189 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/typing/misc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1757 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/units.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.159136 ccxt-4.2.92/ccxt/static_dependencies/keccak/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       45 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/keccak/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6934 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/keccak/keccak.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.159136 ccxt-4.2.92/ccxt/static_dependencies/msgpack/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1077 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/msgpack/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/msgpack/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5629 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/msgpack/ext.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33175 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/msgpack/fallback.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.163137 ccxt-4.2.92/ccxt/static_dependencies/parsimonious/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      385 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/parsimonious/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3603 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/parsimonious/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16864 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/parsimonious/expressions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19190 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/parsimonious/grammar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13084 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/parsimonious/nodes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1087 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/parsimonious/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.163137 ccxt-4.2.92/ccxt/static_dependencies/toolz/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      374 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/toolz/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20555 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/toolz/_signatures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18447 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/toolz/_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      997 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/toolz/compatibility.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.167137 ccxt-4.2.92/ccxt/static_dependencies/toolz/curried/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2226 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/toolz/curried/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      344 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/toolz/curried/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      525 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/toolz/curried/operator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8955 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/toolz/dicttoolz.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29821 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/toolz/functoolz.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27612 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/toolz/itertoolz.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1256 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/toolz/recipes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      139 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/static_dependencies/toolz/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.167137 ccxt-4.2.92/ccxt/test/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      141 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/test/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:45.175138 ccxt-4.2.92/ccxt/test/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1889 2024-04-08 17:15:17.000000 ccxt-4.2.92/ccxt/test/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      978 2024-04-08 17:16:43.000000 ccxt-4.2.92/ccxt/test/base/test_account.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2931 2024-04-08 17:16:43.000000 ccxt-4.2.92/ccxt/test/base/test_balance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1808 2024-04-08 17:16:43.000000 ccxt-4.2.92/ccxt/test/base/test_borrow_interest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1500 2024-04-08 17:16:43.000000 ccxt-4.2.92/ccxt/test/base/test_borrow_rate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1177 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/test/base/test_calculate_fee.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7702 2024-04-08 17:15:15.000000 ccxt-4.2.92/ccxt/test/base/test_crypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4472 2024-04-08 17:16:43.000000 ccxt-4.2.92/ccxt/test/base/test_currency.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5235 2024-04-08 17:15:14.000000 ccxt-4.2.92/ccxt/test/base/test_datetime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20934 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/test/base/test_decimal_to_precision.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1402 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/test/base/test_deep_extend.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2452 2024-04-08 17:16:43.000000 ccxt-4.2.92/ccxt/test/base/test_deposit_withdrawal.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3592 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/test/base/test_exchange_datetime_functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2024-04-08 17:16:43.000000 ccxt-4.2.92/ccxt/test/base/test_funding_rate_history.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1332 2024-04-08 17:16:43.000000 ccxt-4.2.92/ccxt/test/base/test_last_price.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2283 2024-04-08 17:16:43.000000 ccxt-4.2.92/ccxt/test/base/test_ledger_entry.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2154 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/test/base/test_ledger_item.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1656 2024-04-08 17:16:43.000000 ccxt-4.2.92/ccxt/test/base/test_leverage_tier.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      869 2024-04-08 17:16:43.000000 ccxt-4.2.92/ccxt/test/base/test_margin_mode.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1730 2024-04-08 17:16:43.000000 ccxt-4.2.92/ccxt/test/base/test_margin_modification.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11632 2024-04-08 17:16:43.000000 ccxt-4.2.92/ccxt/test/base/test_market.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22083 2024-04-08 17:15:14.000000 ccxt-4.2.92/ccxt/test/base/test_number.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2036 2024-04-08 17:16:43.000000 ccxt-4.2.92/ccxt/test/base/test_ohlcv.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1547 2024-04-08 17:16:43.000000 ccxt-4.2.92/ccxt/test/base/test_open_interest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3964 2024-04-08 17:16:43.000000 ccxt-4.2.92/ccxt/test/base/test_order.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3586 2024-04-08 17:16:43.000000 ccxt-4.2.92/ccxt/test/base/test_order_book.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3884 2024-04-08 17:16:43.000000 ccxt-4.2.92/ccxt/test/base/test_position.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19998 2024-04-08 17:16:43.000000 ccxt-4.2.92/ccxt/test/base/test_shared_methods.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      722 2024-04-08 17:16:43.000000 ccxt-4.2.92/ccxt/test/base/test_status.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3123 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/test/base/test_throttle.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5810 2024-04-08 17:16:43.000000 ccxt-4.2.92/ccxt/test/base/test_ticker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2336 2024-04-08 17:16:43.000000 ccxt-4.2.92/ccxt/test/base/test_trade.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1066 2024-04-08 17:16:43.000000 ccxt-4.2.92/ccxt/test/base/test_trading_fee.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1434 2024-04-08 16:59:48.000000 ccxt-4.2.92/ccxt/test/base/test_transaction.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    77013 2024-04-08 17:15:17.000000 ccxt-4.2.92/ccxt/test/test_async.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75994 2024-04-08 17:15:17.000000 ccxt-4.2.92/ccxt/test/test_sync.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71136 2024-04-08 16:59:49.000000 ccxt-4.2.92/ccxt/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   123002 2024-04-08 16:59:49.000000 ccxt-4.2.92/ccxt/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23761 2024-04-08 16:59:49.000000 ccxt-4.2.92/ccxt/tradeogre.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    81600 2024-04-08 16:59:49.000000 ccxt-4.2.92/ccxt/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   113400 2024-04-08 16:59:49.000000 ccxt-4.2.92/ccxt/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51191 2024-04-08 16:59:49.000000 ccxt-4.2.92/ccxt/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   100934 2024-04-08 16:59:49.000000 ccxt-4.2.92/ccxt/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   126326 2024-04-08 16:59:49.000000 ccxt-4.2.92/ccxt/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53066 2024-04-08 16:59:49.000000 ccxt-4.2.92/ccxt/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27952 2024-04-08 16:59:49.000000 ccxt-4.2.92/ccxt/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80552 2024-04-08 16:59:49.000000 ccxt-4.2.92/ccxt/zonda.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-08 17:32:44.991124 ccxt-4.2.92/ccxt.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)   114404 2024-04-08 17:32:44.000000 ccxt-4.2.92/ccxt.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15741 2024-04-08 17:32:44.000000 ccxt-4.2.92/ccxt.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-08 17:32:44.000000 ccxt-4.2.92/ccxt.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      218 2024-04-08 17:32:44.000000 ccxt-4.2.92/ccxt.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        5 2024-04-08 17:32:44.000000 ccxt-4.2.92/ccxt.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12515 2024-04-08 17:31:28.000000 ccxt-4.2.92/package.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      205 2024-04-08 17:32:45.179138 ccxt-4.2.92/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3071 2024-04-08 16:59:48.000000 ccxt-4.2.92/setup.py
```

### Comparing `ccxt-4.2.91/LICENSE.txt` & `ccxt-4.2.92/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/PKG-INFO` & `ccxt-4.2.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccxt
-Version: 4.2.91
+Version: 4.2.92
 Summary: A JavaScript / TypeScript / Python / C# / PHP cryptocurrency trading library with support for 100+ exchanges
 Home-page: https://ccxt.com
 Author: Igor Kroitor
 Author-email: igor.kroitor@gmail.com
 License: MIT
 Project-URL: Homepage, https://ccxt.com
 Project-URL: Documentation, https://github.com/ccxt/ccxt/wiki
@@ -221,21 +221,21 @@
         console.log(version, Object.keys(exchanges));
         ```
         
         ### JavaScript (for use with the `<script>` tag):
         
         All-in-one browser bundle (dependencies included), served from a CDN of your choice:
         
-        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@4.2.91/dist/ccxt.browser.js
-        * unpkg: https://unpkg.com/ccxt@4.2.91/dist/ccxt.browser.js
+        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@4.2.92/dist/ccxt.browser.js
+        * unpkg: https://unpkg.com/ccxt@4.2.92/dist/ccxt.browser.js
         
         CDNs are not updated in real-time and may have delays. Defaulting to the most recent version without specifying the version number is not recommended. Please, keep in mind that we are not responsible for the correct operation of those CDN servers.
         
         ```HTML
-        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@4.2.91/dist/ccxt.browser.js"></script>
+        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@4.2.92/dist/ccxt.browser.js"></script>
         ```
         
         Creates a global `ccxt` object:
         
         ```JavaScript
         console.log (ccxt.exchanges) // print all available exchanges
         ```
```

### Comparing `ccxt-4.2.91/README.rst` & `ccxt-4.2.92/README.rst`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/__init__.py` & `ccxt-4.2.92/ccxt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 # ----------------------------------------------------------------------------
 
-__version__ = '4.2.91'
+__version__ = '4.2.92'
 
 # ----------------------------------------------------------------------------
 
 from ccxt.base.exchange import Exchange                     # noqa: F401
 from ccxt.base.precise import Precise                       # noqa: F401
 
 from ccxt.base.decimal_to_precision import decimal_to_precision  # noqa: F401
```

### Comparing `ccxt-4.2.91/ccxt/abstract/ace.py` & `ccxt-4.2.92/ccxt/abstract/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/alpaca.py` & `ccxt-4.2.92/ccxt/abstract/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/ascendex.py` & `ccxt-4.2.92/ccxt/abstract/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/bequant.py` & `ccxt-4.2.92/ccxt/abstract/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/bigone.py` & `ccxt-4.2.92/ccxt/abstract/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/binance.py` & `ccxt-4.2.92/ccxt/abstract/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/binancecoinm.py` & `ccxt-4.2.92/ccxt/abstract/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/binanceus.py` & `ccxt-4.2.92/ccxt/abstract/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/binanceusdm.py` & `ccxt-4.2.92/ccxt/abstract/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/bingx.py` & `ccxt-4.2.92/ccxt/abstract/bingx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/bit2c.py` & `ccxt-4.2.92/ccxt/abstract/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/bitbank.py` & `ccxt-4.2.92/ccxt/abstract/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/bitbay.py` & `ccxt-4.2.92/ccxt/abstract/bitbay.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/bitbns.py` & `ccxt-4.2.92/ccxt/abstract/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/bitcoincom.py` & `ccxt-4.2.92/ccxt/abstract/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/bitfinex.py` & `ccxt-4.2.92/ccxt/abstract/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/bitfinex2.py` & `ccxt-4.2.92/ccxt/abstract/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/bitflyer.py` & `ccxt-4.2.92/ccxt/abstract/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/bitget.py` & `ccxt-4.2.92/ccxt/abstract/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/bithumb.py` & `ccxt-4.2.92/ccxt/abstract/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/bitmart.py` & `ccxt-4.2.92/ccxt/abstract/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/bitmex.py` & `ccxt-4.2.92/ccxt/abstract/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/bitopro.py` & `ccxt-4.2.92/ccxt/abstract/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/bitpanda.py` & `ccxt-4.2.92/ccxt/abstract/bitpanda.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/bitrue.py` & `ccxt-4.2.92/ccxt/abstract/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/bitso.py` & `ccxt-4.2.92/ccxt/abstract/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/bitstamp.py` & `ccxt-4.2.92/ccxt/abstract/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/bitteam.py` & `ccxt-4.2.92/ccxt/abstract/bitteam.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/bitvavo.py` & `ccxt-4.2.92/ccxt/abstract/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/bl3p.py` & `ccxt-4.2.92/ccxt/abstract/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/blockchaincom.py` & `ccxt-4.2.92/ccxt/abstract/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/blofin.py` & `ccxt-4.2.92/ccxt/abstract/blofin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/btcalpha.py` & `ccxt-4.2.92/ccxt/abstract/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/btcbox.py` & `ccxt-4.2.92/ccxt/abstract/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/btcmarkets.py` & `ccxt-4.2.92/ccxt/abstract/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/btcturk.py` & `ccxt-4.2.92/ccxt/abstract/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/bybit.py` & `ccxt-4.2.92/ccxt/abstract/bybit.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,15 @@
     private_get_v5_ins_loan_ltv_convert = privateGetV5InsLoanLtvConvert = Entry('v5/ins-loan/ltv-convert', 'private', 'GET', {'cost': 5})
     private_get_v5_lending_info = privateGetV5LendingInfo = Entry('v5/lending/info', 'private', 'GET', {'cost': 5})
     private_get_v5_lending_history_order = privateGetV5LendingHistoryOrder = Entry('v5/lending/history-order', 'private', 'GET', {'cost': 5})
     private_get_v5_lending_account = privateGetV5LendingAccount = Entry('v5/lending/account', 'private', 'GET', {'cost': 5})
     private_get_v5_broker_earning_record = privateGetV5BrokerEarningRecord = Entry('v5/broker/earning-record', 'private', 'GET', {'cost': 5})
     private_get_v5_broker_earnings_info = privateGetV5BrokerEarningsInfo = Entry('v5/broker/earnings-info', 'private', 'GET', {'cost': 5})
     private_get_v5_broker_account_info = privateGetV5BrokerAccountInfo = Entry('v5/broker/account-info', 'private', 'GET', {'cost': 5})
+    private_get_v5_broker_asset_query_sub_member_deposit_record = privateGetV5BrokerAssetQuerySubMemberDepositRecord = Entry('v5/broker/asset/query-sub-member-deposit-record', 'private', 'GET', {'cost': 10})
     private_post_option_usdc_openapi_private_v1_place_order = privatePostOptionUsdcOpenapiPrivateV1PlaceOrder = Entry('option/usdc/openapi/private/v1/place-order', 'private', 'POST', {'cost': 2.5})
     private_post_option_usdc_openapi_private_v1_replace_order = privatePostOptionUsdcOpenapiPrivateV1ReplaceOrder = Entry('option/usdc/openapi/private/v1/replace-order', 'private', 'POST', {'cost': 2.5})
     private_post_option_usdc_openapi_private_v1_cancel_order = privatePostOptionUsdcOpenapiPrivateV1CancelOrder = Entry('option/usdc/openapi/private/v1/cancel-order', 'private', 'POST', {'cost': 2.5})
     private_post_option_usdc_openapi_private_v1_cancel_all = privatePostOptionUsdcOpenapiPrivateV1CancelAll = Entry('option/usdc/openapi/private/v1/cancel-all', 'private', 'POST', {'cost': 2.5})
     private_post_option_usdc_openapi_private_v1_query_active_orders = privatePostOptionUsdcOpenapiPrivateV1QueryActiveOrders = Entry('option/usdc/openapi/private/v1/query-active-orders', 'private', 'POST', {'cost': 2.5})
     private_post_option_usdc_openapi_private_v1_query_order_history = privatePostOptionUsdcOpenapiPrivateV1QueryOrderHistory = Entry('option/usdc/openapi/private/v1/query-order-history', 'private', 'POST', {'cost': 2.5})
     private_post_option_usdc_openapi_private_v1_execution_list = privatePostOptionUsdcOpenapiPrivateV1ExecutionList = Entry('option/usdc/openapi/private/v1/execution-list', 'private', 'POST', {'cost': 2.5})
```

### Comparing `ccxt-4.2.91/ccxt/abstract/cex.py` & `ccxt-4.2.92/ccxt/abstract/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/coinbase.py` & `ccxt-4.2.92/ccxt/abstract/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/coinbaseinternational.py` & `ccxt-4.2.92/ccxt/abstract/coinbaseinternational.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/coinbasepro.py` & `ccxt-4.2.92/ccxt/abstract/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/coincheck.py` & `ccxt-4.2.92/ccxt/abstract/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/coinex.py` & `ccxt-4.2.92/ccxt/abstract/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/coinlist.py` & `ccxt-4.2.92/ccxt/abstract/coinlist.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/coinmate.py` & `ccxt-4.2.92/ccxt/abstract/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/coinmetro.py` & `ccxt-4.2.92/ccxt/abstract/coinmetro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/coinone.py` & `ccxt-4.2.92/ccxt/abstract/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/coinsph.py` & `ccxt-4.2.92/ccxt/abstract/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/coinspot.py` & `ccxt-4.2.92/ccxt/abstract/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/cryptocom.py` & `ccxt-4.2.92/ccxt/abstract/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/currencycom.py` & `ccxt-4.2.92/ccxt/abstract/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/delta.py` & `ccxt-4.2.92/ccxt/abstract/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/deribit.py` & `ccxt-4.2.92/ccxt/abstract/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/digifinex.py` & `ccxt-4.2.92/ccxt/abstract/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/exmo.py` & `ccxt-4.2.92/ccxt/abstract/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/fmfwio.py` & `ccxt-4.2.92/ccxt/abstract/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/gate.py` & `ccxt-4.2.92/ccxt/abstract/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/gateio.py` & `ccxt-4.2.92/ccxt/abstract/gateio.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/gemini.py` & `ccxt-4.2.92/ccxt/abstract/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/hitbtc.py` & `ccxt-4.2.92/ccxt/abstract/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/hitbtc3.py` & `ccxt-4.2.92/ccxt/abstract/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/hollaex.py` & `ccxt-4.2.92/ccxt/abstract/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/htx.py` & `ccxt-4.2.92/ccxt/abstract/htx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/huobi.py` & `ccxt-4.2.92/ccxt/abstract/huobi.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/huobijp.py` & `ccxt-4.2.92/ccxt/abstract/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/idex.py` & `ccxt-4.2.92/ccxt/abstract/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/independentreserve.py` & `ccxt-4.2.92/ccxt/abstract/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/indodax.py` & `ccxt-4.2.92/ccxt/abstract/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/kraken.py` & `ccxt-4.2.92/ccxt/abstract/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/krakenfutures.py` & `ccxt-4.2.92/ccxt/abstract/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/kucoin.py` & `ccxt-4.2.92/ccxt/abstract/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/kucoinfutures.py` & `ccxt-4.2.92/ccxt/abstract/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/kuna.py` & `ccxt-4.2.92/ccxt/abstract/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/latoken.py` & `ccxt-4.2.92/ccxt/abstract/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/lbank.py` & `ccxt-4.2.92/ccxt/abstract/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/luno.py` & `ccxt-4.2.92/ccxt/abstract/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/lykke.py` & `ccxt-4.2.92/ccxt/abstract/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/mercado.py` & `ccxt-4.2.92/ccxt/abstract/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/mexc.py` & `ccxt-4.2.92/ccxt/abstract/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/ndax.py` & `ccxt-4.2.92/ccxt/abstract/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/novadax.py` & `ccxt-4.2.92/ccxt/abstract/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/oceanex.py` & `ccxt-4.2.92/ccxt/abstract/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/okcoin.py` & `ccxt-4.2.92/ccxt/abstract/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/okx.py` & `ccxt-4.2.92/ccxt/abstract/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/onetrading.py` & `ccxt-4.2.92/ccxt/abstract/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/p2b.py` & `ccxt-4.2.92/ccxt/abstract/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/paymium.py` & `ccxt-4.2.92/ccxt/abstract/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/phemex.py` & `ccxt-4.2.92/ccxt/abstract/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/poloniex.py` & `ccxt-4.2.92/ccxt/abstract/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/poloniexfutures.py` & `ccxt-4.2.92/ccxt/abstract/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/probit.py` & `ccxt-4.2.92/ccxt/abstract/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/timex.py` & `ccxt-4.2.92/ccxt/abstract/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/tokocrypto.py` & `ccxt-4.2.92/ccxt/abstract/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/tradeogre.py` & `ccxt-4.2.92/ccxt/abstract/tradeogre.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/upbit.py` & `ccxt-4.2.92/ccxt/abstract/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/wavesexchange.py` & `ccxt-4.2.92/ccxt/abstract/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/wazirx.py` & `ccxt-4.2.92/ccxt/abstract/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/whitebit.py` & `ccxt-4.2.92/ccxt/abstract/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/woo.py` & `ccxt-4.2.92/ccxt/abstract/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/yobit.py` & `ccxt-4.2.92/ccxt/abstract/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/zaif.py` & `ccxt-4.2.92/ccxt/abstract/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/abstract/zonda.py` & `ccxt-4.2.92/ccxt/abstract/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/ace.py` & `ccxt-4.2.92/ccxt/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/alpaca.py` & `ccxt-4.2.92/ccxt/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/ascendex.py` & `ccxt-4.2.92/ccxt/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/__init__.py` & `ccxt-4.2.92/ccxt/async_support/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """CCXT: CryptoCurrency eXchange Trading Library (Async)"""
 
 # -----------------------------------------------------------------------------
 
-__version__ = '4.2.91'
+__version__ = '4.2.92'
 
 # -----------------------------------------------------------------------------
 
 from ccxt.async_support.base.exchange import Exchange                   # noqa: F401
 
 from ccxt.base.decimal_to_precision import decimal_to_precision  # noqa: F401
 from ccxt.base.decimal_to_precision import TRUNCATE              # noqa: F401
```

### Comparing `ccxt-4.2.91/ccxt/async_support/ace.py` & `ccxt-4.2.92/ccxt/async_support/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/alpaca.py` & `ccxt-4.2.92/ccxt/async_support/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/ascendex.py` & `ccxt-4.2.92/ccxt/async_support/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/base/exchange.py` & `ccxt-4.2.92/ccxt/async_support/base/exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # -----------------------------------------------------------------------------
 
-__version__ = '4.2.91'
+__version__ = '4.2.92'
 
 # -----------------------------------------------------------------------------
 
 import asyncio
 import concurrent.futures
 import socket
 import certifi
```

### Comparing `ccxt-4.2.91/ccxt/async_support/base/throttler.py` & `ccxt-4.2.92/ccxt/async_support/base/throttler.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/base/ws/__init__.py` & `ccxt-4.2.92/ccxt/async_support/base/ws/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/base/ws/aiohttp_client.py` & `ccxt-4.2.92/ccxt/async_support/base/ws/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/base/ws/cache.py` & `ccxt-4.2.92/ccxt/async_support/base/ws/cache.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/base/ws/client.py` & `ccxt-4.2.92/ccxt/async_support/base/ws/client.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/base/ws/fast_client.py` & `ccxt-4.2.92/ccxt/async_support/base/ws/fast_client.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/base/ws/functions.py` & `ccxt-4.2.92/ccxt/async_support/base/ws/functions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/base/ws/future.py` & `ccxt-4.2.92/ccxt/async_support/base/ws/future.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/base/ws/order_book.py` & `ccxt-4.2.92/ccxt/async_support/base/ws/order_book.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/base/ws/order_book_side.py` & `ccxt-4.2.92/ccxt/async_support/base/ws/order_book_side.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/bequant.py` & `ccxt-4.2.92/ccxt/async_support/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/bigone.py` & `ccxt-4.2.92/ccxt/async_support/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/binance.py` & `ccxt-4.2.92/ccxt/async_support/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/binancecoinm.py` & `ccxt-4.2.92/ccxt/async_support/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/binanceus.py` & `ccxt-4.2.92/ccxt/async_support/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/binanceusdm.py` & `ccxt-4.2.92/ccxt/async_support/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/bingx.py` & `ccxt-4.2.92/ccxt/async_support/bingx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/bit2c.py` & `ccxt-4.2.92/ccxt/async_support/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/bitbank.py` & `ccxt-4.2.92/ccxt/async_support/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/bitbns.py` & `ccxt-4.2.92/ccxt/async_support/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/bitcoincom.py` & `ccxt-4.2.92/ccxt/async_support/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/bitfinex.py` & `ccxt-4.2.92/ccxt/async_support/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/bitfinex2.py` & `ccxt-4.2.92/ccxt/async_support/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/bitflyer.py` & `ccxt-4.2.92/ccxt/async_support/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/bitget.py` & `ccxt-4.2.92/ccxt/async_support/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/bithumb.py` & `ccxt-4.2.92/ccxt/async_support/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/bitmart.py` & `ccxt-4.2.92/ccxt/async_support/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/bitmex.py` & `ccxt-4.2.92/ccxt/async_support/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/bitopro.py` & `ccxt-4.2.92/ccxt/async_support/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/bitrue.py` & `ccxt-4.2.92/ccxt/async_support/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/bitso.py` & `ccxt-4.2.92/ccxt/async_support/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/bitstamp.py` & `ccxt-4.2.92/ccxt/async_support/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/bitteam.py` & `ccxt-4.2.92/ccxt/async_support/bitteam.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/bitvavo.py` & `ccxt-4.2.92/ccxt/async_support/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/bl3p.py` & `ccxt-4.2.92/ccxt/async_support/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/blockchaincom.py` & `ccxt-4.2.92/ccxt/async_support/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/blofin.py` & `ccxt-4.2.92/ccxt/async_support/blofin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/btcalpha.py` & `ccxt-4.2.92/ccxt/async_support/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/btcbox.py` & `ccxt-4.2.92/ccxt/async_support/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/btcmarkets.py` & `ccxt-4.2.92/ccxt/async_support/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/btcturk.py` & `ccxt-4.2.92/ccxt/async_support/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/bybit.py` & `ccxt-4.2.92/ccxt/async_support/bybit.py`

 * *Files 0% similar despite different names*

```diff
@@ -381,14 +381,15 @@
                         'v5/lending/info': 5,
                         'v5/lending/history-order': 5,
                         'v5/lending/account': 5,
                         # broker
                         'v5/broker/earning-record': 5,
                         'v5/broker/earnings-info': 5,
                         'v5/broker/account-info': 5,
+                        'v5/broker/asset/query-sub-member-deposit-record': 10,
                     },
                     'post': {
                         # Legacy option USDC
                         'option/usdc/openapi/private/v1/place-order': 2.5,
                         'option/usdc/openapi/private/v1/replace-order': 2.5,
                         'option/usdc/openapi/private/v1/cancel-order': 2.5,
                         'option/usdc/openapi/private/v1/cancel-all': 2.5,
```

### Comparing `ccxt-4.2.91/ccxt/async_support/cex.py` & `ccxt-4.2.92/ccxt/async_support/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/coinbase.py` & `ccxt-4.2.92/ccxt/async_support/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/coinbaseinternational.py` & `ccxt-4.2.92/ccxt/async_support/coinbaseinternational.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/coinbasepro.py` & `ccxt-4.2.92/ccxt/async_support/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/coincheck.py` & `ccxt-4.2.92/ccxt/async_support/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/coinex.py` & `ccxt-4.2.92/ccxt/async_support/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/coinlist.py` & `ccxt-4.2.92/ccxt/async_support/coinlist.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/coinmate.py` & `ccxt-4.2.92/ccxt/async_support/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/coinmetro.py` & `ccxt-4.2.92/ccxt/async_support/coinmetro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/coinone.py` & `ccxt-4.2.92/ccxt/async_support/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/coinsph.py` & `ccxt-4.2.92/ccxt/async_support/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/coinspot.py` & `ccxt-4.2.92/ccxt/async_support/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/cryptocom.py` & `ccxt-4.2.92/ccxt/async_support/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/currencycom.py` & `ccxt-4.2.92/ccxt/async_support/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/delta.py` & `ccxt-4.2.92/ccxt/async_support/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/deribit.py` & `ccxt-4.2.92/ccxt/async_support/deribit.py`

 * *Files 0% similar despite different names*

```diff
@@ -688,125 +688,135 @@
             'code': self.safe_currency_code(None, currency),
         }
 
     async def fetch_markets(self, params={}) -> List[Market]:
         """
         retrieves data on all markets for deribit
         :see: https://docs.deribit.com/#public-get_currencies
+        :see: https://docs.deribit.com/#public-get_instruments
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict[]: an array of objects representing market data
         """
-        currenciesResponse = await self.publicGetGetCurrencies(params)
-        #
-        #     {
-        #         "jsonrpc": "2.0",
-        #         "result": [
-        #             {
-        #                 "withdrawal_priorities": [
-        #                     {value: 0.15, name: "very_low"},
-        #                     {value: 1.5, name: "very_high"},
-        #                 ],
-        #                 "withdrawal_fee": 0.0005,
-        #                 "min_withdrawal_fee": 0.0005,
-        #                 "min_confirmations": 1,
-        #                 "fee_precision": 4,
-        #                 "currency_long": "Bitcoin",
-        #                 "currency": "BTC",
-        #                 "coin_type": "BITCOIN"
-        #             }
-        #         ],
-        #         "usIn": 1583761588590479,
-        #         "usOut": 1583761588590544,
-        #         "usDiff": 65,
-        #         "testnet": False
-        #     }
-        #
-        parsedMarkets = {}
-        currenciesResult = self.safe_value(currenciesResponse, 'result', [])
+        instrumentsResponses = []
         result = []
-        for i in range(0, len(currenciesResult)):
-            currencyId = self.safe_string(currenciesResult[i], 'currency')
-            request = {
-                'currency': currencyId,
-            }
-            instrumentsResponse = await self.publicGetGetInstruments(self.extend(request, params))
+        parsedMarkets = {}
+        fetchAllMarkets = None
+        fetchAllMarkets, params = self.handle_option_and_params(params, 'fetchMarkets', 'fetchAllMarkets', True)
+        if fetchAllMarkets:
+            instrumentsResponse = await self.publicGetGetInstruments(params)
+            instrumentsResponses.append(instrumentsResponse)
+        else:
+            currenciesResponse = await self.publicGetGetCurrencies(params)
             #
             #     {
-            #         "jsonrpc":"2.0",
-            #         "result":[
-            #             {
-            #                 "tick_size":0.0005,
-            #                 "taker_commission":0.0003,
-            #                 "strike":52000.0,
-            #                 "settlement_period":"month",
-            #                 "settlement_currency":"BTC",
-            #                 "quote_currency":"BTC",
-            #                 "option_type":"put",  # put, call
-            #                 "min_trade_amount":0.1,
-            #                 "maker_commission":0.0003,
-            #                 "kind":"option",
-            #                 "is_active":true,
-            #                 "instrument_name":"BTC-24JUN22-52000-P",
-            #                 "expiration_timestamp":1656057600000,
-            #                 "creation_timestamp":1648199543000,
-            #                 "counter_currency":"USD",
-            #                 "contract_size":1.0,
-            #                 "block_trade_commission":0.0003,
-            #                 "base_currency":"BTC"
-            #             },
-            #             {
-            #                 "tick_size":0.5,
-            #                 "taker_commission":0.0005,
-            #                 "settlement_period":"month",  # month, week
-            #                 "settlement_currency":"BTC",
-            #                 "quote_currency":"USD",
-            #                 "min_trade_amount":10.0,
-            #                 "max_liquidation_commission":0.0075,
-            #                 "max_leverage":50,
-            #                 "maker_commission":0.0,
-            #                 "kind":"future",
-            #                 "is_active":true,
-            #                 "instrument_name":"BTC-27MAY22",
-            #                 "future_type":"reversed",
-            #                 "expiration_timestamp":1653638400000,
-            #                 "creation_timestamp":1648195209000,
-            #                 "counter_currency":"USD",
-            #                 "contract_size":10.0,
-            #                 "block_trade_commission":0.0001,
-            #                 "base_currency":"BTC"
-            #             },
+            #         "jsonrpc": "2.0",
+            #         "result": [
             #             {
-            #                 "tick_size":0.5,
-            #                 "taker_commission":0.0005,
-            #                 "settlement_period":"perpetual",
-            #                 "settlement_currency":"BTC",
-            #                 "quote_currency":"USD",
-            #                 "min_trade_amount":10.0,
-            #                 "max_liquidation_commission":0.0075,
-            #                 "max_leverage":50,
-            #                 "maker_commission":0.0,
-            #                 "kind":"future",
-            #                 "is_active":true,
-            #                 "instrument_name":"BTC-PERPETUAL",
-            #                 "future_type":"reversed",
-            #                 "expiration_timestamp":32503708800000,
-            #                 "creation_timestamp":1534242287000,
-            #                 "counter_currency":"USD",
-            #                 "contract_size":10.0,
-            #                 "block_trade_commission":0.0001,
-            #                 "base_currency":"BTC"
-            #             },
+            #                 "withdrawal_priorities": [
+            #                     {value: 0.15, name: "very_low"},
+            #                     {value: 1.5, name: "very_high"},
+            #                 ],
+            #                 "withdrawal_fee": 0.0005,
+            #                 "min_withdrawal_fee": 0.0005,
+            #                 "min_confirmations": 1,
+            #                 "fee_precision": 4,
+            #                 "currency_long": "Bitcoin",
+            #                 "currency": "BTC",
+            #                 "coin_type": "BITCOIN"
+            #             }
             #         ],
-            #         "usIn":1648691472831791,
-            #         "usOut":1648691472831896,
-            #         "usDiff":105,
-            #         "testnet":false
+            #         "usIn": 1583761588590479,
+            #         "usOut": 1583761588590544,
+            #         "usDiff": 65,
+            #         "testnet": False
             #     }
             #
-            instrumentsResult = self.safe_value(instrumentsResponse, 'result', [])
+            currenciesResult = self.safe_value(currenciesResponse, 'result', [])
+            for i in range(0, len(currenciesResult)):
+                currencyId = self.safe_string(currenciesResult[i], 'currency')
+                request = {
+                    'currency': currencyId,
+                }
+                instrumentsResponse = await self.publicGetGetInstruments(self.extend(request, params))
+                #
+                #     {
+                #         "jsonrpc":"2.0",
+                #         "result":[
+                #             {
+                #                 "tick_size":0.0005,
+                #                 "taker_commission":0.0003,
+                #                 "strike":52000.0,
+                #                 "settlement_period":"month",
+                #                 "settlement_currency":"BTC",
+                #                 "quote_currency":"BTC",
+                #                 "option_type":"put",  # put, call
+                #                 "min_trade_amount":0.1,
+                #                 "maker_commission":0.0003,
+                #                 "kind":"option",
+                #                 "is_active":true,
+                #                 "instrument_name":"BTC-24JUN22-52000-P",
+                #                 "expiration_timestamp":1656057600000,
+                #                 "creation_timestamp":1648199543000,
+                #                 "counter_currency":"USD",
+                #                 "contract_size":1.0,
+                #                 "block_trade_commission":0.0003,
+                #                 "base_currency":"BTC"
+                #             },
+                #             {
+                #                 "tick_size":0.5,
+                #                 "taker_commission":0.0005,
+                #                 "settlement_period":"month",  # month, week
+                #                 "settlement_currency":"BTC",
+                #                 "quote_currency":"USD",
+                #                 "min_trade_amount":10.0,
+                #                 "max_liquidation_commission":0.0075,
+                #                 "max_leverage":50,
+                #                 "maker_commission":0.0,
+                #                 "kind":"future",
+                #                 "is_active":true,
+                #                 "instrument_name":"BTC-27MAY22",
+                #                 "future_type":"reversed",
+                #                 "expiration_timestamp":1653638400000,
+                #                 "creation_timestamp":1648195209000,
+                #                 "counter_currency":"USD",
+                #                 "contract_size":10.0,
+                #                 "block_trade_commission":0.0001,
+                #                 "base_currency":"BTC"
+                #             },
+                #             {
+                #                 "tick_size":0.5,
+                #                 "taker_commission":0.0005,
+                #                 "settlement_period":"perpetual",
+                #                 "settlement_currency":"BTC",
+                #                 "quote_currency":"USD",
+                #                 "min_trade_amount":10.0,
+                #                 "max_liquidation_commission":0.0075,
+                #                 "max_leverage":50,
+                #                 "maker_commission":0.0,
+                #                 "kind":"future",
+                #                 "is_active":true,
+                #                 "instrument_name":"BTC-PERPETUAL",
+                #                 "future_type":"reversed",
+                #                 "expiration_timestamp":32503708800000,
+                #                 "creation_timestamp":1534242287000,
+                #                 "counter_currency":"USD",
+                #                 "contract_size":10.0,
+                #                 "block_trade_commission":0.0001,
+                #                 "base_currency":"BTC"
+                #             },
+                #         ],
+                #         "usIn":1648691472831791,
+                #         "usOut":1648691472831896,
+                #         "usDiff":105,
+                #         "testnet":false
+                #     }
+                #
+                instrumentsResponses.append(instrumentsResponse)
+        for i in range(0, len(instrumentsResponses)):
+            instrumentsResult = self.safe_value(instrumentsResponses[i], 'result', [])
             for k in range(0, len(instrumentsResult)):
                 market = instrumentsResult[k]
                 kind = self.safe_string(market, 'kind')
                 isSpot = (kind == 'spot')
                 id = self.safe_string(market, 'instrument_name')
                 baseId = self.safe_string(market, 'base_currency')
                 quoteId = self.safe_string(market, 'counter_currency')
```

### Comparing `ccxt-4.2.91/ccxt/async_support/digifinex.py` & `ccxt-4.2.92/ccxt/async_support/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/exmo.py` & `ccxt-4.2.92/ccxt/async_support/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/flowbtc.py` & `ccxt-4.2.92/ccxt/async_support/flowbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/fmfwio.py` & `ccxt-4.2.92/ccxt/async_support/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/gate.py` & `ccxt-4.2.92/ccxt/async_support/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/gemini.py` & `ccxt-4.2.92/ccxt/async_support/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/hitbtc.py` & `ccxt-4.2.92/ccxt/async_support/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/hollaex.py` & `ccxt-4.2.92/ccxt/async_support/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/htx.py` & `ccxt-4.2.92/ccxt/async_support/htx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/huobijp.py` & `ccxt-4.2.92/ccxt/async_support/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/hyperliquid.py` & `ccxt-4.2.92/ccxt/async_support/hyperliquid.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/idex.py` & `ccxt-4.2.92/ccxt/async_support/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/independentreserve.py` & `ccxt-4.2.92/ccxt/async_support/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/indodax.py` & `ccxt-4.2.92/ccxt/async_support/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/kraken.py` & `ccxt-4.2.92/ccxt/async_support/kraken.py`

 * *Files 1% similar despite different names*

```diff
@@ -7092,570 +7092,692 @@
 0001bb30: 696f 6e73 0a20 2020 2020 2020 203a 7365  ions.        :se
 0001bb40: 653a 2068 7474 7073 3a2f 2f64 6f63 732e  e: https://docs.
 0001bb50: 6b72 616b 656e 2e63 6f6d 2f72 6573 742f  kraken.com/rest/
 0001bb60: 2374 6167 2f41 6363 6f75 6e74 2d44 6174  #tag/Account-Dat
 0001bb70: 612f 6f70 6572 6174 696f 6e2f 6765 744f  a/operation/getO
 0001bb80: 7065 6e50 6f73 6974 696f 6e73 0a20 2020  penPositions.   
 0001bb90: 2020 2020 203a 7061 7261 6d20 7374 725b       :param str[
-0001bba0: 5d7c 4e6f 6e65 2073 796d 626f 6c73 3a20  ]|None symbols: 
-0001bbb0: 6e6f 7420 7573 6564 2062 7920 6b72 616b  not used by krak
-0001bbc0: 656e 2066 6574 6368 506f 7369 7469 6f6e  en fetchPosition
-0001bbd0: 7328 290a 2020 2020 2020 2020 3a70 6172  s().        :par
-0001bbe0: 616d 2064 6963 7420 5b70 6172 616d 735d  am dict [params]
-0001bbf0: 3a20 6578 7472 6120 7061 7261 6d65 7465  : extra paramete
-0001bc00: 7273 2073 7065 6369 6669 6320 746f 2074  rs specific to t
-0001bc10: 6865 2065 7863 6861 6e67 6520 4150 4920  he exchange API 
-0001bc20: 656e 6470 6f69 6e74 0a20 2020 2020 2020  endpoint.       
-0001bc30: 203a 7265 7475 726e 7320 6469 6374 5b5d   :returns dict[]
-0001bc40: 3a20 6120 6c69 7374 206f 6620 6070 6f73  : a list of `pos
-0001bc50: 6974 696f 6e20 7374 7275 6374 7572 6520  ition structure 
-0001bc60: 3c68 7474 7073 3a2f 2f64 6f63 732e 6363  <https://docs.cc
-0001bc70: 7874 2e63 6f6d 2f23 2f3f 6964 3d70 6f73  xt.com/#/?id=pos
-0001bc80: 6974 696f 6e2d 7374 7275 6374 7572 653e  ition-structure>
-0001bc90: 600a 2020 2020 2020 2020 2222 220a 2020  `.        """.  
-0001bca0: 2020 2020 2020 6177 6169 7420 7365 6c66        await self
-0001bcb0: 2e6c 6f61 645f 6d61 726b 6574 7328 290a  .load_markets().
-0001bcc0: 2020 2020 2020 2020 7265 7175 6573 7420          request 
-0001bcd0: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-0001bce0: 2320 2774 7869 6427 3a20 2763 6f6d 6d61  # 'txid': 'comma
-0001bcf0: 2064 656c 696d 6974 6564 206c 6973 7420   delimited list 
-0001bd00: 6f66 2074 7261 6e73 6163 7469 6f6e 2069  of transaction i
-0001bd10: 6473 2074 6f20 7265 7374 7269 6374 206f  ds to restrict o
-0001bd20: 7574 7075 7420 746f 272c 0a20 2020 2020  utput to',.     
-0001bd30: 2020 2020 2020 2023 2027 646f 6361 6c63         # 'docalc
-0001bd40: 7327 3a20 4661 6c73 652c 2020 2320 7768  s': False,  # wh
-0001bd50: 6574 6865 7220 6f72 206e 6f74 2074 6f20  ether or not to 
-0001bd60: 696e 636c 7564 6520 7072 6f66 6974 2f6c  include profit/l
-0001bd70: 6f73 7320 6361 6c63 756c 6174 696f 6e73  oss calculations
-0001bd80: 0a20 2020 2020 2020 2020 2020 2023 2027  .            # '
-0001bd90: 636f 6e73 6f6c 6964 6174 696f 6e27 3a20  consolidation': 
-0001bda0: 276d 6172 6b65 7427 2c20 2023 2077 6861  'market',  # wha
-0001bdb0: 7420 746f 2063 6f6e 736f 6c69 6461 7465  t to consolidate
-0001bdc0: 2074 6865 2070 6f73 6974 696f 6e73 2064   the positions d
-0001bdd0: 6174 6120 6172 6f75 6e64 2c20 6d61 726b  ata around, mark
-0001bde0: 6574 2077 696c 6c20 636f 6e73 6f6c 6964  et will consolid
-0001bdf0: 6174 6520 706f 7369 7469 6f6e 7320 6261  ate positions ba
-0001be00: 7365 6420 6f6e 206d 6172 6b65 7420 7061  sed on market pa
-0001be10: 6972 0a20 2020 2020 2020 207d 0a20 2020  ir.        }.   
-0001be20: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
-0001be30: 6177 6169 7420 7365 6c66 2e70 7269 7661  await self.priva
-0001be40: 7465 506f 7374 4f70 656e 506f 7369 7469  tePostOpenPositi
-0001be50: 6f6e 7328 7365 6c66 2e65 7874 656e 6428  ons(self.extend(
-0001be60: 7265 7175 6573 742c 2070 6172 616d 7329  request, params)
-0001be70: 290a 2020 2020 2020 2020 230a 2020 2020  ).        #.    
-0001be80: 2020 2020 2320 6e6f 2063 6f6e 736f 6c69      # no consoli
-0001be90: 6461 7469 6f6e 0a20 2020 2020 2020 2023  dation.        #
-0001bea0: 0a20 2020 2020 2020 2023 2020 2020 207b  .        #     {
-0001beb0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0001bec0: 2020 2022 6572 726f 7222 3a20 5b5d 2c0a     "error": [],.
-0001bed0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0001bee0: 2020 2272 6573 756c 7422 3a20 7b0a 2020    "result": {.  
-0001bef0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0001bf00: 2020 2020 2754 4755 464d 592d 464c 4553      'TGUFMY-FLES
-0001bf10: 4a2d 5659 4958 334a 273a 207b 0a20 2020  J-VYIX3J': {.   
-0001bf20: 2020 2020 2023 2020 2020 2020 2020 2020       #          
-0001bf30: 2020 2020 2020 2022 6f72 6465 7274 7869         "ordertxi
-0001bf40: 6422 3a20 224f 334c 524e 552d 5a4b 4447  d": "O3LRNU-ZKDG
-0001bf50: 352d 584e 4344 4652 222c 0a20 2020 2020  5-XNCDFR",.     
-0001bf60: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0001bf70: 2020 2020 2022 706f 7373 7461 7475 7322       "posstatus"
-0001bf80: 3a20 226f 7065 6e22 2c0a 2020 2020 2020  : "open",.      
-0001bf90: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-0001bfa0: 2020 2020 2270 6169 7222 3a20 2245 5448      "pair": "ETH
-0001bfb0: 5553 4454 222c 0a20 2020 2020 2020 2023  USDT",.        #
-0001bfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bfd0: 2022 7469 6d65 223a 2020 3136 3131 3535   "time":  161155
-0001bfe0: 3732 3331 2e34 3538 342c 0a20 2020 2020  7231.4584,.     
-0001bff0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0001c000: 2020 2020 2022 7479 7065 223a 2022 6275       "type": "bu
-0001c010: 7922 2c0a 2020 2020 2020 2020 2320 2020  y",.        #   
-0001c020: 2020 2020 2020 2020 2020 2020 2020 226f                "o
-0001c030: 7264 6572 7479 7065 223a 2022 6d61 726b  rdertype": "mark
-0001c040: 6574 222c 0a20 2020 2020 2020 2023 2020  et",.        #  
-0001c050: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0001c060: 636f 7374 223a 2022 3238 2e34 3938 3030  cost": "28.49800
-0001c070: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
-0001c080: 2020 2020 2020 2020 2020 2020 2022 6665               "fe
-0001c090: 6522 3a20 2230 2e30 3739 3739 222c 0a20  e": "0.07979",. 
-0001c0a0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0001c0b0: 2020 2020 2020 2020 2022 766f 6c22 3a20           "vol": 
-0001c0c0: 2230 2e30 3230 3030 3030 3022 2c0a 2020  "0.02000000",.  
-0001c0d0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0001c0e0: 2020 2020 2020 2020 2276 6f6c 5f63 6c6f          "vol_clo
-0001c0f0: 7365 6422 3a20 2230 2e30 3030 3030 3030  sed": "0.0000000
-0001c100: 3022 2c0a 2020 2020 2020 2020 2320 2020  0",.        #   
-0001c110: 2020 2020 2020 2020 2020 2020 2020 226d                "m
-0001c120: 6172 6769 6e22 3a20 2231 342e 3234 3930  argin": "14.2490
-0001c130: 3022 2c0a 2020 2020 2020 2020 2320 2020  0",.        #   
-0001c140: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-0001c150: 6572 6d73 223a 2022 302e 3032 3030 2520  erms": "0.0200% 
-0001c160: 7065 7220 3420 686f 7572 7322 2c0a 2020  per 4 hours",.  
-0001c170: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0001c180: 2020 2020 2020 2020 2272 6f6c 6c6f 7665          "rollove
-0001c190: 7274 6d22 3a20 2231 3631 3135 3731 3633  rtm": "161157163
-0001c1a0: 3122 2c0a 2020 2020 2020 2020 2320 2020  1",.        #   
-0001c1b0: 2020 2020 2020 2020 2020 2020 2020 226d                "m
-0001c1c0: 6973 6322 3a20 2222 2c0a 2020 2020 2020  isc": "",.      
-0001c1d0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-0001c1e0: 2020 2020 226f 666c 6167 7322 3a20 2222      "oflags": ""
-0001c1f0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0001c200: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-0001c210: 2023 2020 2020 2020 2020 207d 0a20 2020   #         }.   
-0001c220: 2020 2020 2023 2020 2020 207d 0a20 2020       #     }.   
-0001c230: 2020 2020 2023 0a20 2020 2020 2020 2023       #.        #
-0001c240: 2063 6f6e 736f 6c69 6461 7469 6f6e 2062   consolidation b
-0001c250: 7920 6d61 726b 6574 0a20 2020 2020 2020  y market.       
-0001c260: 2023 0a20 2020 2020 2020 2023 2020 2020   #.        #    
-0001c270: 207b 0a20 2020 2020 2020 2023 2020 2020   {.        #    
-0001c280: 2020 2020 2022 6572 726f 7222 3a20 5b5d       "error": []
-0001c290: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
-0001c2a0: 2020 2020 2272 6573 756c 7422 3a20 5b0a      "result": [.
-0001c2b0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0001c2c0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-0001c2d0: 2320 2020 2020 2020 2020 2020 2020 2020  #               
-0001c2e0: 2020 2270 6169 7222 3a20 2245 5448 5553    "pair": "ETHUS
-0001c2f0: 4454 222c 0a20 2020 2020 2020 2023 2020  DT",.        #  
-0001c300: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0001c310: 706f 7369 7469 6f6e 7322 3a20 2231 222c  positions": "1",
-0001c320: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0001c330: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-0001c340: 223a 2022 6275 7922 2c0a 2020 2020 2020  ": "buy",.      
-0001c350: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-0001c360: 2020 2020 226c 6576 6572 6167 6522 3a20      "leverage": 
-0001c370: 2232 2e30 3030 3030 222c 0a20 2020 2020  "2.00000",.     
-0001c380: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0001c390: 2020 2020 2022 636f 7374 223a 2022 3238       "cost": "28
-0001c3a0: 2e34 3938 3030 222c 0a20 2020 2020 2020  .49800",.       
-0001c3b0: 2023 2020 2020 2020 2020 2020 2020 2020   #              
-0001c3c0: 2020 2022 6665 6522 3a20 2230 2e30 3739     "fee": "0.079
-0001c3d0: 3739 222c 0a20 2020 2020 2020 2023 2020  79",.        #  
-0001c3e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0001c3f0: 766f 6c22 3a20 2230 2e30 3230 3030 3030  vol": "0.0200000
-0001c400: 3022 2c0a 2020 2020 2020 2020 2320 2020  0",.        #   
-0001c410: 2020 2020 2020 2020 2020 2020 2020 2276                "v
-0001c420: 6f6c 5f63 6c6f 7365 6422 3a20 2230 2e30  ol_closed": "0.0
-0001c430: 3030 3030 3030 3022 2c0a 2020 2020 2020  0000000",.      
-0001c440: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-0001c450: 2020 2020 226d 6172 6769 6e22 3a20 2231      "margin": "1
-0001c460: 342e 3234 3930 3022 0a20 2020 2020 2020  4.24900".       
-0001c470: 2023 2020 2020 2020 2020 2020 2020 207d   #             }
-0001c480: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0001c490: 2020 205d 0a20 2020 2020 2020 2023 2020     ].        #  
-0001c4a0: 2020 207d 0a20 2020 2020 2020 2023 0a20     }.        #. 
-0001c4b0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-0001c4c0: 7365 6c66 2e73 6166 655f 7661 6c75 6528  self.safe_value(
-0001c4d0: 7265 7370 6f6e 7365 2c20 2772 6573 756c  response, 'resul
-0001c4e0: 7427 290a 2020 2020 2020 2020 2320 746f  t').        # to
-0001c4f0: 646f 2075 6e69 6679 2070 6172 7365 506f  do unify parsePo
-0001c500: 7369 7469 6f6e 2f70 6172 7365 506f 7369  sition/parsePosi
-0001c510: 7469 6f6e 730a 2020 2020 2020 2020 7265  tions.        re
-0001c520: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-0001c530: 2064 6566 2070 6172 7365 5f61 6363 6f75   def parse_accou
-0001c540: 6e74 5f74 7970 6528 7365 6c66 2c20 6163  nt_type(self, ac
-0001c550: 636f 756e 7429 3a0a 2020 2020 2020 2020  count):.        
-0001c560: 6163 636f 756e 7442 7954 7970 6520 3d20  accountByType = 
-0001c570: 7b0a 2020 2020 2020 2020 2020 2020 2773  {.            's
-0001c580: 706f 7427 3a20 2753 706f 7420 5761 6c6c  pot': 'Spot Wall
-0001c590: 6574 272c 0a20 2020 2020 2020 2020 2020  et',.           
-0001c5a0: 2027 7377 6170 273a 2027 4675 7475 7265   'swap': 'Future
-0001c5b0: 7320 5761 6c6c 6574 272c 0a20 2020 2020  s Wallet',.     
-0001c5c0: 2020 2020 2020 2027 6675 7475 7265 273a         'future':
-0001c5d0: 2027 4675 7475 7265 7320 5761 6c6c 6574   'Futures Wallet
-0001c5e0: 272c 0a20 2020 2020 2020 207d 0a20 2020  ',.        }.   
-0001c5f0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0001c600: 2e73 6166 655f 7374 7269 6e67 2861 6363  .safe_string(acc
-0001c610: 6f75 6e74 4279 5479 7065 2c20 6163 636f  ountByType, acco
-0001c620: 756e 742c 2061 6363 6f75 6e74 290a 0a20  unt, account).. 
-0001c630: 2020 2061 7379 6e63 2064 6566 2074 7261     async def tra
-0001c640: 6e73 6665 725f 6f75 7428 7365 6c66 2c20  nsfer_out(self, 
-0001c650: 636f 6465 3a20 7374 722c 2061 6d6f 756e  code: str, amoun
-0001c660: 742c 2070 6172 616d 733d 7b7d 293a 0a20  t, params={}):. 
-0001c670: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0001c680: 2020 2074 7261 6e73 6665 7220 6672 6f6d     transfer from
-0001c690: 2073 706f 7420 7761 6c6c 6574 2074 6f20   spot wallet to 
-0001c6a0: 6675 7475 7265 7320 7761 6c6c 6574 0a20  futures wallet. 
-0001c6b0: 2020 2020 2020 203a 7365 653a 2068 7474         :see: htt
-0001c6c0: 7073 3a2f 2f64 6f63 732e 6b72 616b 656e  ps://docs.kraken
-0001c6d0: 2e63 6f6d 2f72 6573 742f 2374 6167 2f55  .com/rest/#tag/U
-0001c6e0: 7365 722d 4675 6e64 696e 672f 6f70 6572  ser-Funding/oper
-0001c6f0: 6174 696f 6e2f 7761 6c6c 6574 5472 616e  ation/walletTran
-0001c700: 7366 6572 0a20 2020 2020 2020 203a 7061  sfer.        :pa
-0001c710: 7261 6d20 7374 7220 636f 6465 3a20 556e  ram str code: Un
-0001c720: 6966 6965 6420 6375 7272 656e 6379 2063  ified currency c
-0001c730: 6f64 650a 2020 2020 2020 2020 3a70 6172  ode.        :par
-0001c740: 616d 2066 6c6f 6174 2061 6d6f 756e 743a  am float amount:
-0001c750: 2053 697a 6520 6f66 2074 6865 2074 7261   Size of the tra
-0001c760: 6e73 6665 720a 2020 2020 2020 2020 3a70  nsfer.        :p
-0001c770: 6172 616d 2064 6963 7420 5b70 6172 616d  aram dict [param
-0001c780: 735d 3a20 4578 6368 616e 6765 2073 7065  s]: Exchange spe
-0001c790: 6369 6669 6320 7061 7261 6d65 7465 7273  cific parameters
-0001c7a0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-0001c7b0: 733a 2061 2060 7472 616e 7366 6572 2073  s: a `transfer s
-0001c7c0: 7472 7563 7475 7265 203c 6874 7470 733a  tructure <https:
-0001c7d0: 2f2f 646f 6373 2e63 6378 742e 636f 6d2f  //docs.ccxt.com/
-0001c7e0: 232f 3f69 643d 7472 616e 7366 6572 2d73  #/?id=transfer-s
-0001c7f0: 7472 7563 7475 7265 3e60 0a20 2020 2020  tructure>`.     
-0001c800: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-0001c810: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
-0001c820: 2e74 7261 6e73 6665 7228 636f 6465 2c20  .transfer(code, 
-0001c830: 616d 6f75 6e74 2c20 2773 706f 7427 2c20  amount, 'spot', 
-0001c840: 2773 7761 7027 2c20 7061 7261 6d73 290a  'swap', params).
-0001c850: 0a20 2020 2061 7379 6e63 2064 6566 2074  .    async def t
-0001c860: 7261 6e73 6665 7228 7365 6c66 2c20 636f  ransfer(self, co
-0001c870: 6465 3a20 7374 722c 2061 6d6f 756e 743a  de: str, amount:
-0001c880: 2066 6c6f 6174 2c20 6672 6f6d 4163 636f   float, fromAcco
-0001c890: 756e 743a 2073 7472 2c20 746f 4163 636f  unt: str, toAcco
-0001c8a0: 756e 743a 2073 7472 2c20 7061 7261 6d73  unt: str, params
-0001c8b0: 3d7b 7d29 202d 3e20 5472 616e 7366 6572  ={}) -> Transfer
-0001c8c0: 456e 7472 793a 0a20 2020 2020 2020 2022  Entry:.        "
-0001c8d0: 2222 0a20 2020 2020 2020 203a 7365 653a  "".        :see:
-0001c8e0: 2068 7474 7073 3a2f 2f64 6f63 732e 6b72   https://docs.kr
-0001c8f0: 616b 656e 2e63 6f6d 2f72 6573 742f 2374  aken.com/rest/#t
-0001c900: 6167 2f55 7365 722d 4675 6e64 696e 672f  ag/User-Funding/
-0001c910: 6f70 6572 6174 696f 6e2f 7761 6c6c 6574  operation/wallet
-0001c920: 5472 616e 7366 6572 0a20 2020 2020 2020  Transfer.       
-0001c930: 2074 7261 6e73 6665 7273 2063 7572 7265   transfers curre
-0001c940: 6e63 6965 7320 6265 7477 6565 6e20 7375  ncies between su
-0001c950: 622d 6163 636f 756e 7473 286f 6e6c 7920  b-accounts(only 
-0001c960: 7370 6f74 2d3e 7377 6170 2064 6972 6563  spot->swap direc
-0001c970: 7469 6f6e 2069 7320 7375 7070 6f72 7465  tion is supporte
-0001c980: 6429 0a20 2020 2020 2020 203a 7061 7261  d).        :para
-0001c990: 6d20 7374 7220 636f 6465 3a20 556e 6966  m str code: Unif
-0001c9a0: 6965 6420 6375 7272 656e 6379 2063 6f64  ied currency cod
-0001c9b0: 650a 2020 2020 2020 2020 3a70 6172 616d  e.        :param
-0001c9c0: 2066 6c6f 6174 2061 6d6f 756e 743a 2053   float amount: S
-0001c9d0: 697a 6520 6f66 2074 6865 2074 7261 6e73  ize of the trans
-0001c9e0: 6665 720a 2020 2020 2020 2020 3a70 6172  fer.        :par
-0001c9f0: 616d 2073 7472 2066 726f 6d41 6363 6f75  am str fromAccou
-0001ca00: 6e74 3a20 2773 706f 7427 206f 7220 2753  nt: 'spot' or 'S
-0001ca10: 706f 7420 5761 6c6c 6574 270a 2020 2020  pot Wallet'.    
-0001ca20: 2020 2020 3a70 6172 616d 2073 7472 2074      :param str t
-0001ca30: 6f41 6363 6f75 6e74 3a20 2773 7761 7027  oAccount: 'swap'
-0001ca40: 206f 7220 2746 7574 7572 6573 2057 616c   or 'Futures Wal
-0001ca50: 6c65 7427 0a20 2020 2020 2020 203a 7061  let'.        :pa
-0001ca60: 7261 6d20 6469 6374 205b 7061 7261 6d73  ram dict [params
-0001ca70: 5d3a 2045 7863 6861 6e67 6520 7370 6563  ]: Exchange spec
-0001ca80: 6966 6963 2070 6172 616d 6574 6572 730a  ific parameters.
-0001ca90: 2020 2020 2020 2020 3a72 6574 7572 6e73          :returns
-0001caa0: 3a20 6120 6074 7261 6e73 6665 7220 7374  : a `transfer st
-0001cab0: 7275 6374 7572 6520 3c68 7474 7073 3a2f  ructure <https:/
-0001cac0: 2f64 6f63 732e 6363 7874 2e63 6f6d 2f23  /docs.ccxt.com/#
-0001cad0: 2f3f 6964 3d74 7261 6e73 6665 722d 7374  /?id=transfer-st
-0001cae0: 7275 6374 7572 653e 600a 2020 2020 2020  ructure>`.      
-0001caf0: 2020 2222 220a 2020 2020 2020 2020 6177    """.        aw
-0001cb00: 6169 7420 7365 6c66 2e6c 6f61 645f 6d61  ait self.load_ma
-0001cb10: 726b 6574 7328 290a 2020 2020 2020 2020  rkets().        
-0001cb20: 6375 7272 656e 6379 203d 2073 656c 662e  currency = self.
-0001cb30: 6375 7272 656e 6379 2863 6f64 6529 0a20  currency(code). 
-0001cb40: 2020 2020 2020 2066 726f 6d41 6363 6f75         fromAccou
-0001cb50: 6e74 203d 2073 656c 662e 7061 7273 655f  nt = self.parse_
-0001cb60: 6163 636f 756e 745f 7479 7065 2866 726f  account_type(fro
-0001cb70: 6d41 6363 6f75 6e74 290a 2020 2020 2020  mAccount).      
-0001cb80: 2020 746f 4163 636f 756e 7420 3d20 7365    toAccount = se
-0001cb90: 6c66 2e70 6172 7365 5f61 6363 6f75 6e74  lf.parse_account
-0001cba0: 5f74 7970 6528 746f 4163 636f 756e 7429  _type(toAccount)
-0001cbb0: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
-0001cbc0: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
-0001cbd0: 2027 616d 6f75 6e74 273a 2073 656c 662e   'amount': self.
-0001cbe0: 6375 7272 656e 6379 5f74 6f5f 7072 6563  currency_to_prec
-0001cbf0: 6973 696f 6e28 636f 6465 2c20 616d 6f75  ision(code, amou
-0001cc00: 6e74 292c 0a20 2020 2020 2020 2020 2020  nt),.           
-0001cc10: 2027 6672 6f6d 273a 2066 726f 6d41 6363   'from': fromAcc
-0001cc20: 6f75 6e74 2c0a 2020 2020 2020 2020 2020  ount,.          
-0001cc30: 2020 2774 6f27 3a20 746f 4163 636f 756e    'to': toAccoun
-0001cc40: 742c 0a20 2020 2020 2020 2020 2020 2027  t,.            '
-0001cc50: 6173 7365 7427 3a20 6375 7272 656e 6379  asset': currency
-0001cc60: 5b27 6964 275d 2c0a 2020 2020 2020 2020  ['id'],.        
-0001cc70: 7d0a 2020 2020 2020 2020 6966 2066 726f  }.        if fro
-0001cc80: 6d41 6363 6f75 6e74 2021 3d20 2753 706f  mAccount != 'Spo
-0001cc90: 7420 5761 6c6c 6574 273a 0a20 2020 2020  t Wallet':.     
-0001cca0: 2020 2020 2020 2072 6169 7365 2042 6164         raise Bad
-0001ccb0: 5265 7175 6573 7428 7365 6c66 2e69 6420  Request(self.id 
-0001ccc0: 2b20 2720 7472 616e 7366 6572 2063 616e  + ' transfer can
-0001ccd0: 6e6f 7420 7472 616e 7366 6572 2066 726f  not transfer fro
-0001cce0: 6d20 2720 2b20 6672 6f6d 4163 636f 756e  m ' + fromAccoun
-0001ccf0: 7420 2b20 2720 746f 2027 202b 2074 6f41  t + ' to ' + toA
-0001cd00: 6363 6f75 6e74 202b 2027 2e20 5573 6520  ccount + '. Use 
-0001cd10: 6b72 616b 656e 6675 7475 7265 7320 696e  krakenfutures in
-0001cd20: 7374 6561 6420 746f 2074 7261 6e73 6665  stead to transfe
-0001cd30: 7220 6672 6f6d 2074 6865 2066 7574 7572  r from the futur
-0001cd40: 6573 2061 6363 6f75 6e74 2e27 290a 2020  es account.').  
-0001cd50: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-0001cd60: 2061 7761 6974 2073 656c 662e 7072 6976   await self.priv
-0001cd70: 6174 6550 6f73 7457 616c 6c65 7454 7261  atePostWalletTra
-0001cd80: 6e73 6665 7228 7365 6c66 2e65 7874 656e  nsfer(self.exten
-0001cd90: 6428 7265 7175 6573 742c 2070 6172 616d  d(request, param
-0001cda0: 7329 290a 2020 2020 2020 2020 230a 2020  s)).        #.  
-0001cdb0: 2020 2020 2020 2320 2020 7b0a 2020 2020        #   {.    
-0001cdc0: 2020 2020 2320 2020 2020 2020 2265 7272      #       "err
-0001cdd0: 6f72 223a 5b0a 2020 2020 2020 2020 2320  or":[.        # 
-0001cde0: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
-0001cdf0: 2023 2020 2020 2020 2022 7265 7375 6c74   #       "result
-0001ce00: 223a 7b0a 2020 2020 2020 2020 2320 2020  ":{.        #   
-0001ce10: 2020 2020 2020 2022 7265 6669 6422 3a22         "refid":"
-0001ce20: 424f 4955 5349 462d 4d37 444c 4d4e 2d55  BOIUSIF-M7DLMN-U
-0001ce30: 585a 3350 3522 0a20 2020 2020 2020 2023  XZ3P5".        #
-0001ce40: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-0001ce50: 2023 2020 207d 0a20 2020 2020 2020 2023   #   }.        #
-0001ce60: 0a20 2020 2020 2020 2074 7261 6e73 6665  .        transfe
-0001ce70: 7220 3d20 7365 6c66 2e70 6172 7365 5f74  r = self.parse_t
-0001ce80: 7261 6e73 6665 7228 7265 7370 6f6e 7365  ransfer(response
-0001ce90: 2c20 6375 7272 656e 6379 290a 2020 2020  , currency).    
-0001cea0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0001ceb0: 6578 7465 6e64 2874 7261 6e73 6665 722c  extend(transfer,
-0001cec0: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
-0001ced0: 616d 6f75 6e74 273a 2061 6d6f 756e 742c  amount': amount,
-0001cee0: 0a20 2020 2020 2020 2020 2020 2027 6672  .            'fr
-0001cef0: 6f6d 4163 636f 756e 7427 3a20 6672 6f6d  omAccount': from
-0001cf00: 4163 636f 756e 742c 0a20 2020 2020 2020  Account,.       
-0001cf10: 2020 2020 2027 746f 4163 636f 756e 7427       'toAccount'
-0001cf20: 3a20 746f 4163 636f 756e 742c 0a20 2020  : toAccount,.   
-0001cf30: 2020 2020 207d 290a 0a20 2020 2064 6566       })..    def
-0001cf40: 2070 6172 7365 5f74 7261 6e73 6665 7228   parse_transfer(
-0001cf50: 7365 6c66 2c20 7472 616e 7366 6572 2c20  self, transfer, 
-0001cf60: 6375 7272 656e 6379 3a20 4375 7272 656e  currency: Curren
-0001cf70: 6379 203d 204e 6f6e 6529 3a0a 2020 2020  cy = None):.    
-0001cf80: 2020 2020 230a 2020 2020 2020 2020 2320      #.        # 
-0001cf90: 7472 616e 7366 6572 0a20 2020 2020 2020  transfer.       
-0001cfa0: 2023 0a20 2020 2020 2020 2023 2020 2020   #.        #    
-0001cfb0: 7b0a 2020 2020 2020 2020 2320 2020 2020  {.        #     
-0001cfc0: 2020 2022 6572 726f 7222 3a5b 0a20 2020     "error":[.   
-0001cfd0: 2020 2020 2023 2020 2020 2020 2020 5d2c       #        ],
-0001cfe0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0001cff0: 2020 2272 6573 756c 7422 3a7b 0a20 2020    "result":{.   
-0001d000: 2020 2020 2023 2020 2020 2020 2020 2020       #          
-0001d010: 2022 7265 6669 6422 3a22 424f 4955 5349   "refid":"BOIUSI
-0001d020: 462d 4d37 444c 4d4e 2d55 585a 3350 3522  F-M7DLMN-UXZ3P5"
-0001d030: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0001d040: 2020 7d0a 2020 2020 2020 2020 2320 2020    }.        #   
-0001d050: 207d 0a20 2020 2020 2020 2023 0a20 2020   }.        #.   
-0001d060: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
-0001d070: 6c66 2e73 6166 655f 7661 6c75 6528 7472  lf.safe_value(tr
-0001d080: 616e 7366 6572 2c20 2772 6573 756c 7427  ansfer, 'result'
-0001d090: 2c20 7b7d 290a 2020 2020 2020 2020 7265  , {}).        re
-0001d0a0: 6669 6420 3d20 7365 6c66 2e73 6166 655f  fid = self.safe_
-0001d0b0: 7374 7269 6e67 2872 6573 756c 742c 2027  string(result, '
-0001d0c0: 7265 6669 6427 290a 2020 2020 2020 2020  refid').        
-0001d0d0: 7265 7475 726e 207b 0a20 2020 2020 2020  return {.       
-0001d0e0: 2020 2020 2027 696e 666f 273a 2074 7261       'info': tra
-0001d0f0: 6e73 6665 722c 0a20 2020 2020 2020 2020  nsfer,.         
-0001d100: 2020 2027 6964 273a 2072 6566 6964 2c0a     'id': refid,.
-0001d110: 2020 2020 2020 2020 2020 2020 2774 696d              'tim
-0001d120: 6573 7461 6d70 273a 204e 6f6e 652c 0a20  estamp': None,. 
-0001d130: 2020 2020 2020 2020 2020 2027 6461 7465             'date
-0001d140: 7469 6d65 273a 204e 6f6e 652c 0a20 2020  time': None,.   
-0001d150: 2020 2020 2020 2020 2027 6375 7272 656e           'curren
-0001d160: 6379 273a 2073 656c 662e 7361 6665 5f73  cy': self.safe_s
-0001d170: 7472 696e 6728 6375 7272 656e 6379 2c20  tring(currency, 
-0001d180: 2763 6f64 6527 292c 0a20 2020 2020 2020  'code'),.       
-0001d190: 2020 2020 2027 616d 6f75 6e74 273a 204e       'amount': N
-0001d1a0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-0001d1b0: 2027 6672 6f6d 4163 636f 756e 7427 3a20   'fromAccount': 
-0001d1c0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-0001d1d0: 2020 2774 6f41 6363 6f75 6e74 273a 204e    'toAccount': N
-0001d1e0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-0001d1f0: 2027 7374 6174 7573 273a 2027 7375 6365   'status': 'suce
-0001d200: 7373 272c 0a20 2020 2020 2020 207d 0a0a  ss',.        }..
-0001d210: 2020 2020 6465 6620 7369 676e 2873 656c      def sign(sel
-0001d220: 662c 2070 6174 682c 2061 7069 3d27 7075  f, path, api='pu
-0001d230: 626c 6963 272c 206d 6574 686f 643d 2747  blic', method='G
-0001d240: 4554 272c 2070 6172 616d 733d 7b7d 2c20  ET', params={}, 
-0001d250: 6865 6164 6572 733d 4e6f 6e65 2c20 626f  headers=None, bo
-0001d260: 6479 3d4e 6f6e 6529 3a0a 2020 2020 2020  dy=None):.      
-0001d270: 2020 7572 6c20 3d20 272f 2720 2b20 7365    url = '/' + se
-0001d280: 6c66 2e76 6572 7369 6f6e 202b 2027 2f27  lf.version + '/'
-0001d290: 202b 2061 7069 202b 2027 2f27 202b 2070   + api + '/' + p
-0001d2a0: 6174 680a 2020 2020 2020 2020 6966 2061  ath.        if a
-0001d2b0: 7069 203d 3d20 2770 7562 6c69 6327 3a0a  pi == 'public':.
-0001d2c0: 2020 2020 2020 2020 2020 2020 6966 2070              if p
-0001d2d0: 6172 616d 733a 0a20 2020 2020 2020 2020  arams:.         
-0001d2e0: 2020 2020 2020 2023 2075 726c 656e 636f         # urlenco
-0001d2f0: 6465 4e65 7374 6564 2069 7320 7573 6564  deNested is used
-0001d300: 2074 6f20 6164 6472 6573 7320 6874 7470   to address http
-0001d310: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
-0001d320: 6378 742f 6363 7874 2f69 7373 7565 732f  cxt/ccxt/issues/
-0001d330: 3132 3837 320a 2020 2020 2020 2020 2020  12872.          
-0001d340: 2020 2020 2020 7572 6c20 2b3d 2027 3f27        url += '?'
-0001d350: 202b 2073 656c 662e 7572 6c65 6e63 6f64   + self.urlencod
-0001d360: 655f 6e65 7374 6564 2870 6172 616d 7329  e_nested(params)
-0001d370: 0a20 2020 2020 2020 2065 6c69 6620 6170  .        elif ap
-0001d380: 6920 3d3d 2027 7072 6976 6174 6527 3a0a  i == 'private':.
-0001d390: 2020 2020 2020 2020 2020 2020 6973 4361              isCa
-0001d3a0: 6e63 656c 4f72 6465 7242 6174 6368 203d  ncelOrderBatch =
-0001d3b0: 2028 7061 7468 203d 3d20 2743 616e 6365   (path == 'Cance
-0001d3c0: 6c4f 7264 6572 4261 7463 6827 290a 2020  lOrderBatch').  
-0001d3d0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0001d3e0: 6865 636b 5f72 6571 7569 7265 645f 6372  heck_required_cr
-0001d3f0: 6564 656e 7469 616c 7328 290a 2020 2020  edentials().    
-0001d400: 2020 2020 2020 2020 6e6f 6e63 6520 3d20          nonce = 
-0001d410: 7374 7228 7365 6c66 2e6e 6f6e 6365 2829  str(self.nonce()
-0001d420: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
-0001d430: 7572 6c65 6e63 6f64 654e 6573 7465 6420  urlencodeNested 
-0001d440: 6973 2075 7365 6420 746f 2061 6464 7265  is used to addre
-0001d450: 7373 2068 7474 7073 3a2f 2f67 6974 6875  ss https://githu
-0001d460: 622e 636f 6d2f 6363 7874 2f63 6378 742f  b.com/ccxt/ccxt/
-0001d470: 6973 7375 6573 2f31 3238 3732 0a20 2020  issues/12872.   
-0001d480: 2020 2020 2020 2020 2069 6620 6973 4361           if isCa
-0001d490: 6e63 656c 4f72 6465 7242 6174 6368 3a0a  ncelOrderBatch:.
-0001d4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d4b0: 626f 6479 203d 2073 656c 662e 6a73 6f6e  body = self.json
-0001d4c0: 2873 656c 662e 6578 7465 6e64 287b 276e  (self.extend({'n
-0001d4d0: 6f6e 6365 273a 206e 6f6e 6365 7d2c 2070  once': nonce}, p
-0001d4e0: 6172 616d 7329 290a 2020 2020 2020 2020  arams)).        
-0001d4f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0001d500: 2020 2020 2020 2020 2020 626f 6479 203d            body =
-0001d510: 2073 656c 662e 7572 6c65 6e63 6f64 655f   self.urlencode_
-0001d520: 6e65 7374 6564 2873 656c 662e 6578 7465  nested(self.exte
-0001d530: 6e64 287b 276e 6f6e 6365 273a 206e 6f6e  nd({'nonce': non
-0001d540: 6365 7d2c 2070 6172 616d 7329 290a 2020  ce}, params)).  
-0001d550: 2020 2020 2020 2020 2020 6175 7468 203d            auth =
-0001d560: 2073 656c 662e 656e 636f 6465 286e 6f6e   self.encode(non
-0001d570: 6365 202b 2062 6f64 7929 0a20 2020 2020  ce + body).     
-0001d580: 2020 2020 2020 2068 6173 6820 3d20 7365         hash = se
-0001d590: 6c66 2e68 6173 6828 6175 7468 2c20 2773  lf.hash(auth, 's
-0001d5a0: 6861 3235 3627 2c20 2762 696e 6172 7927  ha256', 'binary'
-0001d5b0: 290a 2020 2020 2020 2020 2020 2020 6269  ).            bi
-0001d5c0: 6e61 7279 203d 2073 656c 662e 656e 636f  nary = self.enco
-0001d5d0: 6465 2875 726c 290a 2020 2020 2020 2020  de(url).        
-0001d5e0: 2020 2020 6269 6e68 6173 6820 3d20 7365      binhash = se
-0001d5f0: 6c66 2e62 696e 6172 795f 636f 6e63 6174  lf.binary_concat
-0001d600: 2862 696e 6172 792c 2068 6173 6829 0a20  (binary, hash). 
-0001d610: 2020 2020 2020 2020 2020 2073 6563 7265             secre
-0001d620: 7420 3d20 7365 6c66 2e62 6173 6536 345f  t = self.base64_
-0001d630: 746f 5f62 696e 6172 7928 7365 6c66 2e73  to_binary(self.s
-0001d640: 6563 7265 7429 0a20 2020 2020 2020 2020  ecret).         
-0001d650: 2020 2073 6967 6e61 7475 7265 203d 2073     signature = s
-0001d660: 656c 662e 686d 6163 2862 696e 6861 7368  elf.hmac(binhash
-0001d670: 2c20 7365 6372 6574 2c20 6861 7368 6c69  , secret, hashli
-0001d680: 622e 7368 6135 3132 2c20 2762 6173 6536  b.sha512, 'base6
-0001d690: 3427 290a 2020 2020 2020 2020 2020 2020  4').            
-0001d6a0: 6865 6164 6572 7320 3d20 7b0a 2020 2020  headers = {.    
-0001d6b0: 2020 2020 2020 2020 2020 2020 2741 5049              'API
-0001d6c0: 2d4b 6579 273a 2073 656c 662e 6170 694b  -Key': self.apiK
-0001d6d0: 6579 2c0a 2020 2020 2020 2020 2020 2020  ey,.            
-0001d6e0: 2020 2020 2741 5049 2d53 6967 6e27 3a20      'API-Sign': 
-0001d6f0: 7369 676e 6174 7572 652c 0a20 2020 2020  signature,.     
-0001d700: 2020 2020 2020 2020 2020 2023 2027 436f             # 'Co
-0001d710: 6e74 656e 742d 5479 7065 273a 2027 6170  ntent-Type': 'ap
-0001d720: 706c 6963 6174 696f 6e2f 782d 7777 772d  plication/x-www-
-0001d730: 666f 726d 2d75 726c 656e 636f 6465 6427  form-urlencoded'
-0001d740: 2c0a 2020 2020 2020 2020 2020 2020 7d0a  ,.            }.
-0001d750: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-0001d760: 7343 616e 6365 6c4f 7264 6572 4261 7463  sCancelOrderBatc
-0001d770: 683a 0a20 2020 2020 2020 2020 2020 2020  h:.             
-0001d780: 2020 2068 6561 6465 7273 5b27 436f 6e74     headers['Cont
-0001d790: 656e 742d 5479 7065 275d 203d 2027 6170  ent-Type'] = 'ap
-0001d7a0: 706c 6963 6174 696f 6e2f 6a73 6f6e 270a  plication/json'.
-0001d7b0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0001d7c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001d7d0: 2020 6865 6164 6572 735b 2743 6f6e 7465    headers['Conte
-0001d7e0: 6e74 2d54 7970 6527 5d20 3d20 2761 7070  nt-Type'] = 'app
-0001d7f0: 6c69 6361 7469 6f6e 2f78 2d77 7777 2d66  lication/x-www-f
-0001d800: 6f72 6d2d 7572 6c65 6e63 6f64 6564 270a  orm-urlencoded'.
-0001d810: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0001d820: 2020 2020 2020 2020 2020 7572 6c20 3d20            url = 
-0001d830: 272f 2720 2b20 7061 7468 0a20 2020 2020  '/' + path.     
-0001d840: 2020 2075 726c 203d 2073 656c 662e 7572     url = self.ur
-0001d850: 6c73 5b27 6170 6927 5d5b 6170 695d 202b  ls['api'][api] +
-0001d860: 2075 726c 0a20 2020 2020 2020 2072 6574   url.        ret
-0001d870: 7572 6e20 7b27 7572 6c27 3a20 7572 6c2c  urn {'url': url,
-0001d880: 2027 6d65 7468 6f64 273a 206d 6574 686f   'method': metho
-0001d890: 642c 2027 626f 6479 273a 2062 6f64 792c  d, 'body': body,
-0001d8a0: 2027 6865 6164 6572 7327 3a20 6865 6164   'headers': head
-0001d8b0: 6572 737d 0a0a 2020 2020 6465 6620 6e6f  ers}..    def no
-0001d8c0: 6e63 6528 7365 6c66 293a 0a20 2020 2020  nce(self):.     
-0001d8d0: 2020 2072 6574 7572 6e20 7365 6c66 2e6d     return self.m
-0001d8e0: 696c 6c69 7365 636f 6e64 7328 290a 0a20  illiseconds().. 
-0001d8f0: 2020 2064 6566 2068 616e 646c 655f 6572     def handle_er
-0001d900: 726f 7273 2873 656c 662c 2063 6f64 652c  rors(self, code,
-0001d910: 2072 6561 736f 6e2c 2075 726c 2c20 6d65   reason, url, me
-0001d920: 7468 6f64 2c20 6865 6164 6572 732c 2062  thod, headers, b
-0001d930: 6f64 792c 2072 6573 706f 6e73 652c 2072  ody, response, r
-0001d940: 6571 7565 7374 4865 6164 6572 732c 2072  equestHeaders, r
-0001d950: 6571 7565 7374 426f 6479 293a 0a20 2020  equestBody):.   
-0001d960: 2020 2020 2069 6620 636f 6465 203d 3d20       if code == 
-0001d970: 3532 303a 0a20 2020 2020 2020 2020 2020  520:.           
-0001d980: 2072 6169 7365 2045 7863 6861 6e67 654e   raise ExchangeN
-0001d990: 6f74 4176 6169 6c61 626c 6528 7365 6c66  otAvailable(self
-0001d9a0: 2e69 6420 2b20 2720 2720 2b20 7374 7228  .id + ' ' + str(
-0001d9b0: 636f 6465 2920 2b20 2720 2720 2b20 7265  code) + ' ' + re
-0001d9c0: 6173 6f6e 290a 2020 2020 2020 2020 2320  ason).        # 
-0001d9d0: 746f 646f 3a20 7265 7772 6974 6520 7365  todo: rewrite se
-0001d9e0: 6c66 2066 6f72 2022 6272 6f61 6422 2065  lf for "broad" e
-0001d9f0: 7863 6570 7469 6f6e 7320 6d61 7463 6869  xceptions matchi
-0001da00: 6e67 0a20 2020 2020 2020 2069 6620 626f  ng.        if bo
-0001da10: 6479 2e66 696e 6428 2749 6e76 616c 6964  dy.find('Invalid
-0001da20: 206f 7264 6572 2729 203e 3d20 303a 0a20   order') >= 0:. 
-0001da30: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0001da40: 2049 6e76 616c 6964 4f72 6465 7228 7365   InvalidOrder(se
-0001da50: 6c66 2e69 6420 2b20 2720 2720 2b20 626f  lf.id + ' ' + bo
-0001da60: 6479 290a 2020 2020 2020 2020 6966 2062  dy).        if b
-0001da70: 6f64 792e 6669 6e64 2827 496e 7661 6c69  ody.find('Invali
-0001da80: 6420 6e6f 6e63 6527 2920 3e3d 2030 3a0a  d nonce') >= 0:.
-0001da90: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0001daa0: 6520 496e 7661 6c69 644e 6f6e 6365 2873  e InvalidNonce(s
-0001dab0: 656c 662e 6964 202b 2027 2027 202b 2062  elf.id + ' ' + b
-0001dac0: 6f64 7929 0a20 2020 2020 2020 2069 6620  ody).        if 
-0001dad0: 626f 6479 2e66 696e 6428 2749 6e73 7566  body.find('Insuf
-0001dae0: 6669 6369 656e 7420 6675 6e64 7327 2920  ficient funds') 
-0001daf0: 3e3d 2030 3a0a 2020 2020 2020 2020 2020  >= 0:.          
-0001db00: 2020 7261 6973 6520 496e 7375 6666 6963    raise Insuffic
-0001db10: 6965 6e74 4675 6e64 7328 7365 6c66 2e69  ientFunds(self.i
-0001db20: 6420 2b20 2720 2720 2b20 626f 6479 290a  d + ' ' + body).
-0001db30: 2020 2020 2020 2020 6966 2062 6f64 792e          if body.
-0001db40: 6669 6e64 2827 4361 6e63 656c 2070 656e  find('Cancel pen
-0001db50: 6469 6e67 2729 203e 3d20 303a 0a20 2020  ding') >= 0:.   
-0001db60: 2020 2020 2020 2020 2072 6169 7365 2043           raise C
-0001db70: 616e 6365 6c50 656e 6469 6e67 2873 656c  ancelPending(sel
-0001db80: 662e 6964 202b 2027 2027 202b 2062 6f64  f.id + ' ' + bod
-0001db90: 7929 0a20 2020 2020 2020 2069 6620 626f  y).        if bo
-0001dba0: 6479 2e66 696e 6428 2749 6e76 616c 6964  dy.find('Invalid
-0001dbb0: 2061 7267 756d 656e 7473 3a76 6f6c 756d   arguments:volum
-0001dbc0: 6527 2920 3e3d 2030 3a0a 2020 2020 2020  e') >= 0:.      
-0001dbd0: 2020 2020 2020 7261 6973 6520 496e 7661        raise Inva
-0001dbe0: 6c69 644f 7264 6572 2873 656c 662e 6964  lidOrder(self.id
-0001dbf0: 202b 2027 2027 202b 2062 6f64 7929 0a20   + ' ' + body). 
-0001dc00: 2020 2020 2020 2069 6620 626f 6479 2e66         if body.f
-0001dc10: 696e 6428 2752 6174 6520 6c69 6d69 7420  ind('Rate limit 
-0001dc20: 6578 6365 6564 6564 2729 203e 3d20 303a  exceeded') >= 0:
-0001dc30: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0001dc40: 7365 2052 6174 654c 696d 6974 4578 6365  se RateLimitExce
-0001dc50: 6564 6564 2873 656c 662e 6964 202b 2027  eded(self.id + '
-0001dc60: 2027 202b 2062 6f64 7929 0a20 2020 2020   ' + body).     
-0001dc70: 2020 2069 6620 7265 7370 6f6e 7365 2069     if response i
-0001dc80: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0001dc90: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-0001dca0: 2020 2020 2020 2020 6966 2062 6f64 795b          if body[
-0001dcb0: 305d 203d 3d20 277b 273a 0a20 2020 2020  0] == '{':.     
-0001dcc0: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
-0001dcd0: 696e 7374 616e 6365 2872 6573 706f 6e73  instance(respons
-0001dce0: 652c 2073 7472 293a 0a20 2020 2020 2020  e, str):.       
-0001dcf0: 2020 2020 2020 2020 2069 6620 2765 7272           if 'err
-0001dd00: 6f72 2720 696e 2072 6573 706f 6e73 653a  or' in response:
-0001dd10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001dd20: 2020 2020 206e 756d 4572 726f 7273 203d       numErrors =
-0001dd30: 206c 656e 2872 6573 706f 6e73 655b 2765   len(response['e
-0001dd40: 7272 6f72 275d 290a 2020 2020 2020 2020  rror']).        
-0001dd50: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0001dd60: 756d 4572 726f 7273 3a0a 2020 2020 2020  umErrors:.      
-0001dd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dd80: 2020 6d65 7373 6167 6520 3d20 7365 6c66    message = self
-0001dd90: 2e69 6420 2b20 2720 2720 2b20 626f 6479  .id + ' ' + body
-0001dda0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ddb0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-0001ddc0: 6e20 7261 6e67 6528 302c 206c 656e 2872  n range(0, len(r
-0001ddd0: 6573 706f 6e73 655b 2765 7272 6f72 275d  esponse['error']
-0001dde0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-0001ddf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001de00: 6572 726f 7220 3d20 7265 7370 6f6e 7365  error = response
-0001de10: 5b27 6572 726f 7227 5d5b 695d 0a20 2020  ['error'][i].   
-0001de20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001de30: 2020 2020 2020 2020 2073 656c 662e 7468           self.th
-0001de40: 726f 775f 6578 6163 746c 795f 6d61 7463  row_exactly_matc
-0001de50: 6865 645f 6578 6365 7074 696f 6e28 7365  hed_exception(se
-0001de60: 6c66 2e65 7863 6570 7469 6f6e 732c 2065  lf.exceptions, e
-0001de70: 7272 6f72 2c20 6d65 7373 6167 6529 0a20  rror, message). 
-0001de80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001de90: 2020 2020 2020 2072 6169 7365 2045 7863         raise Exc
-0001dea0: 6861 6e67 6545 7272 6f72 286d 6573 7361  hangeError(messa
-0001deb0: 6765 290a 2020 2020 2020 2020 7265 7475  ge).        retu
-0001dec0: 726e 204e 6f6e 650a                      rn None.
+0001bba0: 5d20 5b73 796d 626f 6c73 5d3a 206e 6f74  ] [symbols]: not
+0001bbb0: 2075 7365 6420 6279 206b 7261 6b65 6e20   used by kraken 
+0001bbc0: 6665 7463 6850 6f73 6974 696f 6e73 2829  fetchPositions()
+0001bbd0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0001bbe0: 6469 6374 205b 7061 7261 6d73 5d3a 2065  dict [params]: e
+0001bbf0: 7874 7261 2070 6172 616d 6574 6572 7320  xtra parameters 
+0001bc00: 7370 6563 6966 6963 2074 6f20 7468 6520  specific to the 
+0001bc10: 6578 6368 616e 6765 2041 5049 2065 6e64  exchange API end
+0001bc20: 706f 696e 740a 2020 2020 2020 2020 3a72  point.        :r
+0001bc30: 6574 7572 6e73 2064 6963 745b 5d3a 2061  eturns dict[]: a
+0001bc40: 206c 6973 7420 6f66 2060 706f 7369 7469   list of `positi
+0001bc50: 6f6e 2073 7472 7563 7475 7265 203c 6874  on structure <ht
+0001bc60: 7470 733a 2f2f 646f 6373 2e63 6378 742e  tps://docs.ccxt.
+0001bc70: 636f 6d2f 232f 3f69 643d 706f 7369 7469  com/#/?id=positi
+0001bc80: 6f6e 2d73 7472 7563 7475 7265 3e60 0a20  on-structure>`. 
+0001bc90: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0001bca0: 2020 2061 7761 6974 2073 656c 662e 6c6f     await self.lo
+0001bcb0: 6164 5f6d 6172 6b65 7473 2829 0a20 2020  ad_markets().   
+0001bcc0: 2020 2020 2072 6571 7565 7374 203d 207b       request = {
+0001bcd0: 0a20 2020 2020 2020 2020 2020 2023 2027  .            # '
+0001bce0: 7478 6964 273a 2027 636f 6d6d 6120 6465  txid': 'comma de
+0001bcf0: 6c69 6d69 7465 6420 6c69 7374 206f 6620  limited list of 
+0001bd00: 7472 616e 7361 6374 696f 6e20 6964 7320  transaction ids 
+0001bd10: 746f 2072 6573 7472 6963 7420 6f75 7470  to restrict outp
+0001bd20: 7574 2074 6f27 2c0a 2020 2020 2020 2020  ut to',.        
+0001bd30: 2020 2020 2764 6f63 616c 6373 273a 2027      'docalcs': '
+0001bd40: 7472 7565 272c 2020 2320 7768 6574 6865  true',  # whethe
+0001bd50: 7220 6f72 206e 6f74 2074 6f20 696e 636c  r or not to incl
+0001bd60: 7564 6520 7072 6f66 6974 2f6c 6f73 7320  ude profit/loss 
+0001bd70: 6361 6c63 756c 6174 696f 6e73 0a20 2020  calculations.   
+0001bd80: 2020 2020 2020 2020 2027 636f 6e73 6f6c           'consol
+0001bd90: 6964 6174 696f 6e27 3a20 276d 6172 6b65  idation': 'marke
+0001bda0: 7427 2c20 2023 2077 6861 7420 746f 2063  t',  # what to c
+0001bdb0: 6f6e 736f 6c69 6461 7465 2074 6865 2070  onsolidate the p
+0001bdc0: 6f73 6974 696f 6e73 2064 6174 6120 6172  ositions data ar
+0001bdd0: 6f75 6e64 2c20 6d61 726b 6574 2077 696c  ound, market wil
+0001bde0: 6c20 636f 6e73 6f6c 6964 6174 6520 706f  l consolidate po
+0001bdf0: 7369 7469 6f6e 7320 6261 7365 6420 6f6e  sitions based on
+0001be00: 206d 6172 6b65 7420 7061 6972 0a20 2020   market pair.   
+0001be10: 2020 2020 207d 0a20 2020 2020 2020 2072       }.        r
+0001be20: 6573 706f 6e73 6520 3d20 6177 6169 7420  esponse = await 
+0001be30: 7365 6c66 2e70 7269 7661 7465 506f 7374  self.privatePost
+0001be40: 4f70 656e 506f 7369 7469 6f6e 7328 7365  OpenPositions(se
+0001be50: 6c66 2e65 7874 656e 6428 7265 7175 6573  lf.extend(reques
+0001be60: 742c 2070 6172 616d 7329 290a 2020 2020  t, params)).    
+0001be70: 2020 2020 230a 2020 2020 2020 2020 2320      #.        # 
+0001be80: 6e6f 2063 6f6e 736f 6c69 6461 7469 6f6e  no consolidation
+0001be90: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
+0001bea0: 2020 2023 2020 2020 207b 0a20 2020 2020     #     {.     
+0001beb0: 2020 2023 2020 2020 2020 2020 2022 6572     #         "er
+0001bec0: 726f 7222 3a20 5b5d 2c0a 2020 2020 2020  ror": [],.      
+0001bed0: 2020 2320 2020 2020 2020 2020 2272 6573    #         "res
+0001bee0: 756c 7422 3a20 7b0a 2020 2020 2020 2020  ult": {.        
+0001bef0: 2320 2020 2020 2020 2020 2020 2020 2754  #             'T
+0001bf00: 4755 464d 592d 464c 4553 4a2d 5659 4958  GUFMY-FLESJ-VYIX
+0001bf10: 334a 273a 207b 0a20 2020 2020 2020 2023  3J': {.        #
+0001bf20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bf30: 2022 6f72 6465 7274 7869 6422 3a20 224f   "ordertxid": "O
+0001bf40: 334c 524e 552d 5a4b 4447 352d 584e 4344  3LRNU-ZKDG5-XNCD
+0001bf50: 4652 222c 0a20 2020 2020 2020 2023 2020  FR",.        #  
+0001bf60: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0001bf70: 706f 7373 7461 7475 7322 3a20 226f 7065  posstatus": "ope
+0001bf80: 6e22 2c0a 2020 2020 2020 2020 2320 2020  n",.        #   
+0001bf90: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+0001bfa0: 6169 7222 3a20 2245 5448 5553 4454 222c  air": "ETHUSDT",
+0001bfb0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0001bfc0: 2020 2020 2020 2020 2020 2022 7469 6d65             "time
+0001bfd0: 223a 2020 3136 3131 3535 3732 3331 2e34  ":  1611557231.4
+0001bfe0: 3538 342c 0a20 2020 2020 2020 2023 2020  584,.        #  
+0001bff0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0001c000: 7479 7065 223a 2022 6275 7922 2c0a 2020  type": "buy",.  
+0001c010: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0001c020: 2020 2020 2020 2020 226f 7264 6572 7479          "orderty
+0001c030: 7065 223a 2022 6d61 726b 6574 222c 0a20  pe": "market",. 
+0001c040: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0001c050: 2020 2020 2020 2020 2022 636f 7374 223a           "cost":
+0001c060: 2022 3238 2e34 3938 3030 222c 0a20 2020   "28.49800",.   
+0001c070: 2020 2020 2023 2020 2020 2020 2020 2020       #          
+0001c080: 2020 2020 2020 2022 6665 6522 3a20 2230         "fee": "0
+0001c090: 2e30 3739 3739 222c 0a20 2020 2020 2020  .07979",.       
+0001c0a0: 2023 2020 2020 2020 2020 2020 2020 2020   #              
+0001c0b0: 2020 2022 766f 6c22 3a20 2230 2e30 3230     "vol": "0.020
+0001c0c0: 3030 3030 3022 2c0a 2020 2020 2020 2020  00000",.        
+0001c0d0: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+0001c0e0: 2020 2276 6f6c 5f63 6c6f 7365 6422 3a20    "vol_closed": 
+0001c0f0: 2230 2e30 3030 3030 3030 3022 2c0a 2020  "0.00000000",.  
+0001c100: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0001c110: 2020 2020 2020 2020 226d 6172 6769 6e22          "margin"
+0001c120: 3a20 2231 342e 3234 3930 3022 2c0a 2020  : "14.24900",.  
+0001c130: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0001c140: 2020 2020 2020 2020 2274 6572 6d73 223a          "terms":
+0001c150: 2022 302e 3032 3030 2520 7065 7220 3420   "0.0200% per 4 
+0001c160: 686f 7572 7322 2c0a 2020 2020 2020 2020  hours",.        
+0001c170: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+0001c180: 2020 2272 6f6c 6c6f 7665 7274 6d22 3a20    "rollovertm": 
+0001c190: 2231 3631 3135 3731 3633 3122 2c0a 2020  "1611571631",.  
+0001c1a0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0001c1b0: 2020 2020 2020 2020 226d 6973 6322 3a20          "misc": 
+0001c1c0: 2222 2c0a 2020 2020 2020 2020 2320 2020  "",.        #   
+0001c1d0: 2020 2020 2020 2020 2020 2020 2020 226f                "o
+0001c1e0: 666c 6167 7322 3a20 2222 0a20 2020 2020  flags": "".     
+0001c1f0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0001c200: 207d 0a20 2020 2020 2020 2023 2020 2020   }.        #    
+0001c210: 2020 2020 207d 0a20 2020 2020 2020 2023       }.        #
+0001c220: 2020 2020 207d 0a20 2020 2020 2020 2023       }.        #
+0001c230: 0a20 2020 2020 2020 2023 2063 6f6e 736f  .        # conso
+0001c240: 6c69 6461 7469 6f6e 2062 7920 6d61 726b  lidation by mark
+0001c250: 6574 0a20 2020 2020 2020 2023 0a20 2020  et.        #.   
+0001c260: 2020 2020 2023 2020 2020 207b 0a20 2020       #     {.   
+0001c270: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
+0001c280: 6572 726f 7222 3a20 5b5d 2c0a 2020 2020  error": [],.    
+0001c290: 2020 2020 2320 2020 2020 2020 2020 2272      #         "r
+0001c2a0: 6573 756c 7422 3a20 5b0a 2020 2020 2020  esult": [.      
+0001c2b0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+0001c2c0: 7b0a 2020 2020 2020 2020 2320 2020 2020  {.        #     
+0001c2d0: 2020 2020 2020 2020 2020 2020 2270 6169              "pai
+0001c2e0: 7222 3a20 2245 5448 5553 4454 222c 0a20  r": "ETHUSDT",. 
+0001c2f0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0001c300: 2020 2020 2020 2020 2022 706f 7369 7469           "positi
+0001c310: 6f6e 7322 3a20 2231 222c 0a20 2020 2020  ons": "1",.     
+0001c320: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0001c330: 2020 2020 2022 7479 7065 223a 2022 6275       "type": "bu
+0001c340: 7922 2c0a 2020 2020 2020 2020 2320 2020  y",.        #   
+0001c350: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+0001c360: 6576 6572 6167 6522 3a20 2232 2e30 3030  everage": "2.000
+0001c370: 3030 222c 0a20 2020 2020 2020 2023 2020  00",.        #  
+0001c380: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0001c390: 636f 7374 223a 2022 3238 2e34 3938 3030  cost": "28.49800
+0001c3a0: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
+0001c3b0: 2020 2020 2020 2020 2020 2020 2022 6665               "fe
+0001c3c0: 6522 3a20 2230 2e30 3739 3739 222c 0a20  e": "0.07979",. 
+0001c3d0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0001c3e0: 2020 2020 2020 2020 2022 766f 6c22 3a20           "vol": 
+0001c3f0: 2230 2e30 3230 3030 3030 3022 2c0a 2020  "0.02000000",.  
+0001c400: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0001c410: 2020 2020 2020 2020 2276 6f6c 5f63 6c6f          "vol_clo
+0001c420: 7365 6422 3a20 2230 2e30 3030 3030 3030  sed": "0.0000000
+0001c430: 3022 2c0a 2020 2020 2020 2020 2320 2020  0",.        #   
+0001c440: 2020 2020 2020 2020 2020 2020 2020 226d                "m
+0001c450: 6172 6769 6e22 3a20 2231 342e 3234 3930  argin": "14.2490
+0001c460: 3022 0a20 2020 2020 2020 2023 2020 2020  0".        #    
+0001c470: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+0001c480: 2020 2023 2020 2020 2020 2020 205d 0a20     #         ]. 
+0001c490: 2020 2020 2020 2023 2020 2020 207d 0a20         #     }. 
+0001c4a0: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
+0001c4b0: 2073 796d 626f 6c73 203d 2073 656c 662e   symbols = self.
+0001c4c0: 6d61 726b 6574 5f73 796d 626f 6c73 2873  market_symbols(s
+0001c4d0: 796d 626f 6c73 290a 2020 2020 2020 2020  ymbols).        
+0001c4e0: 7265 7375 6c74 203d 2073 656c 662e 7361  result = self.sa
+0001c4f0: 6665 5f6c 6973 7428 7265 7370 6f6e 7365  fe_list(response
+0001c500: 2c20 2772 6573 756c 7427 290a 2020 2020  , 'result').    
+0001c510: 2020 2020 7265 7375 6c74 7320 3d20 7365      results = se
+0001c520: 6c66 2e70 6172 7365 5f70 6f73 6974 696f  lf.parse_positio
+0001c530: 6e73 2872 6573 756c 742c 2073 796d 626f  ns(result, symbo
+0001c540: 6c73 290a 2020 2020 2020 2020 7265 7475  ls).        retu
+0001c550: 726e 2073 656c 662e 6669 6c74 6572 5f62  rn self.filter_b
+0001c560: 795f 6172 7261 795f 706f 7369 7469 6f6e  y_array_position
+0001c570: 7328 7265 7375 6c74 732c 2027 7379 6d62  s(results, 'symb
+0001c580: 6f6c 272c 2073 796d 626f 6c73 2c20 4661  ol', symbols, Fa
+0001c590: 6c73 6529 0a0a 2020 2020 6465 6620 7061  lse)..    def pa
+0001c5a0: 7273 655f 706f 7369 7469 6f6e 2873 656c  rse_position(sel
+0001c5b0: 662c 2070 6f73 6974 696f 6e2c 206d 6172  f, position, mar
+0001c5c0: 6b65 743a 204d 6172 6b65 7420 3d20 4e6f  ket: Market = No
+0001c5d0: 6e65 293a 0a20 2020 2020 2020 2023 0a20  ne):.        #. 
+0001c5e0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0001c5f0: 2020 2020 207b 0a20 2020 2020 2020 2023       {.        #
+0001c600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c610: 2022 7061 6972 223a 2022 4554 4855 5344   "pair": "ETHUSD
+0001c620: 5422 2c0a 2020 2020 2020 2020 2320 2020  T",.        #   
+0001c630: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+0001c640: 6f73 6974 696f 6e73 223a 2022 3122 2c0a  ositions": "1",.
+0001c650: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0001c660: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
+0001c670: 3a20 2262 7579 222c 0a20 2020 2020 2020  : "buy",.       
+0001c680: 2023 2020 2020 2020 2020 2020 2020 2020   #              
+0001c690: 2020 2022 6c65 7665 7261 6765 223a 2022     "leverage": "
+0001c6a0: 322e 3030 3030 3022 2c0a 2020 2020 2020  2.00000",.      
+0001c6b0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+0001c6c0: 2020 2020 2263 6f73 7422 3a20 2232 382e      "cost": "28.
+0001c6d0: 3439 3830 3022 2c0a 2020 2020 2020 2020  49800",.        
+0001c6e0: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+0001c6f0: 2020 2266 6565 223a 2022 302e 3037 3937    "fee": "0.0797
+0001c700: 3922 2c0a 2020 2020 2020 2020 2320 2020  9",.        #   
+0001c710: 2020 2020 2020 2020 2020 2020 2020 2276                "v
+0001c720: 6f6c 223a 2022 302e 3032 3030 3030 3030  ol": "0.02000000
+0001c730: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
+0001c740: 2020 2020 2020 2020 2020 2020 2022 766f               "vo
+0001c750: 6c5f 636c 6f73 6564 223a 2022 302e 3030  l_closed": "0.00
+0001c760: 3030 3030 3030 222c 0a20 2020 2020 2020  000000",.       
+0001c770: 2023 2020 2020 2020 2020 2020 2020 2020   #              
+0001c780: 2020 2022 6d61 7267 696e 223a 2022 3134     "margin": "14
+0001c790: 2e32 3439 3030 220a 2020 2020 2020 2020  .24900".        
+0001c7a0: 2320 2020 2020 2020 2020 2020 2020 7d0a  #             }.
+0001c7b0: 2020 2020 2020 2020 230a 2020 2020 2020          #.      
+0001c7c0: 2020 6d61 726b 6574 4964 203d 2073 656c    marketId = sel
+0001c7d0: 662e 7361 6665 5f73 7472 696e 6728 706f  f.safe_string(po
+0001c7e0: 7369 7469 6f6e 2c20 2770 6169 7227 290a  sition, 'pair').
+0001c7f0: 2020 2020 2020 2020 7261 7753 6964 6520          rawSide 
+0001c800: 3d20 7365 6c66 2e73 6166 655f 7374 7269  = self.safe_stri
+0001c810: 6e67 2870 6f73 6974 696f 6e2c 2027 7479  ng(position, 'ty
+0001c820: 7065 2729 0a20 2020 2020 2020 2073 6964  pe').        sid
+0001c830: 6520 3d20 276c 6f6e 6727 2069 6620 2872  e = 'long' if (r
+0001c840: 6177 5369 6465 203d 3d20 2762 7579 2729  awSide == 'buy')
+0001c850: 2065 6c73 6520 2773 686f 7274 270a 2020   else 'short'.  
+0001c860: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0001c870: 662e 7361 6665 5f70 6f73 6974 696f 6e28  f.safe_position(
+0001c880: 7b0a 2020 2020 2020 2020 2020 2020 2769  {.            'i
+0001c890: 6e66 6f27 3a20 706f 7369 7469 6f6e 2c0a  nfo': position,.
+0001c8a0: 2020 2020 2020 2020 2020 2020 2769 6427              'id'
+0001c8b0: 3a20 4e6f 6e65 2c0a 2020 2020 2020 2020  : None,.        
+0001c8c0: 2020 2020 2773 796d 626f 6c27 3a20 7365      'symbol': se
+0001c8d0: 6c66 2e73 6166 655f 7379 6d62 6f6c 286d  lf.safe_symbol(m
+0001c8e0: 6172 6b65 7449 642c 206d 6172 6b65 7429  arketId, market)
+0001c8f0: 2c0a 2020 2020 2020 2020 2020 2020 276e  ,.            'n
+0001c900: 6f74 696f 6e61 6c27 3a20 4e6f 6e65 2c0a  otional': None,.
+0001c910: 2020 2020 2020 2020 2020 2020 276d 6172              'mar
+0001c920: 6769 6e4d 6f64 6527 3a20 4e6f 6e65 2c0a  ginMode': None,.
+0001c930: 2020 2020 2020 2020 2020 2020 276c 6971              'liq
+0001c940: 7569 6461 7469 6f6e 5072 6963 6527 3a20  uidationPrice': 
+0001c950: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+0001c960: 2020 2765 6e74 7279 5072 6963 6527 3a20    'entryPrice': 
+0001c970: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+0001c980: 2020 2775 6e72 6561 6c69 7a65 6450 6e6c    'unrealizedPnl
+0001c990: 273a 2073 656c 662e 7361 6665 5f6e 756d  ': self.safe_num
+0001c9a0: 6265 7228 706f 7369 7469 6f6e 2c20 276e  ber(position, 'n
+0001c9b0: 6574 2729 2c0a 2020 2020 2020 2020 2020  et'),.          
+0001c9c0: 2020 2772 6561 6c69 7a65 6450 6e6c 273a    'realizedPnl':
+0001c9d0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+0001c9e0: 2020 2027 7065 7263 656e 7461 6765 273a     'percentage':
+0001c9f0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+0001ca00: 2020 2027 636f 6e74 7261 6374 7327 3a20     'contracts': 
+0001ca10: 7365 6c66 2e73 6166 655f 6e75 6d62 6572  self.safe_number
+0001ca20: 2870 6f73 6974 696f 6e2c 2027 766f 6c27  (position, 'vol'
+0001ca30: 292c 0a20 2020 2020 2020 2020 2020 2027  ),.            '
+0001ca40: 636f 6e74 7261 6374 5369 7a65 273a 204e  contractSize': N
+0001ca50: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+0001ca60: 2027 6d61 726b 5072 6963 6527 3a20 4e6f   'markPrice': No
+0001ca70: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+0001ca80: 276c 6173 7450 7269 6365 273a 204e 6f6e  'lastPrice': Non
+0001ca90: 652c 0a20 2020 2020 2020 2020 2020 2027  e,.            '
+0001caa0: 7369 6465 273a 2073 6964 652c 0a20 2020  side': side,.   
+0001cab0: 2020 2020 2020 2020 2027 6865 6467 6564           'hedged
+0001cac0: 273a 204e 6f6e 652c 0a20 2020 2020 2020  ': None,.       
+0001cad0: 2020 2020 2027 7469 6d65 7374 616d 7027       'timestamp'
+0001cae0: 3a20 4e6f 6e65 2c0a 2020 2020 2020 2020  : None,.        
+0001caf0: 2020 2020 2764 6174 6574 696d 6527 3a20      'datetime': 
+0001cb00: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+0001cb10: 2020 276c 6173 7455 7064 6174 6554 696d    'lastUpdateTim
+0001cb20: 6573 7461 6d70 273a 204e 6f6e 652c 0a20  estamp': None,. 
+0001cb30: 2020 2020 2020 2020 2020 2027 6d61 696e             'main
+0001cb40: 7465 6e61 6e63 654d 6172 6769 6e27 3a20  tenanceMargin': 
+0001cb50: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+0001cb60: 2020 276d 6169 6e74 656e 616e 6365 4d61    'maintenanceMa
+0001cb70: 7267 696e 5065 7263 656e 7461 6765 273a  rginPercentage':
+0001cb80: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+0001cb90: 2020 2027 636f 6c6c 6174 6572 616c 273a     'collateral':
+0001cba0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+0001cbb0: 2020 2027 696e 6974 6961 6c4d 6172 6769     'initialMargi
+0001cbc0: 6e27 3a20 7365 6c66 2e73 6166 655f 6e75  n': self.safe_nu
+0001cbd0: 6d62 6572 2870 6f73 6974 696f 6e2c 2027  mber(position, '
+0001cbe0: 6d61 7267 696e 2729 2c0a 2020 2020 2020  margin'),.      
+0001cbf0: 2020 2020 2020 2769 6e69 7469 616c 4d61        'initialMa
+0001cc00: 7267 696e 5065 7263 656e 7461 6765 273a  rginPercentage':
+0001cc10: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+0001cc20: 2020 2027 6c65 7665 7261 6765 273a 2073     'leverage': s
+0001cc30: 656c 662e 7361 6665 5f6e 756d 6265 7228  elf.safe_number(
+0001cc40: 706f 7369 7469 6f6e 2c20 276c 6576 6572  position, 'lever
+0001cc50: 6167 6527 292c 0a20 2020 2020 2020 2020  age'),.         
+0001cc60: 2020 2027 6d61 7267 696e 5261 7469 6f27     'marginRatio'
+0001cc70: 3a20 4e6f 6e65 2c0a 2020 2020 2020 2020  : None,.        
+0001cc80: 2020 2020 2773 746f 704c 6f73 7350 7269      'stopLossPri
+0001cc90: 6365 273a 204e 6f6e 652c 0a20 2020 2020  ce': None,.     
+0001cca0: 2020 2020 2020 2027 7461 6b65 5072 6f66         'takeProf
+0001ccb0: 6974 5072 6963 6527 3a20 4e6f 6e65 2c0a  itPrice': None,.
+0001ccc0: 2020 2020 2020 2020 7d29 0a0a 2020 2020          })..    
+0001ccd0: 6465 6620 7061 7273 655f 6163 636f 756e  def parse_accoun
+0001cce0: 745f 7479 7065 2873 656c 662c 2061 6363  t_type(self, acc
+0001ccf0: 6f75 6e74 293a 0a20 2020 2020 2020 2061  ount):.        a
+0001cd00: 6363 6f75 6e74 4279 5479 7065 203d 207b  ccountByType = {
+0001cd10: 0a20 2020 2020 2020 2020 2020 2027 7370  .            'sp
+0001cd20: 6f74 273a 2027 5370 6f74 2057 616c 6c65  ot': 'Spot Walle
+0001cd30: 7427 2c0a 2020 2020 2020 2020 2020 2020  t',.            
+0001cd40: 2773 7761 7027 3a20 2746 7574 7572 6573  'swap': 'Futures
+0001cd50: 2057 616c 6c65 7427 2c0a 2020 2020 2020   Wallet',.      
+0001cd60: 2020 2020 2020 2766 7574 7572 6527 3a20        'future': 
+0001cd70: 2746 7574 7572 6573 2057 616c 6c65 7427  'Futures Wallet'
+0001cd80: 2c0a 2020 2020 2020 2020 7d0a 2020 2020  ,.        }.    
+0001cd90: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0001cda0: 7361 6665 5f73 7472 696e 6728 6163 636f  safe_string(acco
+0001cdb0: 756e 7442 7954 7970 652c 2061 6363 6f75  untByType, accou
+0001cdc0: 6e74 2c20 6163 636f 756e 7429 0a0a 2020  nt, account)..  
+0001cdd0: 2020 6173 796e 6320 6465 6620 7472 616e    async def tran
+0001cde0: 7366 6572 5f6f 7574 2873 656c 662c 2063  sfer_out(self, c
+0001cdf0: 6f64 653a 2073 7472 2c20 616d 6f75 6e74  ode: str, amount
+0001ce00: 2c20 7061 7261 6d73 3d7b 7d29 3a0a 2020  , params={}):.  
+0001ce10: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0001ce20: 2020 7472 616e 7366 6572 2066 726f 6d20    transfer from 
+0001ce30: 7370 6f74 2077 616c 6c65 7420 746f 2066  spot wallet to f
+0001ce40: 7574 7572 6573 2077 616c 6c65 740a 2020  utures wallet.  
+0001ce50: 2020 2020 2020 3a73 6565 3a20 6874 7470        :see: http
+0001ce60: 733a 2f2f 646f 6373 2e6b 7261 6b65 6e2e  s://docs.kraken.
+0001ce70: 636f 6d2f 7265 7374 2f23 7461 672f 5573  com/rest/#tag/Us
+0001ce80: 6572 2d46 756e 6469 6e67 2f6f 7065 7261  er-Funding/opera
+0001ce90: 7469 6f6e 2f77 616c 6c65 7454 7261 6e73  tion/walletTrans
+0001cea0: 6665 720a 2020 2020 2020 2020 3a70 6172  fer.        :par
+0001ceb0: 616d 2073 7472 2063 6f64 653a 2055 6e69  am str code: Uni
+0001cec0: 6669 6564 2063 7572 7265 6e63 7920 636f  fied currency co
+0001ced0: 6465 0a20 2020 2020 2020 203a 7061 7261  de.        :para
+0001cee0: 6d20 666c 6f61 7420 616d 6f75 6e74 3a20  m float amount: 
+0001cef0: 5369 7a65 206f 6620 7468 6520 7472 616e  Size of the tran
+0001cf00: 7366 6572 0a20 2020 2020 2020 203a 7061  sfer.        :pa
+0001cf10: 7261 6d20 6469 6374 205b 7061 7261 6d73  ram dict [params
+0001cf20: 5d3a 2045 7863 6861 6e67 6520 7370 6563  ]: Exchange spec
+0001cf30: 6966 6963 2070 6172 616d 6574 6572 730a  ific parameters.
+0001cf40: 2020 2020 2020 2020 3a72 6574 7572 6e73          :returns
+0001cf50: 3a20 6120 6074 7261 6e73 6665 7220 7374  : a `transfer st
+0001cf60: 7275 6374 7572 6520 3c68 7474 7073 3a2f  ructure <https:/
+0001cf70: 2f64 6f63 732e 6363 7874 2e63 6f6d 2f23  /docs.ccxt.com/#
+0001cf80: 2f3f 6964 3d74 7261 6e73 6665 722d 7374  /?id=transfer-st
+0001cf90: 7275 6374 7572 653e 600a 2020 2020 2020  ructure>`.      
+0001cfa0: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+0001cfb0: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
+0001cfc0: 7472 616e 7366 6572 2863 6f64 652c 2061  transfer(code, a
+0001cfd0: 6d6f 756e 742c 2027 7370 6f74 272c 2027  mount, 'spot', '
+0001cfe0: 7377 6170 272c 2070 6172 616d 7329 0a0a  swap', params)..
+0001cff0: 2020 2020 6173 796e 6320 6465 6620 7472      async def tr
+0001d000: 616e 7366 6572 2873 656c 662c 2063 6f64  ansfer(self, cod
+0001d010: 653a 2073 7472 2c20 616d 6f75 6e74 3a20  e: str, amount: 
+0001d020: 666c 6f61 742c 2066 726f 6d41 6363 6f75  float, fromAccou
+0001d030: 6e74 3a20 7374 722c 2074 6f41 6363 6f75  nt: str, toAccou
+0001d040: 6e74 3a20 7374 722c 2070 6172 616d 733d  nt: str, params=
+0001d050: 7b7d 2920 2d3e 2054 7261 6e73 6665 7245  {}) -> TransferE
+0001d060: 6e74 7279 3a0a 2020 2020 2020 2020 2222  ntry:.        ""
+0001d070: 220a 2020 2020 2020 2020 3a73 6565 3a20  ".        :see: 
+0001d080: 6874 7470 733a 2f2f 646f 6373 2e6b 7261  https://docs.kra
+0001d090: 6b65 6e2e 636f 6d2f 7265 7374 2f23 7461  ken.com/rest/#ta
+0001d0a0: 672f 5573 6572 2d46 756e 6469 6e67 2f6f  g/User-Funding/o
+0001d0b0: 7065 7261 7469 6f6e 2f77 616c 6c65 7454  peration/walletT
+0001d0c0: 7261 6e73 6665 720a 2020 2020 2020 2020  ransfer.        
+0001d0d0: 7472 616e 7366 6572 7320 6375 7272 656e  transfers curren
+0001d0e0: 6369 6573 2062 6574 7765 656e 2073 7562  cies between sub
+0001d0f0: 2d61 6363 6f75 6e74 7328 6f6e 6c79 2073  -accounts(only s
+0001d100: 706f 742d 3e73 7761 7020 6469 7265 6374  pot->swap direct
+0001d110: 696f 6e20 6973 2073 7570 706f 7274 6564  ion is supported
+0001d120: 290a 2020 2020 2020 2020 3a70 6172 616d  ).        :param
+0001d130: 2073 7472 2063 6f64 653a 2055 6e69 6669   str code: Unifi
+0001d140: 6564 2063 7572 7265 6e63 7920 636f 6465  ed currency code
+0001d150: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0001d160: 666c 6f61 7420 616d 6f75 6e74 3a20 5369  float amount: Si
+0001d170: 7a65 206f 6620 7468 6520 7472 616e 7366  ze of the transf
+0001d180: 6572 0a20 2020 2020 2020 203a 7061 7261  er.        :para
+0001d190: 6d20 7374 7220 6672 6f6d 4163 636f 756e  m str fromAccoun
+0001d1a0: 743a 2027 7370 6f74 2720 6f72 2027 5370  t: 'spot' or 'Sp
+0001d1b0: 6f74 2057 616c 6c65 7427 0a20 2020 2020  ot Wallet'.     
+0001d1c0: 2020 203a 7061 7261 6d20 7374 7220 746f     :param str to
+0001d1d0: 4163 636f 756e 743a 2027 7377 6170 2720  Account: 'swap' 
+0001d1e0: 6f72 2027 4675 7475 7265 7320 5761 6c6c  or 'Futures Wall
+0001d1f0: 6574 270a 2020 2020 2020 2020 3a70 6172  et'.        :par
+0001d200: 616d 2064 6963 7420 5b70 6172 616d 735d  am dict [params]
+0001d210: 3a20 4578 6368 616e 6765 2073 7065 6369  : Exchange speci
+0001d220: 6669 6320 7061 7261 6d65 7465 7273 0a20  fic parameters. 
+0001d230: 2020 2020 2020 203a 7265 7475 726e 733a         :returns:
+0001d240: 2061 2060 7472 616e 7366 6572 2073 7472   a `transfer str
+0001d250: 7563 7475 7265 203c 6874 7470 733a 2f2f  ucture <https://
+0001d260: 646f 6373 2e63 6378 742e 636f 6d2f 232f  docs.ccxt.com/#/
+0001d270: 3f69 643d 7472 616e 7366 6572 2d73 7472  ?id=transfer-str
+0001d280: 7563 7475 7265 3e60 0a20 2020 2020 2020  ucture>`.       
+0001d290: 2022 2222 0a20 2020 2020 2020 2061 7761   """.        awa
+0001d2a0: 6974 2073 656c 662e 6c6f 6164 5f6d 6172  it self.load_mar
+0001d2b0: 6b65 7473 2829 0a20 2020 2020 2020 2063  kets().        c
+0001d2c0: 7572 7265 6e63 7920 3d20 7365 6c66 2e63  urrency = self.c
+0001d2d0: 7572 7265 6e63 7928 636f 6465 290a 2020  urrency(code).  
+0001d2e0: 2020 2020 2020 6672 6f6d 4163 636f 756e        fromAccoun
+0001d2f0: 7420 3d20 7365 6c66 2e70 6172 7365 5f61  t = self.parse_a
+0001d300: 6363 6f75 6e74 5f74 7970 6528 6672 6f6d  ccount_type(from
+0001d310: 4163 636f 756e 7429 0a20 2020 2020 2020  Account).       
+0001d320: 2074 6f41 6363 6f75 6e74 203d 2073 656c   toAccount = sel
+0001d330: 662e 7061 7273 655f 6163 636f 756e 745f  f.parse_account_
+0001d340: 7479 7065 2874 6f41 6363 6f75 6e74 290a  type(toAccount).
+0001d350: 2020 2020 2020 2020 7265 7175 6573 7420          request 
+0001d360: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+0001d370: 2761 6d6f 756e 7427 3a20 7365 6c66 2e63  'amount': self.c
+0001d380: 7572 7265 6e63 795f 746f 5f70 7265 6369  urrency_to_preci
+0001d390: 7369 6f6e 2863 6f64 652c 2061 6d6f 756e  sion(code, amoun
+0001d3a0: 7429 2c0a 2020 2020 2020 2020 2020 2020  t),.            
+0001d3b0: 2766 726f 6d27 3a20 6672 6f6d 4163 636f  'from': fromAcco
+0001d3c0: 756e 742c 0a20 2020 2020 2020 2020 2020  unt,.           
+0001d3d0: 2027 746f 273a 2074 6f41 6363 6f75 6e74   'to': toAccount
+0001d3e0: 2c0a 2020 2020 2020 2020 2020 2020 2761  ,.            'a
+0001d3f0: 7373 6574 273a 2063 7572 7265 6e63 795b  sset': currency[
+0001d400: 2769 6427 5d2c 0a20 2020 2020 2020 207d  'id'],.        }
+0001d410: 0a20 2020 2020 2020 2069 6620 6672 6f6d  .        if from
+0001d420: 4163 636f 756e 7420 213d 2027 5370 6f74  Account != 'Spot
+0001d430: 2057 616c 6c65 7427 3a0a 2020 2020 2020   Wallet':.      
+0001d440: 2020 2020 2020 7261 6973 6520 4261 6452        raise BadR
+0001d450: 6571 7565 7374 2873 656c 662e 6964 202b  equest(self.id +
+0001d460: 2027 2074 7261 6e73 6665 7220 6361 6e6e   ' transfer cann
+0001d470: 6f74 2074 7261 6e73 6665 7220 6672 6f6d  ot transfer from
+0001d480: 2027 202b 2066 726f 6d41 6363 6f75 6e74   ' + fromAccount
+0001d490: 202b 2027 2074 6f20 2720 2b20 746f 4163   + ' to ' + toAc
+0001d4a0: 636f 756e 7420 2b20 272e 2055 7365 206b  count + '. Use k
+0001d4b0: 7261 6b65 6e66 7574 7572 6573 2069 6e73  rakenfutures ins
+0001d4c0: 7465 6164 2074 6f20 7472 616e 7366 6572  tead to transfer
+0001d4d0: 2066 726f 6d20 7468 6520 6675 7475 7265   from the future
+0001d4e0: 7320 6163 636f 756e 742e 2729 0a20 2020  s account.').   
+0001d4f0: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+0001d500: 6177 6169 7420 7365 6c66 2e70 7269 7661  await self.priva
+0001d510: 7465 506f 7374 5761 6c6c 6574 5472 616e  tePostWalletTran
+0001d520: 7366 6572 2873 656c 662e 6578 7465 6e64  sfer(self.extend
+0001d530: 2872 6571 7565 7374 2c20 7061 7261 6d73  (request, params
+0001d540: 2929 0a20 2020 2020 2020 2023 0a20 2020  )).        #.   
+0001d550: 2020 2020 2023 2020 207b 0a20 2020 2020       #   {.     
+0001d560: 2020 2023 2020 2020 2020 2022 6572 726f     #       "erro
+0001d570: 7222 3a5b 0a20 2020 2020 2020 2023 2020  r":[.        #  
+0001d580: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+0001d590: 2320 2020 2020 2020 2272 6573 756c 7422  #       "result"
+0001d5a0: 3a7b 0a20 2020 2020 2020 2023 2020 2020  :{.        #    
+0001d5b0: 2020 2020 2020 2272 6566 6964 223a 2242        "refid":"B
+0001d5c0: 4f49 5553 4946 2d4d 3744 4c4d 4e2d 5558  OIUSIF-M7DLMN-UX
+0001d5d0: 5a33 5035 220a 2020 2020 2020 2020 2320  Z3P5".        # 
+0001d5e0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+0001d5f0: 2320 2020 7d0a 2020 2020 2020 2020 230a  #   }.        #.
+0001d600: 2020 2020 2020 2020 7472 616e 7366 6572          transfer
+0001d610: 203d 2073 656c 662e 7061 7273 655f 7472   = self.parse_tr
+0001d620: 616e 7366 6572 2872 6573 706f 6e73 652c  ansfer(response,
+0001d630: 2063 7572 7265 6e63 7929 0a20 2020 2020   currency).     
+0001d640: 2020 2072 6574 7572 6e20 7365 6c66 2e65     return self.e
+0001d650: 7874 656e 6428 7472 616e 7366 6572 2c20  xtend(transfer, 
+0001d660: 7b0a 2020 2020 2020 2020 2020 2020 2761  {.            'a
+0001d670: 6d6f 756e 7427 3a20 616d 6f75 6e74 2c0a  mount': amount,.
+0001d680: 2020 2020 2020 2020 2020 2020 2766 726f              'fro
+0001d690: 6d41 6363 6f75 6e74 273a 2066 726f 6d41  mAccount': fromA
+0001d6a0: 6363 6f75 6e74 2c0a 2020 2020 2020 2020  ccount,.        
+0001d6b0: 2020 2020 2774 6f41 6363 6f75 6e74 273a      'toAccount':
+0001d6c0: 2074 6f41 6363 6f75 6e74 2c0a 2020 2020   toAccount,.    
+0001d6d0: 2020 2020 7d29 0a0a 2020 2020 6465 6620      })..    def 
+0001d6e0: 7061 7273 655f 7472 616e 7366 6572 2873  parse_transfer(s
+0001d6f0: 656c 662c 2074 7261 6e73 6665 722c 2063  elf, transfer, c
+0001d700: 7572 7265 6e63 793a 2043 7572 7265 6e63  urrency: Currenc
+0001d710: 7920 3d20 4e6f 6e65 293a 0a20 2020 2020  y = None):.     
+0001d720: 2020 2023 0a20 2020 2020 2020 2023 2074     #.        # t
+0001d730: 7261 6e73 6665 720a 2020 2020 2020 2020  ransfer.        
+0001d740: 230a 2020 2020 2020 2020 2320 2020 207b  #.        #    {
+0001d750: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0001d760: 2020 2265 7272 6f72 223a 5b0a 2020 2020    "error":[.    
+0001d770: 2020 2020 2320 2020 2020 2020 205d 2c0a      #        ],.
+0001d780: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0001d790: 2022 7265 7375 6c74 223a 7b0a 2020 2020   "result":{.    
+0001d7a0: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+0001d7b0: 2272 6566 6964 223a 2242 4f49 5553 4946  "refid":"BOIUSIF
+0001d7c0: 2d4d 3744 4c4d 4e2d 5558 5a33 5035 220a  -M7DLMN-UXZ3P5".
+0001d7d0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0001d7e0: 207d 0a20 2020 2020 2020 2023 2020 2020   }.        #    
+0001d7f0: 7d0a 2020 2020 2020 2020 230a 2020 2020  }.        #.    
+0001d800: 2020 2020 7265 7375 6c74 203d 2073 656c      result = sel
+0001d810: 662e 7361 6665 5f76 616c 7565 2874 7261  f.safe_value(tra
+0001d820: 6e73 6665 722c 2027 7265 7375 6c74 272c  nsfer, 'result',
+0001d830: 207b 7d29 0a20 2020 2020 2020 2072 6566   {}).        ref
+0001d840: 6964 203d 2073 656c 662e 7361 6665 5f73  id = self.safe_s
+0001d850: 7472 696e 6728 7265 7375 6c74 2c20 2772  tring(result, 'r
+0001d860: 6566 6964 2729 0a20 2020 2020 2020 2072  efid').        r
+0001d870: 6574 7572 6e20 7b0a 2020 2020 2020 2020  eturn {.        
+0001d880: 2020 2020 2769 6e66 6f27 3a20 7472 616e      'info': tran
+0001d890: 7366 6572 2c0a 2020 2020 2020 2020 2020  sfer,.          
+0001d8a0: 2020 2769 6427 3a20 7265 6669 642c 0a20    'id': refid,. 
+0001d8b0: 2020 2020 2020 2020 2020 2027 7469 6d65             'time
+0001d8c0: 7374 616d 7027 3a20 4e6f 6e65 2c0a 2020  stamp': None,.  
+0001d8d0: 2020 2020 2020 2020 2020 2764 6174 6574            'datet
+0001d8e0: 696d 6527 3a20 4e6f 6e65 2c0a 2020 2020  ime': None,.    
+0001d8f0: 2020 2020 2020 2020 2763 7572 7265 6e63          'currenc
+0001d900: 7927 3a20 7365 6c66 2e73 6166 655f 7374  y': self.safe_st
+0001d910: 7269 6e67 2863 7572 7265 6e63 792c 2027  ring(currency, '
+0001d920: 636f 6465 2729 2c0a 2020 2020 2020 2020  code'),.        
+0001d930: 2020 2020 2761 6d6f 756e 7427 3a20 4e6f      'amount': No
+0001d940: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+0001d950: 2766 726f 6d41 6363 6f75 6e74 273a 204e  'fromAccount': N
+0001d960: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+0001d970: 2027 746f 4163 636f 756e 7427 3a20 4e6f   'toAccount': No
+0001d980: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+0001d990: 2773 7461 7475 7327 3a20 2773 7563 6573  'status': 'suces
+0001d9a0: 7327 2c0a 2020 2020 2020 2020 7d0a 0a20  s',.        }.. 
+0001d9b0: 2020 2064 6566 2073 6967 6e28 7365 6c66     def sign(self
+0001d9c0: 2c20 7061 7468 2c20 6170 693d 2770 7562  , path, api='pub
+0001d9d0: 6c69 6327 2c20 6d65 7468 6f64 3d27 4745  lic', method='GE
+0001d9e0: 5427 2c20 7061 7261 6d73 3d7b 7d2c 2068  T', params={}, h
+0001d9f0: 6561 6465 7273 3d4e 6f6e 652c 2062 6f64  eaders=None, bod
+0001da00: 793d 4e6f 6e65 293a 0a20 2020 2020 2020  y=None):.       
+0001da10: 2075 726c 203d 2027 2f27 202b 2073 656c   url = '/' + sel
+0001da20: 662e 7665 7273 696f 6e20 2b20 272f 2720  f.version + '/' 
+0001da30: 2b20 6170 6920 2b20 272f 2720 2b20 7061  + api + '/' + pa
+0001da40: 7468 0a20 2020 2020 2020 2069 6620 6170  th.        if ap
+0001da50: 6920 3d3d 2027 7075 626c 6963 273a 0a20  i == 'public':. 
+0001da60: 2020 2020 2020 2020 2020 2069 6620 7061             if pa
+0001da70: 7261 6d73 3a0a 2020 2020 2020 2020 2020  rams:.          
+0001da80: 2020 2020 2020 2320 7572 6c65 6e63 6f64        # urlencod
+0001da90: 654e 6573 7465 6420 6973 2075 7365 6420  eNested is used 
+0001daa0: 746f 2061 6464 7265 7373 2068 7474 7073  to address https
+0001dab0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6363  ://github.com/cc
+0001dac0: 7874 2f63 6378 742f 6973 7375 6573 2f31  xt/ccxt/issues/1
+0001dad0: 3238 3732 0a20 2020 2020 2020 2020 2020  2872.           
+0001dae0: 2020 2020 2075 726c 202b 3d20 273f 2720       url += '?' 
+0001daf0: 2b20 7365 6c66 2e75 726c 656e 636f 6465  + self.urlencode
+0001db00: 5f6e 6573 7465 6428 7061 7261 6d73 290a  _nested(params).
+0001db10: 2020 2020 2020 2020 656c 6966 2061 7069          elif api
+0001db20: 203d 3d20 2770 7269 7661 7465 273a 0a20   == 'private':. 
+0001db30: 2020 2020 2020 2020 2020 2069 7343 616e             isCan
+0001db40: 6365 6c4f 7264 6572 4261 7463 6820 3d20  celOrderBatch = 
+0001db50: 2870 6174 6820 3d3d 2027 4361 6e63 656c  (path == 'Cancel
+0001db60: 4f72 6465 7242 6174 6368 2729 0a20 2020  OrderBatch').   
+0001db70: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
+0001db80: 6563 6b5f 7265 7175 6972 6564 5f63 7265  eck_required_cre
+0001db90: 6465 6e74 6961 6c73 2829 0a20 2020 2020  dentials().     
+0001dba0: 2020 2020 2020 206e 6f6e 6365 203d 2073         nonce = s
+0001dbb0: 7472 2873 656c 662e 6e6f 6e63 6528 2929  tr(self.nonce())
+0001dbc0: 0a20 2020 2020 2020 2020 2020 2023 2075  .            # u
+0001dbd0: 726c 656e 636f 6465 4e65 7374 6564 2069  rlencodeNested i
+0001dbe0: 7320 7573 6564 2074 6f20 6164 6472 6573  s used to addres
+0001dbf0: 7320 6874 7470 733a 2f2f 6769 7468 7562  s https://github
+0001dc00: 2e63 6f6d 2f63 6378 742f 6363 7874 2f69  .com/ccxt/ccxt/i
+0001dc10: 7373 7565 732f 3132 3837 320a 2020 2020  ssues/12872.    
+0001dc20: 2020 2020 2020 2020 6966 2069 7343 616e          if isCan
+0001dc30: 6365 6c4f 7264 6572 4261 7463 683a 0a20  celOrderBatch:. 
+0001dc40: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0001dc50: 6f64 7920 3d20 7365 6c66 2e6a 736f 6e28  ody = self.json(
+0001dc60: 7365 6c66 2e65 7874 656e 6428 7b27 6e6f  self.extend({'no
+0001dc70: 6e63 6527 3a20 6e6f 6e63 657d 2c20 7061  nce': nonce}, pa
+0001dc80: 7261 6d73 2929 0a20 2020 2020 2020 2020  rams)).         
+0001dc90: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0001dca0: 2020 2020 2020 2020 2062 6f64 7920 3d20           body = 
+0001dcb0: 7365 6c66 2e75 726c 656e 636f 6465 5f6e  self.urlencode_n
+0001dcc0: 6573 7465 6428 7365 6c66 2e65 7874 656e  ested(self.exten
+0001dcd0: 6428 7b27 6e6f 6e63 6527 3a20 6e6f 6e63  d({'nonce': nonc
+0001dce0: 657d 2c20 7061 7261 6d73 2929 0a20 2020  e}, params)).   
+0001dcf0: 2020 2020 2020 2020 2061 7574 6820 3d20           auth = 
+0001dd00: 7365 6c66 2e65 6e63 6f64 6528 6e6f 6e63  self.encode(nonc
+0001dd10: 6520 2b20 626f 6479 290a 2020 2020 2020  e + body).      
+0001dd20: 2020 2020 2020 6861 7368 203d 2073 656c        hash = sel
+0001dd30: 662e 6861 7368 2861 7574 682c 2027 7368  f.hash(auth, 'sh
+0001dd40: 6132 3536 272c 2027 6269 6e61 7279 2729  a256', 'binary')
+0001dd50: 0a20 2020 2020 2020 2020 2020 2062 696e  .            bin
+0001dd60: 6172 7920 3d20 7365 6c66 2e65 6e63 6f64  ary = self.encod
+0001dd70: 6528 7572 6c29 0a20 2020 2020 2020 2020  e(url).         
+0001dd80: 2020 2062 696e 6861 7368 203d 2073 656c     binhash = sel
+0001dd90: 662e 6269 6e61 7279 5f63 6f6e 6361 7428  f.binary_concat(
+0001dda0: 6269 6e61 7279 2c20 6861 7368 290a 2020  binary, hash).  
+0001ddb0: 2020 2020 2020 2020 2020 7365 6372 6574            secret
+0001ddc0: 203d 2073 656c 662e 6261 7365 3634 5f74   = self.base64_t
+0001ddd0: 6f5f 6269 6e61 7279 2873 656c 662e 7365  o_binary(self.se
+0001dde0: 6372 6574 290a 2020 2020 2020 2020 2020  cret).          
+0001ddf0: 2020 7369 676e 6174 7572 6520 3d20 7365    signature = se
+0001de00: 6c66 2e68 6d61 6328 6269 6e68 6173 682c  lf.hmac(binhash,
+0001de10: 2073 6563 7265 742c 2068 6173 686c 6962   secret, hashlib
+0001de20: 2e73 6861 3531 322c 2027 6261 7365 3634  .sha512, 'base64
+0001de30: 2729 0a20 2020 2020 2020 2020 2020 2068  ').            h
+0001de40: 6561 6465 7273 203d 207b 0a20 2020 2020  eaders = {.     
+0001de50: 2020 2020 2020 2020 2020 2027 4150 492d             'API-
+0001de60: 4b65 7927 3a20 7365 6c66 2e61 7069 4b65  Key': self.apiKe
+0001de70: 792c 0a20 2020 2020 2020 2020 2020 2020  y,.             
+0001de80: 2020 2027 4150 492d 5369 676e 273a 2073     'API-Sign': s
+0001de90: 6967 6e61 7475 7265 2c0a 2020 2020 2020  ignature,.      
+0001dea0: 2020 2020 2020 2020 2020 2320 2743 6f6e            # 'Con
+0001deb0: 7465 6e74 2d54 7970 6527 3a20 2761 7070  tent-Type': 'app
+0001dec0: 6c69 6361 7469 6f6e 2f78 2d77 7777 2d66  lication/x-www-f
+0001ded0: 6f72 6d2d 7572 6c65 6e63 6f64 6564 272c  orm-urlencoded',
+0001dee0: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+0001def0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+0001df00: 4361 6e63 656c 4f72 6465 7242 6174 6368  CancelOrderBatch
+0001df10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001df20: 2020 6865 6164 6572 735b 2743 6f6e 7465    headers['Conte
+0001df30: 6e74 2d54 7970 6527 5d20 3d20 2761 7070  nt-Type'] = 'app
+0001df40: 6c69 6361 7469 6f6e 2f6a 736f 6e27 0a20  lication/json'. 
+0001df50: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0001df60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001df70: 2068 6561 6465 7273 5b27 436f 6e74 656e   headers['Conten
+0001df80: 742d 5479 7065 275d 203d 2027 6170 706c  t-Type'] = 'appl
+0001df90: 6963 6174 696f 6e2f 782d 7777 772d 666f  ication/x-www-fo
+0001dfa0: 726d 2d75 726c 656e 636f 6465 6427 0a20  rm-urlencoded'. 
+0001dfb0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0001dfc0: 2020 2020 2020 2020 2075 726c 203d 2027           url = '
+0001dfd0: 2f27 202b 2070 6174 680a 2020 2020 2020  /' + path.      
+0001dfe0: 2020 7572 6c20 3d20 7365 6c66 2e75 726c    url = self.url
+0001dff0: 735b 2761 7069 275d 5b61 7069 5d20 2b20  s['api'][api] + 
+0001e000: 7572 6c0a 2020 2020 2020 2020 7265 7475  url.        retu
+0001e010: 726e 207b 2775 726c 273a 2075 726c 2c20  rn {'url': url, 
+0001e020: 276d 6574 686f 6427 3a20 6d65 7468 6f64  'method': method
+0001e030: 2c20 2762 6f64 7927 3a20 626f 6479 2c20  , 'body': body, 
+0001e040: 2768 6561 6465 7273 273a 2068 6561 6465  'headers': heade
+0001e050: 7273 7d0a 0a20 2020 2064 6566 206e 6f6e  rs}..    def non
+0001e060: 6365 2873 656c 6629 3a0a 2020 2020 2020  ce(self):.      
+0001e070: 2020 7265 7475 726e 2073 656c 662e 6d69    return self.mi
+0001e080: 6c6c 6973 6563 6f6e 6473 2829 0a0a 2020  lliseconds()..  
+0001e090: 2020 6465 6620 6861 6e64 6c65 5f65 7272    def handle_err
+0001e0a0: 6f72 7328 7365 6c66 2c20 636f 6465 2c20  ors(self, code, 
+0001e0b0: 7265 6173 6f6e 2c20 7572 6c2c 206d 6574  reason, url, met
+0001e0c0: 686f 642c 2068 6561 6465 7273 2c20 626f  hod, headers, bo
+0001e0d0: 6479 2c20 7265 7370 6f6e 7365 2c20 7265  dy, response, re
+0001e0e0: 7175 6573 7448 6561 6465 7273 2c20 7265  questHeaders, re
+0001e0f0: 7175 6573 7442 6f64 7929 3a0a 2020 2020  questBody):.    
+0001e100: 2020 2020 6966 2063 6f64 6520 3d3d 2035      if code == 5
+0001e110: 3230 3a0a 2020 2020 2020 2020 2020 2020  20:.            
+0001e120: 7261 6973 6520 4578 6368 616e 6765 4e6f  raise ExchangeNo
+0001e130: 7441 7661 696c 6162 6c65 2873 656c 662e  tAvailable(self.
+0001e140: 6964 202b 2027 2027 202b 2073 7472 2863  id + ' ' + str(c
+0001e150: 6f64 6529 202b 2027 2027 202b 2072 6561  ode) + ' ' + rea
+0001e160: 736f 6e29 0a20 2020 2020 2020 2023 2074  son).        # t
+0001e170: 6f64 6f3a 2072 6577 7269 7465 2073 656c  odo: rewrite sel
+0001e180: 6620 666f 7220 2262 726f 6164 2220 6578  f for "broad" ex
+0001e190: 6365 7074 696f 6e73 206d 6174 6368 696e  ceptions matchin
+0001e1a0: 670a 2020 2020 2020 2020 6966 2062 6f64  g.        if bod
+0001e1b0: 792e 6669 6e64 2827 496e 7661 6c69 6420  y.find('Invalid 
+0001e1c0: 6f72 6465 7227 2920 3e3d 2030 3a0a 2020  order') >= 0:.  
+0001e1d0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0001e1e0: 496e 7661 6c69 644f 7264 6572 2873 656c  InvalidOrder(sel
+0001e1f0: 662e 6964 202b 2027 2027 202b 2062 6f64  f.id + ' ' + bod
+0001e200: 7929 0a20 2020 2020 2020 2069 6620 626f  y).        if bo
+0001e210: 6479 2e66 696e 6428 2749 6e76 616c 6964  dy.find('Invalid
+0001e220: 206e 6f6e 6365 2729 203e 3d20 303a 0a20   nonce') >= 0:. 
+0001e230: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0001e240: 2049 6e76 616c 6964 4e6f 6e63 6528 7365   InvalidNonce(se
+0001e250: 6c66 2e69 6420 2b20 2720 2720 2b20 626f  lf.id + ' ' + bo
+0001e260: 6479 290a 2020 2020 2020 2020 6966 2062  dy).        if b
+0001e270: 6f64 792e 6669 6e64 2827 496e 7375 6666  ody.find('Insuff
+0001e280: 6963 6965 6e74 2066 756e 6473 2729 203e  icient funds') >
+0001e290: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+0001e2a0: 2072 6169 7365 2049 6e73 7566 6669 6369   raise Insuffici
+0001e2b0: 656e 7446 756e 6473 2873 656c 662e 6964  entFunds(self.id
+0001e2c0: 202b 2027 2027 202b 2062 6f64 7929 0a20   + ' ' + body). 
+0001e2d0: 2020 2020 2020 2069 6620 626f 6479 2e66         if body.f
+0001e2e0: 696e 6428 2743 616e 6365 6c20 7065 6e64  ind('Cancel pend
+0001e2f0: 696e 6727 2920 3e3d 2030 3a0a 2020 2020  ing') >= 0:.    
+0001e300: 2020 2020 2020 2020 7261 6973 6520 4361          raise Ca
+0001e310: 6e63 656c 5065 6e64 696e 6728 7365 6c66  ncelPending(self
+0001e320: 2e69 6420 2b20 2720 2720 2b20 626f 6479  .id + ' ' + body
+0001e330: 290a 2020 2020 2020 2020 6966 2062 6f64  ).        if bod
+0001e340: 792e 6669 6e64 2827 496e 7661 6c69 6420  y.find('Invalid 
+0001e350: 6172 6775 6d65 6e74 733a 766f 6c75 6d65  arguments:volume
+0001e360: 2729 203e 3d20 303a 0a20 2020 2020 2020  ') >= 0:.       
+0001e370: 2020 2020 2072 6169 7365 2049 6e76 616c       raise Inval
+0001e380: 6964 4f72 6465 7228 7365 6c66 2e69 6420  idOrder(self.id 
+0001e390: 2b20 2720 2720 2b20 626f 6479 290a 2020  + ' ' + body).  
+0001e3a0: 2020 2020 2020 6966 2062 6f64 792e 6669        if body.fi
+0001e3b0: 6e64 2827 5261 7465 206c 696d 6974 2065  nd('Rate limit e
+0001e3c0: 7863 6565 6465 6427 2920 3e3d 2030 3a0a  xceeded') >= 0:.
+0001e3d0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0001e3e0: 6520 5261 7465 4c69 6d69 7445 7863 6565  e RateLimitExcee
+0001e3f0: 6465 6428 7365 6c66 2e69 6420 2b20 2720  ded(self.id + ' 
+0001e400: 2720 2b20 626f 6479 290a 2020 2020 2020  ' + body).      
+0001e410: 2020 6966 2072 6573 706f 6e73 6520 6973    if response is
+0001e420: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0001e430: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
+0001e440: 2020 2020 2020 2069 6620 626f 6479 5b30         if body[0
+0001e450: 5d20 3d3d 2027 7b27 3a0a 2020 2020 2020  ] == '{':.      
+0001e460: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
+0001e470: 6e73 7461 6e63 6528 7265 7370 6f6e 7365  nstance(response
+0001e480: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
+0001e490: 2020 2020 2020 2020 6966 2027 6572 726f          if 'erro
+0001e4a0: 7227 2069 6e20 7265 7370 6f6e 7365 3a0a  r' in response:.
+0001e4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e4c0: 2020 2020 6e75 6d45 7272 6f72 7320 3d20      numErrors = 
+0001e4d0: 6c65 6e28 7265 7370 6f6e 7365 5b27 6572  len(response['er
+0001e4e0: 726f 7227 5d29 0a20 2020 2020 2020 2020  ror']).         
+0001e4f0: 2020 2020 2020 2020 2020 2069 6620 6e75             if nu
+0001e500: 6d45 7272 6f72 733a 0a20 2020 2020 2020  mErrors:.       
+0001e510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e520: 206d 6573 7361 6765 203d 2073 656c 662e   message = self.
+0001e530: 6964 202b 2027 2027 202b 2062 6f64 790a  id + ' ' + body.
+0001e540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e550: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+0001e560: 2072 616e 6765 2830 2c20 6c65 6e28 7265   range(0, len(re
+0001e570: 7370 6f6e 7365 5b27 6572 726f 7227 5d29  sponse['error'])
+0001e580: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0001e590: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0001e5a0: 7272 6f72 203d 2072 6573 706f 6e73 655b  rror = response[
+0001e5b0: 2765 7272 6f72 275d 5b69 5d0a 2020 2020  'error'][i].    
+0001e5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e5d0: 2020 2020 2020 2020 7365 6c66 2e74 6872          self.thr
+0001e5e0: 6f77 5f65 7861 6374 6c79 5f6d 6174 6368  ow_exactly_match
+0001e5f0: 6564 5f65 7863 6570 7469 6f6e 2873 656c  ed_exception(sel
+0001e600: 662e 6578 6365 7074 696f 6e73 2c20 6572  f.exceptions, er
+0001e610: 726f 722c 206d 6573 7361 6765 290a 2020  ror, message).  
+0001e620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e630: 2020 2020 2020 7261 6973 6520 4578 6368        raise Exch
+0001e640: 616e 6765 4572 726f 7228 6d65 7373 6167  angeError(messag
+0001e650: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
+0001e660: 6e20 4e6f 6e65 0a                        n None.
```

### Comparing `ccxt-4.2.91/ccxt/async_support/krakenfutures.py` & `ccxt-4.2.92/ccxt/async_support/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/kucoin.py` & `ccxt-4.2.92/ccxt/async_support/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/kucoinfutures.py` & `ccxt-4.2.92/ccxt/async_support/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/kuna.py` & `ccxt-4.2.92/ccxt/async_support/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/latoken.py` & `ccxt-4.2.92/ccxt/async_support/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/lbank.py` & `ccxt-4.2.92/ccxt/async_support/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/luno.py` & `ccxt-4.2.92/ccxt/async_support/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/lykke.py` & `ccxt-4.2.92/ccxt/async_support/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/mercado.py` & `ccxt-4.2.92/ccxt/async_support/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/mexc.py` & `ccxt-4.2.92/ccxt/async_support/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/ndax.py` & `ccxt-4.2.92/ccxt/async_support/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/novadax.py` & `ccxt-4.2.92/ccxt/async_support/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/oceanex.py` & `ccxt-4.2.92/ccxt/async_support/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/okcoin.py` & `ccxt-4.2.92/ccxt/async_support/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/okx.py` & `ccxt-4.2.92/ccxt/async_support/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/onetrading.py` & `ccxt-4.2.92/ccxt/async_support/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/p2b.py` & `ccxt-4.2.92/ccxt/async_support/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/paymium.py` & `ccxt-4.2.92/ccxt/async_support/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/phemex.py` & `ccxt-4.2.92/ccxt/async_support/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/poloniex.py` & `ccxt-4.2.92/ccxt/async_support/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/poloniexfutures.py` & `ccxt-4.2.92/ccxt/async_support/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/probit.py` & `ccxt-4.2.92/ccxt/async_support/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/timex.py` & `ccxt-4.2.92/ccxt/async_support/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/tokocrypto.py` & `ccxt-4.2.92/ccxt/async_support/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/tradeogre.py` & `ccxt-4.2.92/ccxt/async_support/tradeogre.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/upbit.py` & `ccxt-4.2.92/ccxt/async_support/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/wavesexchange.py` & `ccxt-4.2.92/ccxt/async_support/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/wazirx.py` & `ccxt-4.2.92/ccxt/async_support/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/whitebit.py` & `ccxt-4.2.92/ccxt/async_support/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/woo.py` & `ccxt-4.2.92/ccxt/async_support/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/yobit.py` & `ccxt-4.2.92/ccxt/async_support/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/zaif.py` & `ccxt-4.2.92/ccxt/async_support/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/async_support/zonda.py` & `ccxt-4.2.92/ccxt/async_support/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/base/__init__.py` & `ccxt-4.2.92/ccxt/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/base/decimal_to_precision.py` & `ccxt-4.2.92/ccxt/base/decimal_to_precision.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/base/errors.py` & `ccxt-4.2.92/ccxt/base/errors.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/base/exchange.py` & `ccxt-4.2.92/ccxt/base/exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Base exchange class"""
 
 # -----------------------------------------------------------------------------
 
-__version__ = '4.2.91'
+__version__ = '4.2.92'
 
 # -----------------------------------------------------------------------------
 
 from ccxt.base.errors import ExchangeError
 from ccxt.base.errors import NetworkError
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import AuthenticationError
@@ -5448,29 +5448,32 @@
             month = 'NOV'
         elif monthRaw == '12':
             month = 'DEC'
         reconstructedDate = day + month + year
         return reconstructedDate
 
     def convert_market_id_expire_date(self, date: str):
-        # parse 19JAN24 to 240119
+        # parse 03JAN24 to 240103
         monthMappping = {
             'JAN': '01',
             'FEB': '02',
             'MAR': '03',
             'APR': '04',
             'MAY': '05',
             'JUN': '06',
             'JUL': '07',
             'AUG': '08',
             'SEP': '09',
             'OCT': '10',
             'NOV': '11',
             'DEC': '12',
         }
+        # if exchange omits first zero and provides i.e. '3JAN24' instead of '03JAN24'
+        if len(date) == 6:
+            date = '0' + date
         year = date[0:2]
         monthName = date[2:5]
         month = self.safe_string(monthMappping, monthName)
         day = date[5:7]
         reconstructedDate = day + month + year
         return reconstructedDate
```

### Comparing `ccxt-4.2.91/ccxt/base/precise.py` & `ccxt-4.2.92/ccxt/base/precise.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/base/types.py` & `ccxt-4.2.92/ccxt/base/types.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/bequant.py` & `ccxt-4.2.92/ccxt/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/bigone.py` & `ccxt-4.2.92/ccxt/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/binance.py` & `ccxt-4.2.92/ccxt/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/binancecoinm.py` & `ccxt-4.2.92/ccxt/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/binanceus.py` & `ccxt-4.2.92/ccxt/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/binanceusdm.py` & `ccxt-4.2.92/ccxt/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/bingx.py` & `ccxt-4.2.92/ccxt/bingx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/bit2c.py` & `ccxt-4.2.92/ccxt/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/bitbank.py` & `ccxt-4.2.92/ccxt/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/bitbns.py` & `ccxt-4.2.92/ccxt/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/bitfinex.py` & `ccxt-4.2.92/ccxt/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/bitfinex2.py` & `ccxt-4.2.92/ccxt/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/bitflyer.py` & `ccxt-4.2.92/ccxt/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/bitget.py` & `ccxt-4.2.92/ccxt/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/bithumb.py` & `ccxt-4.2.92/ccxt/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/bitmart.py` & `ccxt-4.2.92/ccxt/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/bitmex.py` & `ccxt-4.2.92/ccxt/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/bitopro.py` & `ccxt-4.2.92/ccxt/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/bitrue.py` & `ccxt-4.2.92/ccxt/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/bitso.py` & `ccxt-4.2.92/ccxt/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/bitstamp.py` & `ccxt-4.2.92/ccxt/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/bitteam.py` & `ccxt-4.2.92/ccxt/bitteam.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/bitvavo.py` & `ccxt-4.2.92/ccxt/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/bl3p.py` & `ccxt-4.2.92/ccxt/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/blockchaincom.py` & `ccxt-4.2.92/ccxt/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/blofin.py` & `ccxt-4.2.92/ccxt/blofin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/btcalpha.py` & `ccxt-4.2.92/ccxt/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/btcbox.py` & `ccxt-4.2.92/ccxt/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/btcmarkets.py` & `ccxt-4.2.92/ccxt/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/btcturk.py` & `ccxt-4.2.92/ccxt/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/bybit.py` & `ccxt-4.2.92/ccxt/bybit.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,14 +380,15 @@
                         'v5/lending/info': 5,
                         'v5/lending/history-order': 5,
                         'v5/lending/account': 5,
                         # broker
                         'v5/broker/earning-record': 5,
                         'v5/broker/earnings-info': 5,
                         'v5/broker/account-info': 5,
+                        'v5/broker/asset/query-sub-member-deposit-record': 10,
                     },
                     'post': {
                         # Legacy option USDC
                         'option/usdc/openapi/private/v1/place-order': 2.5,
                         'option/usdc/openapi/private/v1/replace-order': 2.5,
                         'option/usdc/openapi/private/v1/cancel-order': 2.5,
                         'option/usdc/openapi/private/v1/cancel-all': 2.5,
```

### Comparing `ccxt-4.2.91/ccxt/cex.py` & `ccxt-4.2.92/ccxt/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/coinbase.py` & `ccxt-4.2.92/ccxt/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/coinbaseinternational.py` & `ccxt-4.2.92/ccxt/coinbaseinternational.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/coinbasepro.py` & `ccxt-4.2.92/ccxt/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/coincheck.py` & `ccxt-4.2.92/ccxt/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/coinex.py` & `ccxt-4.2.92/ccxt/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/coinlist.py` & `ccxt-4.2.92/ccxt/coinlist.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/coinmate.py` & `ccxt-4.2.92/ccxt/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/coinmetro.py` & `ccxt-4.2.92/ccxt/coinmetro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/coinone.py` & `ccxt-4.2.92/ccxt/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/coinsph.py` & `ccxt-4.2.92/ccxt/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/coinspot.py` & `ccxt-4.2.92/ccxt/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/cryptocom.py` & `ccxt-4.2.92/ccxt/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/currencycom.py` & `ccxt-4.2.92/ccxt/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/delta.py` & `ccxt-4.2.92/ccxt/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/deribit.py` & `ccxt-4.2.92/ccxt/deribit.py`

 * *Files 0% similar despite different names*

```diff
@@ -688,125 +688,135 @@
             'code': self.safe_currency_code(None, currency),
         }
 
     def fetch_markets(self, params={}) -> List[Market]:
         """
         retrieves data on all markets for deribit
         :see: https://docs.deribit.com/#public-get_currencies
+        :see: https://docs.deribit.com/#public-get_instruments
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict[]: an array of objects representing market data
         """
-        currenciesResponse = self.publicGetGetCurrencies(params)
-        #
-        #     {
-        #         "jsonrpc": "2.0",
-        #         "result": [
-        #             {
-        #                 "withdrawal_priorities": [
-        #                     {value: 0.15, name: "very_low"},
-        #                     {value: 1.5, name: "very_high"},
-        #                 ],
-        #                 "withdrawal_fee": 0.0005,
-        #                 "min_withdrawal_fee": 0.0005,
-        #                 "min_confirmations": 1,
-        #                 "fee_precision": 4,
-        #                 "currency_long": "Bitcoin",
-        #                 "currency": "BTC",
-        #                 "coin_type": "BITCOIN"
-        #             }
-        #         ],
-        #         "usIn": 1583761588590479,
-        #         "usOut": 1583761588590544,
-        #         "usDiff": 65,
-        #         "testnet": False
-        #     }
-        #
-        parsedMarkets = {}
-        currenciesResult = self.safe_value(currenciesResponse, 'result', [])
+        instrumentsResponses = []
         result = []
-        for i in range(0, len(currenciesResult)):
-            currencyId = self.safe_string(currenciesResult[i], 'currency')
-            request = {
-                'currency': currencyId,
-            }
-            instrumentsResponse = self.publicGetGetInstruments(self.extend(request, params))
+        parsedMarkets = {}
+        fetchAllMarkets = None
+        fetchAllMarkets, params = self.handle_option_and_params(params, 'fetchMarkets', 'fetchAllMarkets', True)
+        if fetchAllMarkets:
+            instrumentsResponse = self.publicGetGetInstruments(params)
+            instrumentsResponses.append(instrumentsResponse)
+        else:
+            currenciesResponse = self.publicGetGetCurrencies(params)
             #
             #     {
-            #         "jsonrpc":"2.0",
-            #         "result":[
-            #             {
-            #                 "tick_size":0.0005,
-            #                 "taker_commission":0.0003,
-            #                 "strike":52000.0,
-            #                 "settlement_period":"month",
-            #                 "settlement_currency":"BTC",
-            #                 "quote_currency":"BTC",
-            #                 "option_type":"put",  # put, call
-            #                 "min_trade_amount":0.1,
-            #                 "maker_commission":0.0003,
-            #                 "kind":"option",
-            #                 "is_active":true,
-            #                 "instrument_name":"BTC-24JUN22-52000-P",
-            #                 "expiration_timestamp":1656057600000,
-            #                 "creation_timestamp":1648199543000,
-            #                 "counter_currency":"USD",
-            #                 "contract_size":1.0,
-            #                 "block_trade_commission":0.0003,
-            #                 "base_currency":"BTC"
-            #             },
-            #             {
-            #                 "tick_size":0.5,
-            #                 "taker_commission":0.0005,
-            #                 "settlement_period":"month",  # month, week
-            #                 "settlement_currency":"BTC",
-            #                 "quote_currency":"USD",
-            #                 "min_trade_amount":10.0,
-            #                 "max_liquidation_commission":0.0075,
-            #                 "max_leverage":50,
-            #                 "maker_commission":0.0,
-            #                 "kind":"future",
-            #                 "is_active":true,
-            #                 "instrument_name":"BTC-27MAY22",
-            #                 "future_type":"reversed",
-            #                 "expiration_timestamp":1653638400000,
-            #                 "creation_timestamp":1648195209000,
-            #                 "counter_currency":"USD",
-            #                 "contract_size":10.0,
-            #                 "block_trade_commission":0.0001,
-            #                 "base_currency":"BTC"
-            #             },
+            #         "jsonrpc": "2.0",
+            #         "result": [
             #             {
-            #                 "tick_size":0.5,
-            #                 "taker_commission":0.0005,
-            #                 "settlement_period":"perpetual",
-            #                 "settlement_currency":"BTC",
-            #                 "quote_currency":"USD",
-            #                 "min_trade_amount":10.0,
-            #                 "max_liquidation_commission":0.0075,
-            #                 "max_leverage":50,
-            #                 "maker_commission":0.0,
-            #                 "kind":"future",
-            #                 "is_active":true,
-            #                 "instrument_name":"BTC-PERPETUAL",
-            #                 "future_type":"reversed",
-            #                 "expiration_timestamp":32503708800000,
-            #                 "creation_timestamp":1534242287000,
-            #                 "counter_currency":"USD",
-            #                 "contract_size":10.0,
-            #                 "block_trade_commission":0.0001,
-            #                 "base_currency":"BTC"
-            #             },
+            #                 "withdrawal_priorities": [
+            #                     {value: 0.15, name: "very_low"},
+            #                     {value: 1.5, name: "very_high"},
+            #                 ],
+            #                 "withdrawal_fee": 0.0005,
+            #                 "min_withdrawal_fee": 0.0005,
+            #                 "min_confirmations": 1,
+            #                 "fee_precision": 4,
+            #                 "currency_long": "Bitcoin",
+            #                 "currency": "BTC",
+            #                 "coin_type": "BITCOIN"
+            #             }
             #         ],
-            #         "usIn":1648691472831791,
-            #         "usOut":1648691472831896,
-            #         "usDiff":105,
-            #         "testnet":false
+            #         "usIn": 1583761588590479,
+            #         "usOut": 1583761588590544,
+            #         "usDiff": 65,
+            #         "testnet": False
             #     }
             #
-            instrumentsResult = self.safe_value(instrumentsResponse, 'result', [])
+            currenciesResult = self.safe_value(currenciesResponse, 'result', [])
+            for i in range(0, len(currenciesResult)):
+                currencyId = self.safe_string(currenciesResult[i], 'currency')
+                request = {
+                    'currency': currencyId,
+                }
+                instrumentsResponse = self.publicGetGetInstruments(self.extend(request, params))
+                #
+                #     {
+                #         "jsonrpc":"2.0",
+                #         "result":[
+                #             {
+                #                 "tick_size":0.0005,
+                #                 "taker_commission":0.0003,
+                #                 "strike":52000.0,
+                #                 "settlement_period":"month",
+                #                 "settlement_currency":"BTC",
+                #                 "quote_currency":"BTC",
+                #                 "option_type":"put",  # put, call
+                #                 "min_trade_amount":0.1,
+                #                 "maker_commission":0.0003,
+                #                 "kind":"option",
+                #                 "is_active":true,
+                #                 "instrument_name":"BTC-24JUN22-52000-P",
+                #                 "expiration_timestamp":1656057600000,
+                #                 "creation_timestamp":1648199543000,
+                #                 "counter_currency":"USD",
+                #                 "contract_size":1.0,
+                #                 "block_trade_commission":0.0003,
+                #                 "base_currency":"BTC"
+                #             },
+                #             {
+                #                 "tick_size":0.5,
+                #                 "taker_commission":0.0005,
+                #                 "settlement_period":"month",  # month, week
+                #                 "settlement_currency":"BTC",
+                #                 "quote_currency":"USD",
+                #                 "min_trade_amount":10.0,
+                #                 "max_liquidation_commission":0.0075,
+                #                 "max_leverage":50,
+                #                 "maker_commission":0.0,
+                #                 "kind":"future",
+                #                 "is_active":true,
+                #                 "instrument_name":"BTC-27MAY22",
+                #                 "future_type":"reversed",
+                #                 "expiration_timestamp":1653638400000,
+                #                 "creation_timestamp":1648195209000,
+                #                 "counter_currency":"USD",
+                #                 "contract_size":10.0,
+                #                 "block_trade_commission":0.0001,
+                #                 "base_currency":"BTC"
+                #             },
+                #             {
+                #                 "tick_size":0.5,
+                #                 "taker_commission":0.0005,
+                #                 "settlement_period":"perpetual",
+                #                 "settlement_currency":"BTC",
+                #                 "quote_currency":"USD",
+                #                 "min_trade_amount":10.0,
+                #                 "max_liquidation_commission":0.0075,
+                #                 "max_leverage":50,
+                #                 "maker_commission":0.0,
+                #                 "kind":"future",
+                #                 "is_active":true,
+                #                 "instrument_name":"BTC-PERPETUAL",
+                #                 "future_type":"reversed",
+                #                 "expiration_timestamp":32503708800000,
+                #                 "creation_timestamp":1534242287000,
+                #                 "counter_currency":"USD",
+                #                 "contract_size":10.0,
+                #                 "block_trade_commission":0.0001,
+                #                 "base_currency":"BTC"
+                #             },
+                #         ],
+                #         "usIn":1648691472831791,
+                #         "usOut":1648691472831896,
+                #         "usDiff":105,
+                #         "testnet":false
+                #     }
+                #
+                instrumentsResponses.append(instrumentsResponse)
+        for i in range(0, len(instrumentsResponses)):
+            instrumentsResult = self.safe_value(instrumentsResponses[i], 'result', [])
             for k in range(0, len(instrumentsResult)):
                 market = instrumentsResult[k]
                 kind = self.safe_string(market, 'kind')
                 isSpot = (kind == 'spot')
                 id = self.safe_string(market, 'instrument_name')
                 baseId = self.safe_string(market, 'base_currency')
                 quoteId = self.safe_string(market, 'counter_currency')
```

### Comparing `ccxt-4.2.91/ccxt/digifinex.py` & `ccxt-4.2.92/ccxt/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/exmo.py` & `ccxt-4.2.92/ccxt/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/flowbtc.py` & `ccxt-4.2.92/ccxt/flowbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/fmfwio.py` & `ccxt-4.2.92/ccxt/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/gate.py` & `ccxt-4.2.92/ccxt/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/gemini.py` & `ccxt-4.2.92/ccxt/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/hitbtc.py` & `ccxt-4.2.92/ccxt/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/hollaex.py` & `ccxt-4.2.92/ccxt/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/htx.py` & `ccxt-4.2.92/ccxt/htx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/huobijp.py` & `ccxt-4.2.92/ccxt/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/hyperliquid.py` & `ccxt-4.2.92/ccxt/hyperliquid.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/idex.py` & `ccxt-4.2.92/ccxt/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/independentreserve.py` & `ccxt-4.2.92/ccxt/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/indodax.py` & `ccxt-4.2.92/ccxt/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/kraken.py` & `ccxt-4.2.92/ccxt/kraken.py`

 * *Files 1% similar despite different names*

```diff
@@ -7058,567 +7058,689 @@
 0001b910: 6974 696f 6e73 0a20 2020 2020 2020 203a  itions.        :
 0001b920: 7365 653a 2068 7474 7073 3a2f 2f64 6f63  see: https://doc
 0001b930: 732e 6b72 616b 656e 2e63 6f6d 2f72 6573  s.kraken.com/res
 0001b940: 742f 2374 6167 2f41 6363 6f75 6e74 2d44  t/#tag/Account-D
 0001b950: 6174 612f 6f70 6572 6174 696f 6e2f 6765  ata/operation/ge
 0001b960: 744f 7065 6e50 6f73 6974 696f 6e73 0a20  tOpenPositions. 
 0001b970: 2020 2020 2020 203a 7061 7261 6d20 7374         :param st
-0001b980: 725b 5d7c 4e6f 6e65 2073 796d 626f 6c73  r[]|None symbols
-0001b990: 3a20 6e6f 7420 7573 6564 2062 7920 6b72  : not used by kr
-0001b9a0: 616b 656e 2066 6574 6368 506f 7369 7469  aken fetchPositi
-0001b9b0: 6f6e 7328 290a 2020 2020 2020 2020 3a70  ons().        :p
-0001b9c0: 6172 616d 2064 6963 7420 5b70 6172 616d  aram dict [param
-0001b9d0: 735d 3a20 6578 7472 6120 7061 7261 6d65  s]: extra parame
-0001b9e0: 7465 7273 2073 7065 6369 6669 6320 746f  ters specific to
-0001b9f0: 2074 6865 2065 7863 6861 6e67 6520 4150   the exchange AP
-0001ba00: 4920 656e 6470 6f69 6e74 0a20 2020 2020  I endpoint.     
-0001ba10: 2020 203a 7265 7475 726e 7320 6469 6374     :returns dict
-0001ba20: 5b5d 3a20 6120 6c69 7374 206f 6620 6070  []: a list of `p
-0001ba30: 6f73 6974 696f 6e20 7374 7275 6374 7572  osition structur
-0001ba40: 6520 3c68 7474 7073 3a2f 2f64 6f63 732e  e <https://docs.
-0001ba50: 6363 7874 2e63 6f6d 2f23 2f3f 6964 3d70  ccxt.com/#/?id=p
-0001ba60: 6f73 6974 696f 6e2d 7374 7275 6374 7572  osition-structur
-0001ba70: 653e 600a 2020 2020 2020 2020 2222 220a  e>`.        """.
-0001ba80: 2020 2020 2020 2020 7365 6c66 2e6c 6f61          self.loa
-0001ba90: 645f 6d61 726b 6574 7328 290a 2020 2020  d_markets().    
-0001baa0: 2020 2020 7265 7175 6573 7420 3d20 7b0a      request = {.
-0001bab0: 2020 2020 2020 2020 2020 2020 2320 2774              # 't
-0001bac0: 7869 6427 3a20 2763 6f6d 6d61 2064 656c  xid': 'comma del
-0001bad0: 696d 6974 6564 206c 6973 7420 6f66 2074  imited list of t
-0001bae0: 7261 6e73 6163 7469 6f6e 2069 6473 2074  ransaction ids t
-0001baf0: 6f20 7265 7374 7269 6374 206f 7574 7075  o restrict outpu
-0001bb00: 7420 746f 272c 0a20 2020 2020 2020 2020  t to',.         
-0001bb10: 2020 2023 2027 646f 6361 6c63 7327 3a20     # 'docalcs': 
-0001bb20: 4661 6c73 652c 2020 2320 7768 6574 6865  False,  # whethe
-0001bb30: 7220 6f72 206e 6f74 2074 6f20 696e 636c  r or not to incl
-0001bb40: 7564 6520 7072 6f66 6974 2f6c 6f73 7320  ude profit/loss 
-0001bb50: 6361 6c63 756c 6174 696f 6e73 0a20 2020  calculations.   
-0001bb60: 2020 2020 2020 2020 2023 2027 636f 6e73           # 'cons
-0001bb70: 6f6c 6964 6174 696f 6e27 3a20 276d 6172  olidation': 'mar
-0001bb80: 6b65 7427 2c20 2023 2077 6861 7420 746f  ket',  # what to
-0001bb90: 2063 6f6e 736f 6c69 6461 7465 2074 6865   consolidate the
-0001bba0: 2070 6f73 6974 696f 6e73 2064 6174 6120   positions data 
-0001bbb0: 6172 6f75 6e64 2c20 6d61 726b 6574 2077  around, market w
-0001bbc0: 696c 6c20 636f 6e73 6f6c 6964 6174 6520  ill consolidate 
-0001bbd0: 706f 7369 7469 6f6e 7320 6261 7365 6420  positions based 
-0001bbe0: 6f6e 206d 6172 6b65 7420 7061 6972 0a20  on market pair. 
-0001bbf0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-0001bc00: 2072 6573 706f 6e73 6520 3d20 7365 6c66   response = self
-0001bc10: 2e70 7269 7661 7465 506f 7374 4f70 656e  .privatePostOpen
-0001bc20: 506f 7369 7469 6f6e 7328 7365 6c66 2e65  Positions(self.e
-0001bc30: 7874 656e 6428 7265 7175 6573 742c 2070  xtend(request, p
-0001bc40: 6172 616d 7329 290a 2020 2020 2020 2020  arams)).        
-0001bc50: 230a 2020 2020 2020 2020 2320 6e6f 2063  #.        # no c
-0001bc60: 6f6e 736f 6c69 6461 7469 6f6e 0a20 2020  onsolidation.   
-0001bc70: 2020 2020 2023 0a20 2020 2020 2020 2023       #.        #
-0001bc80: 2020 2020 207b 0a20 2020 2020 2020 2023       {.        #
-0001bc90: 2020 2020 2020 2020 2022 6572 726f 7222           "error"
-0001bca0: 3a20 5b5d 2c0a 2020 2020 2020 2020 2320  : [],.        # 
-0001bcb0: 2020 2020 2020 2020 2272 6573 756c 7422          "result"
-0001bcc0: 3a20 7b0a 2020 2020 2020 2020 2320 2020  : {.        #   
-0001bcd0: 2020 2020 2020 2020 2020 2754 4755 464d            'TGUFM
-0001bce0: 592d 464c 4553 4a2d 5659 4958 334a 273a  Y-FLESJ-VYIX3J':
-0001bcf0: 207b 0a20 2020 2020 2020 2023 2020 2020   {.        #    
-0001bd00: 2020 2020 2020 2020 2020 2020 2022 6f72               "or
-0001bd10: 6465 7274 7869 6422 3a20 224f 334c 524e  dertxid": "O3LRN
-0001bd20: 552d 5a4b 4447 352d 584e 4344 4652 222c  U-ZKDG5-XNCDFR",
-0001bd30: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0001bd40: 2020 2020 2020 2020 2020 2022 706f 7373             "poss
-0001bd50: 7461 7475 7322 3a20 226f 7065 6e22 2c0a  tatus": "open",.
-0001bd60: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0001bd70: 2020 2020 2020 2020 2020 2270 6169 7222            "pair"
-0001bd80: 3a20 2245 5448 5553 4454 222c 0a20 2020  : "ETHUSDT",.   
-0001bd90: 2020 2020 2023 2020 2020 2020 2020 2020       #          
-0001bda0: 2020 2020 2020 2022 7469 6d65 223a 2020         "time":  
-0001bdb0: 3136 3131 3535 3732 3331 2e34 3538 342c  1611557231.4584,
-0001bdc0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0001bdd0: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-0001bde0: 223a 2022 6275 7922 2c0a 2020 2020 2020  ": "buy",.      
-0001bdf0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-0001be00: 2020 2020 226f 7264 6572 7479 7065 223a      "ordertype":
-0001be10: 2022 6d61 726b 6574 222c 0a20 2020 2020   "market",.     
-0001be20: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0001be30: 2020 2020 2022 636f 7374 223a 2022 3238       "cost": "28
-0001be40: 2e34 3938 3030 222c 0a20 2020 2020 2020  .49800",.       
-0001be50: 2023 2020 2020 2020 2020 2020 2020 2020   #              
-0001be60: 2020 2022 6665 6522 3a20 2230 2e30 3739     "fee": "0.079
-0001be70: 3739 222c 0a20 2020 2020 2020 2023 2020  79",.        #  
-0001be80: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0001be90: 766f 6c22 3a20 2230 2e30 3230 3030 3030  vol": "0.0200000
-0001bea0: 3022 2c0a 2020 2020 2020 2020 2320 2020  0",.        #   
-0001beb0: 2020 2020 2020 2020 2020 2020 2020 2276                "v
-0001bec0: 6f6c 5f63 6c6f 7365 6422 3a20 2230 2e30  ol_closed": "0.0
-0001bed0: 3030 3030 3030 3022 2c0a 2020 2020 2020  0000000",.      
-0001bee0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-0001bef0: 2020 2020 226d 6172 6769 6e22 3a20 2231      "margin": "1
-0001bf00: 342e 3234 3930 3022 2c0a 2020 2020 2020  4.24900",.      
-0001bf10: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-0001bf20: 2020 2020 2274 6572 6d73 223a 2022 302e      "terms": "0.
-0001bf30: 3032 3030 2520 7065 7220 3420 686f 7572  0200% per 4 hour
-0001bf40: 7322 2c0a 2020 2020 2020 2020 2320 2020  s",.        #   
-0001bf50: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-0001bf60: 6f6c 6c6f 7665 7274 6d22 3a20 2231 3631  ollovertm": "161
-0001bf70: 3135 3731 3633 3122 2c0a 2020 2020 2020  1571631",.      
-0001bf80: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-0001bf90: 2020 2020 226d 6973 6322 3a20 2222 2c0a      "misc": "",.
-0001bfa0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0001bfb0: 2020 2020 2020 2020 2020 226f 666c 6167            "oflag
-0001bfc0: 7322 3a20 2222 0a20 2020 2020 2020 2023  s": "".        #
-0001bfd0: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
-0001bfe0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0001bff0: 207d 0a20 2020 2020 2020 2023 2020 2020   }.        #    
-0001c000: 207d 0a20 2020 2020 2020 2023 0a20 2020   }.        #.   
-0001c010: 2020 2020 2023 2063 6f6e 736f 6c69 6461       # consolida
-0001c020: 7469 6f6e 2062 7920 6d61 726b 6574 0a20  tion by market. 
-0001c030: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
-0001c040: 2023 2020 2020 207b 0a20 2020 2020 2020   #     {.       
-0001c050: 2023 2020 2020 2020 2020 2022 6572 726f   #         "erro
-0001c060: 7222 3a20 5b5d 2c0a 2020 2020 2020 2020  r": [],.        
-0001c070: 2320 2020 2020 2020 2020 2272 6573 756c  #         "resul
-0001c080: 7422 3a20 5b0a 2020 2020 2020 2020 2320  t": [.        # 
-0001c090: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-0001c0a0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0001c0b0: 2020 2020 2020 2020 2270 6169 7222 3a20          "pair": 
-0001c0c0: 2245 5448 5553 4454 222c 0a20 2020 2020  "ETHUSDT",.     
-0001c0d0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0001c0e0: 2020 2020 2022 706f 7369 7469 6f6e 7322       "positions"
-0001c0f0: 3a20 2231 222c 0a20 2020 2020 2020 2023  : "1",.        #
-0001c100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c110: 2022 7479 7065 223a 2022 6275 7922 2c0a   "type": "buy",.
-0001c120: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0001c130: 2020 2020 2020 2020 2020 226c 6576 6572            "lever
-0001c140: 6167 6522 3a20 2232 2e30 3030 3030 222c  age": "2.00000",
-0001c150: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0001c160: 2020 2020 2020 2020 2020 2022 636f 7374             "cost
-0001c170: 223a 2022 3238 2e34 3938 3030 222c 0a20  ": "28.49800",. 
-0001c180: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0001c190: 2020 2020 2020 2020 2022 6665 6522 3a20           "fee": 
-0001c1a0: 2230 2e30 3739 3739 222c 0a20 2020 2020  "0.07979",.     
-0001c1b0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0001c1c0: 2020 2020 2022 766f 6c22 3a20 2230 2e30       "vol": "0.0
-0001c1d0: 3230 3030 3030 3022 2c0a 2020 2020 2020  2000000",.      
-0001c1e0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-0001c1f0: 2020 2020 2276 6f6c 5f63 6c6f 7365 6422      "vol_closed"
-0001c200: 3a20 2230 2e30 3030 3030 3030 3022 2c0a  : "0.00000000",.
-0001c210: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0001c220: 2020 2020 2020 2020 2020 226d 6172 6769            "margi
-0001c230: 6e22 3a20 2231 342e 3234 3930 3022 0a20  n": "14.24900". 
-0001c240: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0001c250: 2020 2020 207d 0a20 2020 2020 2020 2023       }.        #
-0001c260: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-0001c270: 2020 2023 2020 2020 207d 0a20 2020 2020     #     }.     
-0001c280: 2020 2023 0a20 2020 2020 2020 2072 6573     #.        res
-0001c290: 756c 7420 3d20 7365 6c66 2e73 6166 655f  ult = self.safe_
-0001c2a0: 7661 6c75 6528 7265 7370 6f6e 7365 2c20  value(response, 
-0001c2b0: 2772 6573 756c 7427 290a 2020 2020 2020  'result').      
-0001c2c0: 2020 2320 746f 646f 2075 6e69 6679 2070    # todo unify p
-0001c2d0: 6172 7365 506f 7369 7469 6f6e 2f70 6172  arsePosition/par
-0001c2e0: 7365 506f 7369 7469 6f6e 730a 2020 2020  sePositions.    
-0001c2f0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-0001c300: 740a 0a20 2020 2064 6566 2070 6172 7365  t..    def parse
-0001c310: 5f61 6363 6f75 6e74 5f74 7970 6528 7365  _account_type(se
-0001c320: 6c66 2c20 6163 636f 756e 7429 3a0a 2020  lf, account):.  
-0001c330: 2020 2020 2020 6163 636f 756e 7442 7954        accountByT
-0001c340: 7970 6520 3d20 7b0a 2020 2020 2020 2020  ype = {.        
-0001c350: 2020 2020 2773 706f 7427 3a20 2753 706f      'spot': 'Spo
-0001c360: 7420 5761 6c6c 6574 272c 0a20 2020 2020  t Wallet',.     
-0001c370: 2020 2020 2020 2027 7377 6170 273a 2027         'swap': '
-0001c380: 4675 7475 7265 7320 5761 6c6c 6574 272c  Futures Wallet',
-0001c390: 0a20 2020 2020 2020 2020 2020 2027 6675  .            'fu
-0001c3a0: 7475 7265 273a 2027 4675 7475 7265 7320  ture': 'Futures 
-0001c3b0: 5761 6c6c 6574 272c 0a20 2020 2020 2020  Wallet',.       
-0001c3c0: 207d 0a20 2020 2020 2020 2072 6574 7572   }.        retur
-0001c3d0: 6e20 7365 6c66 2e73 6166 655f 7374 7269  n self.safe_stri
-0001c3e0: 6e67 2861 6363 6f75 6e74 4279 5479 7065  ng(accountByType
-0001c3f0: 2c20 6163 636f 756e 742c 2061 6363 6f75  , account, accou
-0001c400: 6e74 290a 0a20 2020 2064 6566 2074 7261  nt)..    def tra
-0001c410: 6e73 6665 725f 6f75 7428 7365 6c66 2c20  nsfer_out(self, 
-0001c420: 636f 6465 3a20 7374 722c 2061 6d6f 756e  code: str, amoun
-0001c430: 742c 2070 6172 616d 733d 7b7d 293a 0a20  t, params={}):. 
-0001c440: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0001c450: 2020 2074 7261 6e73 6665 7220 6672 6f6d     transfer from
-0001c460: 2073 706f 7420 7761 6c6c 6574 2074 6f20   spot wallet to 
-0001c470: 6675 7475 7265 7320 7761 6c6c 6574 0a20  futures wallet. 
-0001c480: 2020 2020 2020 203a 7365 653a 2068 7474         :see: htt
-0001c490: 7073 3a2f 2f64 6f63 732e 6b72 616b 656e  ps://docs.kraken
-0001c4a0: 2e63 6f6d 2f72 6573 742f 2374 6167 2f55  .com/rest/#tag/U
-0001c4b0: 7365 722d 4675 6e64 696e 672f 6f70 6572  ser-Funding/oper
-0001c4c0: 6174 696f 6e2f 7761 6c6c 6574 5472 616e  ation/walletTran
-0001c4d0: 7366 6572 0a20 2020 2020 2020 203a 7061  sfer.        :pa
-0001c4e0: 7261 6d20 7374 7220 636f 6465 3a20 556e  ram str code: Un
-0001c4f0: 6966 6965 6420 6375 7272 656e 6379 2063  ified currency c
-0001c500: 6f64 650a 2020 2020 2020 2020 3a70 6172  ode.        :par
-0001c510: 616d 2066 6c6f 6174 2061 6d6f 756e 743a  am float amount:
-0001c520: 2053 697a 6520 6f66 2074 6865 2074 7261   Size of the tra
-0001c530: 6e73 6665 720a 2020 2020 2020 2020 3a70  nsfer.        :p
-0001c540: 6172 616d 2064 6963 7420 5b70 6172 616d  aram dict [param
-0001c550: 735d 3a20 4578 6368 616e 6765 2073 7065  s]: Exchange spe
-0001c560: 6369 6669 6320 7061 7261 6d65 7465 7273  cific parameters
-0001c570: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-0001c580: 733a 2061 2060 7472 616e 7366 6572 2073  s: a `transfer s
-0001c590: 7472 7563 7475 7265 203c 6874 7470 733a  tructure <https:
-0001c5a0: 2f2f 646f 6373 2e63 6378 742e 636f 6d2f  //docs.ccxt.com/
-0001c5b0: 232f 3f69 643d 7472 616e 7366 6572 2d73  #/?id=transfer-s
-0001c5c0: 7472 7563 7475 7265 3e60 0a20 2020 2020  tructure>`.     
-0001c5d0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-0001c5e0: 6574 7572 6e20 7365 6c66 2e74 7261 6e73  eturn self.trans
-0001c5f0: 6665 7228 636f 6465 2c20 616d 6f75 6e74  fer(code, amount
-0001c600: 2c20 2773 706f 7427 2c20 2773 7761 7027  , 'spot', 'swap'
-0001c610: 2c20 7061 7261 6d73 290a 0a20 2020 2064  , params)..    d
-0001c620: 6566 2074 7261 6e73 6665 7228 7365 6c66  ef transfer(self
-0001c630: 2c20 636f 6465 3a20 7374 722c 2061 6d6f  , code: str, amo
-0001c640: 756e 743a 2066 6c6f 6174 2c20 6672 6f6d  unt: float, from
-0001c650: 4163 636f 756e 743a 2073 7472 2c20 746f  Account: str, to
-0001c660: 4163 636f 756e 743a 2073 7472 2c20 7061  Account: str, pa
-0001c670: 7261 6d73 3d7b 7d29 202d 3e20 5472 616e  rams={}) -> Tran
-0001c680: 7366 6572 456e 7472 793a 0a20 2020 2020  sferEntry:.     
-0001c690: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
-0001c6a0: 7365 653a 2068 7474 7073 3a2f 2f64 6f63  see: https://doc
-0001c6b0: 732e 6b72 616b 656e 2e63 6f6d 2f72 6573  s.kraken.com/res
-0001c6c0: 742f 2374 6167 2f55 7365 722d 4675 6e64  t/#tag/User-Fund
-0001c6d0: 696e 672f 6f70 6572 6174 696f 6e2f 7761  ing/operation/wa
-0001c6e0: 6c6c 6574 5472 616e 7366 6572 0a20 2020  lletTransfer.   
-0001c6f0: 2020 2020 2074 7261 6e73 6665 7273 2063       transfers c
-0001c700: 7572 7265 6e63 6965 7320 6265 7477 6565  urrencies betwee
-0001c710: 6e20 7375 622d 6163 636f 756e 7473 286f  n sub-accounts(o
-0001c720: 6e6c 7920 7370 6f74 2d3e 7377 6170 2064  nly spot->swap d
-0001c730: 6972 6563 7469 6f6e 2069 7320 7375 7070  irection is supp
-0001c740: 6f72 7465 6429 0a20 2020 2020 2020 203a  orted).        :
-0001c750: 7061 7261 6d20 7374 7220 636f 6465 3a20  param str code: 
-0001c760: 556e 6966 6965 6420 6375 7272 656e 6379  Unified currency
-0001c770: 2063 6f64 650a 2020 2020 2020 2020 3a70   code.        :p
-0001c780: 6172 616d 2066 6c6f 6174 2061 6d6f 756e  aram float amoun
-0001c790: 743a 2053 697a 6520 6f66 2074 6865 2074  t: Size of the t
-0001c7a0: 7261 6e73 6665 720a 2020 2020 2020 2020  ransfer.        
-0001c7b0: 3a70 6172 616d 2073 7472 2066 726f 6d41  :param str fromA
-0001c7c0: 6363 6f75 6e74 3a20 2773 706f 7427 206f  ccount: 'spot' o
-0001c7d0: 7220 2753 706f 7420 5761 6c6c 6574 270a  r 'Spot Wallet'.
-0001c7e0: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
-0001c7f0: 7472 2074 6f41 6363 6f75 6e74 3a20 2773  tr toAccount: 's
-0001c800: 7761 7027 206f 7220 2746 7574 7572 6573  wap' or 'Futures
-0001c810: 2057 616c 6c65 7427 0a20 2020 2020 2020   Wallet'.       
-0001c820: 203a 7061 7261 6d20 6469 6374 205b 7061   :param dict [pa
-0001c830: 7261 6d73 5d3a 2045 7863 6861 6e67 6520  rams]: Exchange 
-0001c840: 7370 6563 6966 6963 2070 6172 616d 6574  specific paramet
-0001c850: 6572 730a 2020 2020 2020 2020 3a72 6574  ers.        :ret
-0001c860: 7572 6e73 3a20 6120 6074 7261 6e73 6665  urns: a `transfe
-0001c870: 7220 7374 7275 6374 7572 6520 3c68 7474  r structure <htt
-0001c880: 7073 3a2f 2f64 6f63 732e 6363 7874 2e63  ps://docs.ccxt.c
-0001c890: 6f6d 2f23 2f3f 6964 3d74 7261 6e73 6665  om/#/?id=transfe
-0001c8a0: 722d 7374 7275 6374 7572 653e 600a 2020  r-structure>`.  
-0001c8b0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0001c8c0: 2020 7365 6c66 2e6c 6f61 645f 6d61 726b    self.load_mark
-0001c8d0: 6574 7328 290a 2020 2020 2020 2020 6375  ets().        cu
-0001c8e0: 7272 656e 6379 203d 2073 656c 662e 6375  rrency = self.cu
-0001c8f0: 7272 656e 6379 2863 6f64 6529 0a20 2020  rrency(code).   
-0001c900: 2020 2020 2066 726f 6d41 6363 6f75 6e74       fromAccount
-0001c910: 203d 2073 656c 662e 7061 7273 655f 6163   = self.parse_ac
-0001c920: 636f 756e 745f 7479 7065 2866 726f 6d41  count_type(fromA
-0001c930: 6363 6f75 6e74 290a 2020 2020 2020 2020  ccount).        
-0001c940: 746f 4163 636f 756e 7420 3d20 7365 6c66  toAccount = self
-0001c950: 2e70 6172 7365 5f61 6363 6f75 6e74 5f74  .parse_account_t
-0001c960: 7970 6528 746f 4163 636f 756e 7429 0a20  ype(toAccount). 
-0001c970: 2020 2020 2020 2072 6571 7565 7374 203d         request =
-0001c980: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
-0001c990: 616d 6f75 6e74 273a 2073 656c 662e 6375  amount': self.cu
-0001c9a0: 7272 656e 6379 5f74 6f5f 7072 6563 6973  rrency_to_precis
-0001c9b0: 696f 6e28 636f 6465 2c20 616d 6f75 6e74  ion(code, amount
-0001c9c0: 292c 0a20 2020 2020 2020 2020 2020 2027  ),.            '
-0001c9d0: 6672 6f6d 273a 2066 726f 6d41 6363 6f75  from': fromAccou
-0001c9e0: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
-0001c9f0: 2774 6f27 3a20 746f 4163 636f 756e 742c  'to': toAccount,
-0001ca00: 0a20 2020 2020 2020 2020 2020 2027 6173  .            'as
-0001ca10: 7365 7427 3a20 6375 7272 656e 6379 5b27  set': currency['
-0001ca20: 6964 275d 2c0a 2020 2020 2020 2020 7d0a  id'],.        }.
-0001ca30: 2020 2020 2020 2020 6966 2066 726f 6d41          if fromA
-0001ca40: 6363 6f75 6e74 2021 3d20 2753 706f 7420  ccount != 'Spot 
-0001ca50: 5761 6c6c 6574 273a 0a20 2020 2020 2020  Wallet':.       
-0001ca60: 2020 2020 2072 6169 7365 2042 6164 5265       raise BadRe
-0001ca70: 7175 6573 7428 7365 6c66 2e69 6420 2b20  quest(self.id + 
-0001ca80: 2720 7472 616e 7366 6572 2063 616e 6e6f  ' transfer canno
-0001ca90: 7420 7472 616e 7366 6572 2066 726f 6d20  t transfer from 
-0001caa0: 2720 2b20 6672 6f6d 4163 636f 756e 7420  ' + fromAccount 
-0001cab0: 2b20 2720 746f 2027 202b 2074 6f41 6363  + ' to ' + toAcc
-0001cac0: 6f75 6e74 202b 2027 2e20 5573 6520 6b72  ount + '. Use kr
-0001cad0: 616b 656e 6675 7475 7265 7320 696e 7374  akenfutures inst
-0001cae0: 6561 6420 746f 2074 7261 6e73 6665 7220  ead to transfer 
-0001caf0: 6672 6f6d 2074 6865 2066 7574 7572 6573  from the futures
-0001cb00: 2061 6363 6f75 6e74 2e27 290a 2020 2020   account.').    
-0001cb10: 2020 2020 7265 7370 6f6e 7365 203d 2073      response = s
-0001cb20: 656c 662e 7072 6976 6174 6550 6f73 7457  elf.privatePostW
-0001cb30: 616c 6c65 7454 7261 6e73 6665 7228 7365  alletTransfer(se
-0001cb40: 6c66 2e65 7874 656e 6428 7265 7175 6573  lf.extend(reques
-0001cb50: 742c 2070 6172 616d 7329 290a 2020 2020  t, params)).    
-0001cb60: 2020 2020 230a 2020 2020 2020 2020 2320      #.        # 
-0001cb70: 2020 7b0a 2020 2020 2020 2020 2320 2020    {.        #   
-0001cb80: 2020 2020 2265 7272 6f72 223a 5b0a 2020      "error":[.  
-0001cb90: 2020 2020 2020 2320 2020 2020 2020 5d2c        #       ],
-0001cba0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0001cbb0: 2022 7265 7375 6c74 223a 7b0a 2020 2020   "result":{.    
-0001cbc0: 2020 2020 2320 2020 2020 2020 2020 2022      #          "
-0001cbd0: 7265 6669 6422 3a22 424f 4955 5349 462d  refid":"BOIUSIF-
-0001cbe0: 4d37 444c 4d4e 2d55 585a 3350 3522 0a20  M7DLMN-UXZ3P5". 
-0001cbf0: 2020 2020 2020 2023 2020 2020 2020 207d         #       }
-0001cc00: 0a20 2020 2020 2020 2023 2020 207d 0a20  .        #   }. 
-0001cc10: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
-0001cc20: 2074 7261 6e73 6665 7220 3d20 7365 6c66   transfer = self
-0001cc30: 2e70 6172 7365 5f74 7261 6e73 6665 7228  .parse_transfer(
-0001cc40: 7265 7370 6f6e 7365 2c20 6375 7272 656e  response, curren
-0001cc50: 6379 290a 2020 2020 2020 2020 7265 7475  cy).        retu
-0001cc60: 726e 2073 656c 662e 6578 7465 6e64 2874  rn self.extend(t
-0001cc70: 7261 6e73 6665 722c 207b 0a20 2020 2020  ransfer, {.     
-0001cc80: 2020 2020 2020 2027 616d 6f75 6e74 273a         'amount':
-0001cc90: 2061 6d6f 756e 742c 0a20 2020 2020 2020   amount,.       
-0001cca0: 2020 2020 2027 6672 6f6d 4163 636f 756e       'fromAccoun
-0001ccb0: 7427 3a20 6672 6f6d 4163 636f 756e 742c  t': fromAccount,
-0001ccc0: 0a20 2020 2020 2020 2020 2020 2027 746f  .            'to
-0001ccd0: 4163 636f 756e 7427 3a20 746f 4163 636f  Account': toAcco
-0001cce0: 756e 742c 0a20 2020 2020 2020 207d 290a  unt,.        }).
-0001ccf0: 0a20 2020 2064 6566 2070 6172 7365 5f74  .    def parse_t
-0001cd00: 7261 6e73 6665 7228 7365 6c66 2c20 7472  ransfer(self, tr
-0001cd10: 616e 7366 6572 2c20 6375 7272 656e 6379  ansfer, currency
-0001cd20: 3a20 4375 7272 656e 6379 203d 204e 6f6e  : Currency = Non
-0001cd30: 6529 3a0a 2020 2020 2020 2020 230a 2020  e):.        #.  
-0001cd40: 2020 2020 2020 2320 7472 616e 7366 6572        # transfer
-0001cd50: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
-0001cd60: 2020 2023 2020 2020 7b0a 2020 2020 2020     #    {.      
-0001cd70: 2020 2320 2020 2020 2020 2022 6572 726f    #        "erro
-0001cd80: 7222 3a5b 0a20 2020 2020 2020 2023 2020  r":[.        #  
-0001cd90: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
-0001cda0: 2023 2020 2020 2020 2020 2272 6573 756c   #        "resul
-0001cdb0: 7422 3a7b 0a20 2020 2020 2020 2023 2020  t":{.        #  
-0001cdc0: 2020 2020 2020 2020 2022 7265 6669 6422           "refid"
-0001cdd0: 3a22 424f 4955 5349 462d 4d37 444c 4d4e  :"BOIUSIF-M7DLMN
-0001cde0: 2d55 585a 3350 3522 0a20 2020 2020 2020  -UXZ3P5".       
-0001cdf0: 2023 2020 2020 2020 2020 7d0a 2020 2020   #        }.    
-0001ce00: 2020 2020 2320 2020 207d 0a20 2020 2020      #    }.     
-0001ce10: 2020 2023 0a20 2020 2020 2020 2072 6573     #.        res
-0001ce20: 756c 7420 3d20 7365 6c66 2e73 6166 655f  ult = self.safe_
-0001ce30: 7661 6c75 6528 7472 616e 7366 6572 2c20  value(transfer, 
-0001ce40: 2772 6573 756c 7427 2c20 7b7d 290a 2020  'result', {}).  
-0001ce50: 2020 2020 2020 7265 6669 6420 3d20 7365        refid = se
-0001ce60: 6c66 2e73 6166 655f 7374 7269 6e67 2872  lf.safe_string(r
-0001ce70: 6573 756c 742c 2027 7265 6669 6427 290a  esult, 'refid').
-0001ce80: 2020 2020 2020 2020 7265 7475 726e 207b          return {
-0001ce90: 0a20 2020 2020 2020 2020 2020 2027 696e  .            'in
-0001cea0: 666f 273a 2074 7261 6e73 6665 722c 0a20  fo': transfer,. 
-0001ceb0: 2020 2020 2020 2020 2020 2027 6964 273a             'id':
-0001cec0: 2072 6566 6964 2c0a 2020 2020 2020 2020   refid,.        
-0001ced0: 2020 2020 2774 696d 6573 7461 6d70 273a      'timestamp':
-0001cee0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-0001cef0: 2020 2027 6461 7465 7469 6d65 273a 204e     'datetime': N
-0001cf00: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-0001cf10: 2027 6375 7272 656e 6379 273a 2073 656c   'currency': sel
-0001cf20: 662e 7361 6665 5f73 7472 696e 6728 6375  f.safe_string(cu
-0001cf30: 7272 656e 6379 2c20 2763 6f64 6527 292c  rrency, 'code'),
-0001cf40: 0a20 2020 2020 2020 2020 2020 2027 616d  .            'am
-0001cf50: 6f75 6e74 273a 204e 6f6e 652c 0a20 2020  ount': None,.   
-0001cf60: 2020 2020 2020 2020 2027 6672 6f6d 4163           'fromAc
-0001cf70: 636f 756e 7427 3a20 4e6f 6e65 2c0a 2020  count': None,.  
-0001cf80: 2020 2020 2020 2020 2020 2774 6f41 6363            'toAcc
-0001cf90: 6f75 6e74 273a 204e 6f6e 652c 0a20 2020  ount': None,.   
-0001cfa0: 2020 2020 2020 2020 2027 7374 6174 7573           'status
-0001cfb0: 273a 2027 7375 6365 7373 272c 0a20 2020  ': 'sucess',.   
-0001cfc0: 2020 2020 207d 0a0a 2020 2020 6465 6620       }..    def 
-0001cfd0: 7369 676e 2873 656c 662c 2070 6174 682c  sign(self, path,
-0001cfe0: 2061 7069 3d27 7075 626c 6963 272c 206d   api='public', m
-0001cff0: 6574 686f 643d 2747 4554 272c 2070 6172  ethod='GET', par
-0001d000: 616d 733d 7b7d 2c20 6865 6164 6572 733d  ams={}, headers=
-0001d010: 4e6f 6e65 2c20 626f 6479 3d4e 6f6e 6529  None, body=None)
-0001d020: 3a0a 2020 2020 2020 2020 7572 6c20 3d20  :.        url = 
-0001d030: 272f 2720 2b20 7365 6c66 2e76 6572 7369  '/' + self.versi
-0001d040: 6f6e 202b 2027 2f27 202b 2061 7069 202b  on + '/' + api +
-0001d050: 2027 2f27 202b 2070 6174 680a 2020 2020   '/' + path.    
-0001d060: 2020 2020 6966 2061 7069 203d 3d20 2770      if api == 'p
-0001d070: 7562 6c69 6327 3a0a 2020 2020 2020 2020  ublic':.        
-0001d080: 2020 2020 6966 2070 6172 616d 733a 0a20      if params:. 
-0001d090: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0001d0a0: 2075 726c 656e 636f 6465 4e65 7374 6564   urlencodeNested
-0001d0b0: 2069 7320 7573 6564 2074 6f20 6164 6472   is used to addr
-0001d0c0: 6573 7320 6874 7470 733a 2f2f 6769 7468  ess https://gith
-0001d0d0: 7562 2e63 6f6d 2f63 6378 742f 6363 7874  ub.com/ccxt/ccxt
-0001d0e0: 2f69 7373 7565 732f 3132 3837 320a 2020  /issues/12872.  
-0001d0f0: 2020 2020 2020 2020 2020 2020 2020 7572                ur
-0001d100: 6c20 2b3d 2027 3f27 202b 2073 656c 662e  l += '?' + self.
-0001d110: 7572 6c65 6e63 6f64 655f 6e65 7374 6564  urlencode_nested
-0001d120: 2870 6172 616d 7329 0a20 2020 2020 2020  (params).       
-0001d130: 2065 6c69 6620 6170 6920 3d3d 2027 7072   elif api == 'pr
-0001d140: 6976 6174 6527 3a0a 2020 2020 2020 2020  ivate':.        
-0001d150: 2020 2020 6973 4361 6e63 656c 4f72 6465      isCancelOrde
-0001d160: 7242 6174 6368 203d 2028 7061 7468 203d  rBatch = (path =
-0001d170: 3d20 2743 616e 6365 6c4f 7264 6572 4261  = 'CancelOrderBa
-0001d180: 7463 6827 290a 2020 2020 2020 2020 2020  tch').          
-0001d190: 2020 7365 6c66 2e63 6865 636b 5f72 6571    self.check_req
-0001d1a0: 7569 7265 645f 6372 6564 656e 7469 616c  uired_credential
-0001d1b0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-0001d1c0: 6e6f 6e63 6520 3d20 7374 7228 7365 6c66  nonce = str(self
-0001d1d0: 2e6e 6f6e 6365 2829 290a 2020 2020 2020  .nonce()).      
-0001d1e0: 2020 2020 2020 2320 7572 6c65 6e63 6f64        # urlencod
-0001d1f0: 654e 6573 7465 6420 6973 2075 7365 6420  eNested is used 
-0001d200: 746f 2061 6464 7265 7373 2068 7474 7073  to address https
-0001d210: 3a2f 2f67 6974 6875 622e 636f 6d2f 6363  ://github.com/cc
-0001d220: 7874 2f63 6378 742f 6973 7375 6573 2f31  xt/ccxt/issues/1
-0001d230: 3238 3732 0a20 2020 2020 2020 2020 2020  2872.           
-0001d240: 2069 6620 6973 4361 6e63 656c 4f72 6465   if isCancelOrde
-0001d250: 7242 6174 6368 3a0a 2020 2020 2020 2020  rBatch:.        
-0001d260: 2020 2020 2020 2020 626f 6479 203d 2073          body = s
-0001d270: 656c 662e 6a73 6f6e 2873 656c 662e 6578  elf.json(self.ex
-0001d280: 7465 6e64 287b 276e 6f6e 6365 273a 206e  tend({'nonce': n
-0001d290: 6f6e 6365 7d2c 2070 6172 616d 7329 290a  once}, params)).
-0001d2a0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0001d2b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001d2c0: 2020 626f 6479 203d 2073 656c 662e 7572    body = self.ur
-0001d2d0: 6c65 6e63 6f64 655f 6e65 7374 6564 2873  lencode_nested(s
-0001d2e0: 656c 662e 6578 7465 6e64 287b 276e 6f6e  elf.extend({'non
-0001d2f0: 6365 273a 206e 6f6e 6365 7d2c 2070 6172  ce': nonce}, par
-0001d300: 616d 7329 290a 2020 2020 2020 2020 2020  ams)).          
-0001d310: 2020 6175 7468 203d 2073 656c 662e 656e    auth = self.en
-0001d320: 636f 6465 286e 6f6e 6365 202b 2062 6f64  code(nonce + bod
-0001d330: 7929 0a20 2020 2020 2020 2020 2020 2068  y).            h
-0001d340: 6173 6820 3d20 7365 6c66 2e68 6173 6828  ash = self.hash(
-0001d350: 6175 7468 2c20 2773 6861 3235 3627 2c20  auth, 'sha256', 
-0001d360: 2762 696e 6172 7927 290a 2020 2020 2020  'binary').      
-0001d370: 2020 2020 2020 6269 6e61 7279 203d 2073        binary = s
-0001d380: 656c 662e 656e 636f 6465 2875 726c 290a  elf.encode(url).
-0001d390: 2020 2020 2020 2020 2020 2020 6269 6e68              binh
-0001d3a0: 6173 6820 3d20 7365 6c66 2e62 696e 6172  ash = self.binar
-0001d3b0: 795f 636f 6e63 6174 2862 696e 6172 792c  y_concat(binary,
-0001d3c0: 2068 6173 6829 0a20 2020 2020 2020 2020   hash).         
-0001d3d0: 2020 2073 6563 7265 7420 3d20 7365 6c66     secret = self
-0001d3e0: 2e62 6173 6536 345f 746f 5f62 696e 6172  .base64_to_binar
-0001d3f0: 7928 7365 6c66 2e73 6563 7265 7429 0a20  y(self.secret). 
-0001d400: 2020 2020 2020 2020 2020 2073 6967 6e61             signa
-0001d410: 7475 7265 203d 2073 656c 662e 686d 6163  ture = self.hmac
-0001d420: 2862 696e 6861 7368 2c20 7365 6372 6574  (binhash, secret
-0001d430: 2c20 6861 7368 6c69 622e 7368 6135 3132  , hashlib.sha512
-0001d440: 2c20 2762 6173 6536 3427 290a 2020 2020  , 'base64').    
-0001d450: 2020 2020 2020 2020 6865 6164 6572 7320          headers 
-0001d460: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-0001d470: 2020 2020 2741 5049 2d4b 6579 273a 2073      'API-Key': s
-0001d480: 656c 662e 6170 694b 6579 2c0a 2020 2020  elf.apiKey,.    
-0001d490: 2020 2020 2020 2020 2020 2020 2741 5049              'API
-0001d4a0: 2d53 6967 6e27 3a20 7369 676e 6174 7572  -Sign': signatur
-0001d4b0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0001d4c0: 2020 2023 2027 436f 6e74 656e 742d 5479     # 'Content-Ty
-0001d4d0: 7065 273a 2027 6170 706c 6963 6174 696f  pe': 'applicatio
-0001d4e0: 6e2f 782d 7777 772d 666f 726d 2d75 726c  n/x-www-form-url
-0001d4f0: 656e 636f 6465 6427 2c0a 2020 2020 2020  encoded',.      
-0001d500: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-0001d510: 2020 2020 6966 2069 7343 616e 6365 6c4f      if isCancelO
-0001d520: 7264 6572 4261 7463 683a 0a20 2020 2020  rderBatch:.     
-0001d530: 2020 2020 2020 2020 2020 2068 6561 6465             heade
-0001d540: 7273 5b27 436f 6e74 656e 742d 5479 7065  rs['Content-Type
-0001d550: 275d 203d 2027 6170 706c 6963 6174 696f  '] = 'applicatio
-0001d560: 6e2f 6a73 6f6e 270a 2020 2020 2020 2020  n/json'.        
-0001d570: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0001d580: 2020 2020 2020 2020 2020 6865 6164 6572            header
-0001d590: 735b 2743 6f6e 7465 6e74 2d54 7970 6527  s['Content-Type'
-0001d5a0: 5d20 3d20 2761 7070 6c69 6361 7469 6f6e  ] = 'application
-0001d5b0: 2f78 2d77 7777 2d66 6f72 6d2d 7572 6c65  /x-www-form-urle
-0001d5c0: 6e63 6f64 6564 270a 2020 2020 2020 2020  ncoded'.        
-0001d5d0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0001d5e0: 2020 7572 6c20 3d20 272f 2720 2b20 7061    url = '/' + pa
-0001d5f0: 7468 0a20 2020 2020 2020 2075 726c 203d  th.        url =
-0001d600: 2073 656c 662e 7572 6c73 5b27 6170 6927   self.urls['api'
-0001d610: 5d5b 6170 695d 202b 2075 726c 0a20 2020  ][api] + url.   
-0001d620: 2020 2020 2072 6574 7572 6e20 7b27 7572       return {'ur
-0001d630: 6c27 3a20 7572 6c2c 2027 6d65 7468 6f64  l': url, 'method
-0001d640: 273a 206d 6574 686f 642c 2027 626f 6479  ': method, 'body
-0001d650: 273a 2062 6f64 792c 2027 6865 6164 6572  ': body, 'header
-0001d660: 7327 3a20 6865 6164 6572 737d 0a0a 2020  s': headers}..  
-0001d670: 2020 6465 6620 6e6f 6e63 6528 7365 6c66    def nonce(self
-0001d680: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-0001d690: 6e20 7365 6c66 2e6d 696c 6c69 7365 636f  n self.milliseco
-0001d6a0: 6e64 7328 290a 0a20 2020 2064 6566 2068  nds()..    def h
-0001d6b0: 616e 646c 655f 6572 726f 7273 2873 656c  andle_errors(sel
-0001d6c0: 662c 2063 6f64 652c 2072 6561 736f 6e2c  f, code, reason,
-0001d6d0: 2075 726c 2c20 6d65 7468 6f64 2c20 6865   url, method, he
-0001d6e0: 6164 6572 732c 2062 6f64 792c 2072 6573  aders, body, res
-0001d6f0: 706f 6e73 652c 2072 6571 7565 7374 4865  ponse, requestHe
-0001d700: 6164 6572 732c 2072 6571 7565 7374 426f  aders, requestBo
-0001d710: 6479 293a 0a20 2020 2020 2020 2069 6620  dy):.        if 
-0001d720: 636f 6465 203d 3d20 3532 303a 0a20 2020  code == 520:.   
-0001d730: 2020 2020 2020 2020 2072 6169 7365 2045           raise E
-0001d740: 7863 6861 6e67 654e 6f74 4176 6169 6c61  xchangeNotAvaila
-0001d750: 626c 6528 7365 6c66 2e69 6420 2b20 2720  ble(self.id + ' 
-0001d760: 2720 2b20 7374 7228 636f 6465 2920 2b20  ' + str(code) + 
-0001d770: 2720 2720 2b20 7265 6173 6f6e 290a 2020  ' ' + reason).  
-0001d780: 2020 2020 2020 2320 746f 646f 3a20 7265        # todo: re
-0001d790: 7772 6974 6520 7365 6c66 2066 6f72 2022  write self for "
-0001d7a0: 6272 6f61 6422 2065 7863 6570 7469 6f6e  broad" exception
-0001d7b0: 7320 6d61 7463 6869 6e67 0a20 2020 2020  s matching.     
-0001d7c0: 2020 2069 6620 626f 6479 2e66 696e 6428     if body.find(
-0001d7d0: 2749 6e76 616c 6964 206f 7264 6572 2729  'Invalid order')
-0001d7e0: 203e 3d20 303a 0a20 2020 2020 2020 2020   >= 0:.         
-0001d7f0: 2020 2072 6169 7365 2049 6e76 616c 6964     raise Invalid
-0001d800: 4f72 6465 7228 7365 6c66 2e69 6420 2b20  Order(self.id + 
-0001d810: 2720 2720 2b20 626f 6479 290a 2020 2020  ' ' + body).    
-0001d820: 2020 2020 6966 2062 6f64 792e 6669 6e64      if body.find
-0001d830: 2827 496e 7661 6c69 6420 6e6f 6e63 6527  ('Invalid nonce'
-0001d840: 2920 3e3d 2030 3a0a 2020 2020 2020 2020  ) >= 0:.        
-0001d850: 2020 2020 7261 6973 6520 496e 7661 6c69      raise Invali
-0001d860: 644e 6f6e 6365 2873 656c 662e 6964 202b  dNonce(self.id +
-0001d870: 2027 2027 202b 2062 6f64 7929 0a20 2020   ' ' + body).   
-0001d880: 2020 2020 2069 6620 626f 6479 2e66 696e       if body.fin
-0001d890: 6428 2749 6e73 7566 6669 6369 656e 7420  d('Insufficient 
-0001d8a0: 6675 6e64 7327 2920 3e3d 2030 3a0a 2020  funds') >= 0:.  
-0001d8b0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0001d8c0: 496e 7375 6666 6963 6965 6e74 4675 6e64  InsufficientFund
-0001d8d0: 7328 7365 6c66 2e69 6420 2b20 2720 2720  s(self.id + ' ' 
-0001d8e0: 2b20 626f 6479 290a 2020 2020 2020 2020  + body).        
-0001d8f0: 6966 2062 6f64 792e 6669 6e64 2827 4361  if body.find('Ca
-0001d900: 6e63 656c 2070 656e 6469 6e67 2729 203e  ncel pending') >
-0001d910: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-0001d920: 2072 6169 7365 2043 616e 6365 6c50 656e   raise CancelPen
-0001d930: 6469 6e67 2873 656c 662e 6964 202b 2027  ding(self.id + '
-0001d940: 2027 202b 2062 6f64 7929 0a20 2020 2020   ' + body).     
-0001d950: 2020 2069 6620 626f 6479 2e66 696e 6428     if body.find(
-0001d960: 2749 6e76 616c 6964 2061 7267 756d 656e  'Invalid argumen
-0001d970: 7473 3a76 6f6c 756d 6527 2920 3e3d 2030  ts:volume') >= 0
-0001d980: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-0001d990: 6973 6520 496e 7661 6c69 644f 7264 6572  ise InvalidOrder
-0001d9a0: 2873 656c 662e 6964 202b 2027 2027 202b  (self.id + ' ' +
-0001d9b0: 2062 6f64 7929 0a20 2020 2020 2020 2069   body).        i
-0001d9c0: 6620 626f 6479 2e66 696e 6428 2752 6174  f body.find('Rat
-0001d9d0: 6520 6c69 6d69 7420 6578 6365 6564 6564  e limit exceeded
-0001d9e0: 2729 203e 3d20 303a 0a20 2020 2020 2020  ') >= 0:.       
-0001d9f0: 2020 2020 2072 6169 7365 2052 6174 654c       raise RateL
-0001da00: 696d 6974 4578 6365 6564 6564 2873 656c  imitExceeded(sel
-0001da10: 662e 6964 202b 2027 2027 202b 2062 6f64  f.id + ' ' + bod
-0001da20: 7929 0a20 2020 2020 2020 2069 6620 7265  y).        if re
-0001da30: 7370 6f6e 7365 2069 7320 4e6f 6e65 3a0a  sponse is None:.
-0001da40: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0001da50: 726e 204e 6f6e 650a 2020 2020 2020 2020  rn None.        
-0001da60: 6966 2062 6f64 795b 305d 203d 3d20 277b  if body[0] == '{
-0001da70: 273a 0a20 2020 2020 2020 2020 2020 2069  ':.            i
-0001da80: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
-0001da90: 2872 6573 706f 6e73 652c 2073 7472 293a  (response, str):
-0001daa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001dab0: 2069 6620 2765 7272 6f72 2720 696e 2072   if 'error' in r
-0001dac0: 6573 706f 6e73 653a 0a20 2020 2020 2020  esponse:.       
-0001dad0: 2020 2020 2020 2020 2020 2020 206e 756d               num
-0001dae0: 4572 726f 7273 203d 206c 656e 2872 6573  Errors = len(res
-0001daf0: 706f 6e73 655b 2765 7272 6f72 275d 290a  ponse['error']).
-0001db00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001db10: 2020 2020 6966 206e 756d 4572 726f 7273      if numErrors
-0001db20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001db30: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
-0001db40: 6520 3d20 7365 6c66 2e69 6420 2b20 2720  e = self.id + ' 
-0001db50: 2720 2b20 626f 6479 0a20 2020 2020 2020  ' + body.       
-0001db60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001db70: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-0001db80: 302c 206c 656e 2872 6573 706f 6e73 655b  0, len(response[
-0001db90: 2765 7272 6f72 275d 2929 3a0a 2020 2020  'error'])):.    
-0001dba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dbb0: 2020 2020 2020 2020 6572 726f 7220 3d20          error = 
-0001dbc0: 7265 7370 6f6e 7365 5b27 6572 726f 7227  response['error'
-0001dbd0: 5d5b 695d 0a20 2020 2020 2020 2020 2020  ][i].           
-0001dbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dbf0: 2073 656c 662e 7468 726f 775f 6578 6163   self.throw_exac
-0001dc00: 746c 795f 6d61 7463 6865 645f 6578 6365  tly_matched_exce
-0001dc10: 7074 696f 6e28 7365 6c66 2e65 7863 6570  ption(self.excep
-0001dc20: 7469 6f6e 732c 2065 7272 6f72 2c20 6d65  tions, error, me
-0001dc30: 7373 6167 6529 0a20 2020 2020 2020 2020  ssage).         
-0001dc40: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0001dc50: 6169 7365 2045 7863 6861 6e67 6545 7272  aise ExchangeErr
-0001dc60: 6f72 286d 6573 7361 6765 290a 2020 2020  or(message).    
-0001dc70: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+0001b980: 725b 5d20 5b73 796d 626f 6c73 5d3a 206e  r[] [symbols]: n
+0001b990: 6f74 2075 7365 6420 6279 206b 7261 6b65  ot used by krake
+0001b9a0: 6e20 6665 7463 6850 6f73 6974 696f 6e73  n fetchPositions
+0001b9b0: 2829 0a20 2020 2020 2020 203a 7061 7261  ().        :para
+0001b9c0: 6d20 6469 6374 205b 7061 7261 6d73 5d3a  m dict [params]:
+0001b9d0: 2065 7874 7261 2070 6172 616d 6574 6572   extra parameter
+0001b9e0: 7320 7370 6563 6966 6963 2074 6f20 7468  s specific to th
+0001b9f0: 6520 6578 6368 616e 6765 2041 5049 2065  e exchange API e
+0001ba00: 6e64 706f 696e 740a 2020 2020 2020 2020  ndpoint.        
+0001ba10: 3a72 6574 7572 6e73 2064 6963 745b 5d3a  :returns dict[]:
+0001ba20: 2061 206c 6973 7420 6f66 2060 706f 7369   a list of `posi
+0001ba30: 7469 6f6e 2073 7472 7563 7475 7265 203c  tion structure <
+0001ba40: 6874 7470 733a 2f2f 646f 6373 2e63 6378  https://docs.ccx
+0001ba50: 742e 636f 6d2f 232f 3f69 643d 706f 7369  t.com/#/?id=posi
+0001ba60: 7469 6f6e 2d73 7472 7563 7475 7265 3e60  tion-structure>`
+0001ba70: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0001ba80: 2020 2020 2073 656c 662e 6c6f 6164 5f6d       self.load_m
+0001ba90: 6172 6b65 7473 2829 0a20 2020 2020 2020  arkets().       
+0001baa0: 2072 6571 7565 7374 203d 207b 0a20 2020   request = {.   
+0001bab0: 2020 2020 2020 2020 2023 2027 7478 6964           # 'txid
+0001bac0: 273a 2027 636f 6d6d 6120 6465 6c69 6d69  ': 'comma delimi
+0001bad0: 7465 6420 6c69 7374 206f 6620 7472 616e  ted list of tran
+0001bae0: 7361 6374 696f 6e20 6964 7320 746f 2072  saction ids to r
+0001baf0: 6573 7472 6963 7420 6f75 7470 7574 2074  estrict output t
+0001bb00: 6f27 2c0a 2020 2020 2020 2020 2020 2020  o',.            
+0001bb10: 2764 6f63 616c 6373 273a 2027 7472 7565  'docalcs': 'true
+0001bb20: 272c 2020 2320 7768 6574 6865 7220 6f72  ',  # whether or
+0001bb30: 206e 6f74 2074 6f20 696e 636c 7564 6520   not to include 
+0001bb40: 7072 6f66 6974 2f6c 6f73 7320 6361 6c63  profit/loss calc
+0001bb50: 756c 6174 696f 6e73 0a20 2020 2020 2020  ulations.       
+0001bb60: 2020 2020 2027 636f 6e73 6f6c 6964 6174       'consolidat
+0001bb70: 696f 6e27 3a20 276d 6172 6b65 7427 2c20  ion': 'market', 
+0001bb80: 2023 2077 6861 7420 746f 2063 6f6e 736f   # what to conso
+0001bb90: 6c69 6461 7465 2074 6865 2070 6f73 6974  lidate the posit
+0001bba0: 696f 6e73 2064 6174 6120 6172 6f75 6e64  ions data around
+0001bbb0: 2c20 6d61 726b 6574 2077 696c 6c20 636f  , market will co
+0001bbc0: 6e73 6f6c 6964 6174 6520 706f 7369 7469  nsolidate positi
+0001bbd0: 6f6e 7320 6261 7365 6420 6f6e 206d 6172  ons based on mar
+0001bbe0: 6b65 7420 7061 6972 0a20 2020 2020 2020  ket pair.       
+0001bbf0: 207d 0a20 2020 2020 2020 2072 6573 706f   }.        respo
+0001bc00: 6e73 6520 3d20 7365 6c66 2e70 7269 7661  nse = self.priva
+0001bc10: 7465 506f 7374 4f70 656e 506f 7369 7469  tePostOpenPositi
+0001bc20: 6f6e 7328 7365 6c66 2e65 7874 656e 6428  ons(self.extend(
+0001bc30: 7265 7175 6573 742c 2070 6172 616d 7329  request, params)
+0001bc40: 290a 2020 2020 2020 2020 230a 2020 2020  ).        #.    
+0001bc50: 2020 2020 2320 6e6f 2063 6f6e 736f 6c69      # no consoli
+0001bc60: 6461 7469 6f6e 0a20 2020 2020 2020 2023  dation.        #
+0001bc70: 0a20 2020 2020 2020 2023 2020 2020 207b  .        #     {
+0001bc80: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0001bc90: 2020 2022 6572 726f 7222 3a20 5b5d 2c0a     "error": [],.
+0001bca0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0001bcb0: 2020 2272 6573 756c 7422 3a20 7b0a 2020    "result": {.  
+0001bcc0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0001bcd0: 2020 2020 2754 4755 464d 592d 464c 4553      'TGUFMY-FLES
+0001bce0: 4a2d 5659 4958 334a 273a 207b 0a20 2020  J-VYIX3J': {.   
+0001bcf0: 2020 2020 2023 2020 2020 2020 2020 2020       #          
+0001bd00: 2020 2020 2020 2022 6f72 6465 7274 7869         "ordertxi
+0001bd10: 6422 3a20 224f 334c 524e 552d 5a4b 4447  d": "O3LRNU-ZKDG
+0001bd20: 352d 584e 4344 4652 222c 0a20 2020 2020  5-XNCDFR",.     
+0001bd30: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0001bd40: 2020 2020 2022 706f 7373 7461 7475 7322       "posstatus"
+0001bd50: 3a20 226f 7065 6e22 2c0a 2020 2020 2020  : "open",.      
+0001bd60: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+0001bd70: 2020 2020 2270 6169 7222 3a20 2245 5448      "pair": "ETH
+0001bd80: 5553 4454 222c 0a20 2020 2020 2020 2023  USDT",.        #
+0001bd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bda0: 2022 7469 6d65 223a 2020 3136 3131 3535   "time":  161155
+0001bdb0: 3732 3331 2e34 3538 342c 0a20 2020 2020  7231.4584,.     
+0001bdc0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0001bdd0: 2020 2020 2022 7479 7065 223a 2022 6275       "type": "bu
+0001bde0: 7922 2c0a 2020 2020 2020 2020 2320 2020  y",.        #   
+0001bdf0: 2020 2020 2020 2020 2020 2020 2020 226f                "o
+0001be00: 7264 6572 7479 7065 223a 2022 6d61 726b  rdertype": "mark
+0001be10: 6574 222c 0a20 2020 2020 2020 2023 2020  et",.        #  
+0001be20: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0001be30: 636f 7374 223a 2022 3238 2e34 3938 3030  cost": "28.49800
+0001be40: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
+0001be50: 2020 2020 2020 2020 2020 2020 2022 6665               "fe
+0001be60: 6522 3a20 2230 2e30 3739 3739 222c 0a20  e": "0.07979",. 
+0001be70: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0001be80: 2020 2020 2020 2020 2022 766f 6c22 3a20           "vol": 
+0001be90: 2230 2e30 3230 3030 3030 3022 2c0a 2020  "0.02000000",.  
+0001bea0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0001beb0: 2020 2020 2020 2020 2276 6f6c 5f63 6c6f          "vol_clo
+0001bec0: 7365 6422 3a20 2230 2e30 3030 3030 3030  sed": "0.0000000
+0001bed0: 3022 2c0a 2020 2020 2020 2020 2320 2020  0",.        #   
+0001bee0: 2020 2020 2020 2020 2020 2020 2020 226d                "m
+0001bef0: 6172 6769 6e22 3a20 2231 342e 3234 3930  argin": "14.2490
+0001bf00: 3022 2c0a 2020 2020 2020 2020 2320 2020  0",.        #   
+0001bf10: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+0001bf20: 6572 6d73 223a 2022 302e 3032 3030 2520  erms": "0.0200% 
+0001bf30: 7065 7220 3420 686f 7572 7322 2c0a 2020  per 4 hours",.  
+0001bf40: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0001bf50: 2020 2020 2020 2020 2272 6f6c 6c6f 7665          "rollove
+0001bf60: 7274 6d22 3a20 2231 3631 3135 3731 3633  rtm": "161157163
+0001bf70: 3122 2c0a 2020 2020 2020 2020 2320 2020  1",.        #   
+0001bf80: 2020 2020 2020 2020 2020 2020 2020 226d                "m
+0001bf90: 6973 6322 3a20 2222 2c0a 2020 2020 2020  isc": "",.      
+0001bfa0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+0001bfb0: 2020 2020 226f 666c 6167 7322 3a20 2222      "oflags": ""
+0001bfc0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0001bfd0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+0001bfe0: 2023 2020 2020 2020 2020 207d 0a20 2020   #         }.   
+0001bff0: 2020 2020 2023 2020 2020 207d 0a20 2020       #     }.   
+0001c000: 2020 2020 2023 0a20 2020 2020 2020 2023       #.        #
+0001c010: 2063 6f6e 736f 6c69 6461 7469 6f6e 2062   consolidation b
+0001c020: 7920 6d61 726b 6574 0a20 2020 2020 2020  y market.       
+0001c030: 2023 0a20 2020 2020 2020 2023 2020 2020   #.        #    
+0001c040: 207b 0a20 2020 2020 2020 2023 2020 2020   {.        #    
+0001c050: 2020 2020 2022 6572 726f 7222 3a20 5b5d       "error": []
+0001c060: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
+0001c070: 2020 2020 2272 6573 756c 7422 3a20 5b0a      "result": [.
+0001c080: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0001c090: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+0001c0a0: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+0001c0b0: 2020 2270 6169 7222 3a20 2245 5448 5553    "pair": "ETHUS
+0001c0c0: 4454 222c 0a20 2020 2020 2020 2023 2020  DT",.        #  
+0001c0d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0001c0e0: 706f 7369 7469 6f6e 7322 3a20 2231 222c  positions": "1",
+0001c0f0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0001c100: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+0001c110: 223a 2022 6275 7922 2c0a 2020 2020 2020  ": "buy",.      
+0001c120: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+0001c130: 2020 2020 226c 6576 6572 6167 6522 3a20      "leverage": 
+0001c140: 2232 2e30 3030 3030 222c 0a20 2020 2020  "2.00000",.     
+0001c150: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0001c160: 2020 2020 2022 636f 7374 223a 2022 3238       "cost": "28
+0001c170: 2e34 3938 3030 222c 0a20 2020 2020 2020  .49800",.       
+0001c180: 2023 2020 2020 2020 2020 2020 2020 2020   #              
+0001c190: 2020 2022 6665 6522 3a20 2230 2e30 3739     "fee": "0.079
+0001c1a0: 3739 222c 0a20 2020 2020 2020 2023 2020  79",.        #  
+0001c1b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0001c1c0: 766f 6c22 3a20 2230 2e30 3230 3030 3030  vol": "0.0200000
+0001c1d0: 3022 2c0a 2020 2020 2020 2020 2320 2020  0",.        #   
+0001c1e0: 2020 2020 2020 2020 2020 2020 2020 2276                "v
+0001c1f0: 6f6c 5f63 6c6f 7365 6422 3a20 2230 2e30  ol_closed": "0.0
+0001c200: 3030 3030 3030 3022 2c0a 2020 2020 2020  0000000",.      
+0001c210: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+0001c220: 2020 2020 226d 6172 6769 6e22 3a20 2231      "margin": "1
+0001c230: 342e 3234 3930 3022 0a20 2020 2020 2020  4.24900".       
+0001c240: 2023 2020 2020 2020 2020 2020 2020 207d   #             }
+0001c250: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0001c260: 2020 205d 0a20 2020 2020 2020 2023 2020     ].        #  
+0001c270: 2020 207d 0a20 2020 2020 2020 2023 0a20     }.        #. 
+0001c280: 2020 2020 2020 2073 796d 626f 6c73 203d         symbols =
+0001c290: 2073 656c 662e 6d61 726b 6574 5f73 796d   self.market_sym
+0001c2a0: 626f 6c73 2873 796d 626f 6c73 290a 2020  bols(symbols).  
+0001c2b0: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
+0001c2c0: 656c 662e 7361 6665 5f6c 6973 7428 7265  elf.safe_list(re
+0001c2d0: 7370 6f6e 7365 2c20 2772 6573 756c 7427  sponse, 'result'
+0001c2e0: 290a 2020 2020 2020 2020 7265 7375 6c74  ).        result
+0001c2f0: 7320 3d20 7365 6c66 2e70 6172 7365 5f70  s = self.parse_p
+0001c300: 6f73 6974 696f 6e73 2872 6573 756c 742c  ositions(result,
+0001c310: 2073 796d 626f 6c73 290a 2020 2020 2020   symbols).      
+0001c320: 2020 7265 7475 726e 2073 656c 662e 6669    return self.fi
+0001c330: 6c74 6572 5f62 795f 6172 7261 795f 706f  lter_by_array_po
+0001c340: 7369 7469 6f6e 7328 7265 7375 6c74 732c  sitions(results,
+0001c350: 2027 7379 6d62 6f6c 272c 2073 796d 626f   'symbol', symbo
+0001c360: 6c73 2c20 4661 6c73 6529 0a0a 2020 2020  ls, False)..    
+0001c370: 6465 6620 7061 7273 655f 706f 7369 7469  def parse_positi
+0001c380: 6f6e 2873 656c 662c 2070 6f73 6974 696f  on(self, positio
+0001c390: 6e2c 206d 6172 6b65 743a 204d 6172 6b65  n, market: Marke
+0001c3a0: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
+0001c3b0: 2020 2023 0a20 2020 2020 2020 2023 2020     #.        #  
+0001c3c0: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
+0001c3d0: 2020 2020 2023 2020 2020 2020 2020 2020       #          
+0001c3e0: 2020 2020 2020 2022 7061 6972 223a 2022         "pair": "
+0001c3f0: 4554 4855 5344 5422 2c0a 2020 2020 2020  ETHUSDT",.      
+0001c400: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+0001c410: 2020 2020 2270 6f73 6974 696f 6e73 223a      "positions":
+0001c420: 2022 3122 2c0a 2020 2020 2020 2020 2320   "1",.        # 
+0001c430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c440: 2274 7970 6522 3a20 2262 7579 222c 0a20  "type": "buy",. 
+0001c450: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0001c460: 2020 2020 2020 2020 2022 6c65 7665 7261           "levera
+0001c470: 6765 223a 2022 322e 3030 3030 3022 2c0a  ge": "2.00000",.
+0001c480: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0001c490: 2020 2020 2020 2020 2020 2263 6f73 7422            "cost"
+0001c4a0: 3a20 2232 382e 3439 3830 3022 2c0a 2020  : "28.49800",.  
+0001c4b0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0001c4c0: 2020 2020 2020 2020 2266 6565 223a 2022          "fee": "
+0001c4d0: 302e 3037 3937 3922 2c0a 2020 2020 2020  0.07979",.      
+0001c4e0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+0001c4f0: 2020 2020 2276 6f6c 223a 2022 302e 3032      "vol": "0.02
+0001c500: 3030 3030 3030 222c 0a20 2020 2020 2020  000000",.       
+0001c510: 2023 2020 2020 2020 2020 2020 2020 2020   #              
+0001c520: 2020 2022 766f 6c5f 636c 6f73 6564 223a     "vol_closed":
+0001c530: 2022 302e 3030 3030 3030 3030 222c 0a20   "0.00000000",. 
+0001c540: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0001c550: 2020 2020 2020 2020 2022 6d61 7267 696e           "margin
+0001c560: 223a 2022 3134 2e32 3439 3030 220a 2020  ": "14.24900".  
+0001c570: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0001c580: 2020 2020 7d0a 2020 2020 2020 2020 230a      }.        #.
+0001c590: 2020 2020 2020 2020 6d61 726b 6574 4964          marketId
+0001c5a0: 203d 2073 656c 662e 7361 6665 5f73 7472   = self.safe_str
+0001c5b0: 696e 6728 706f 7369 7469 6f6e 2c20 2770  ing(position, 'p
+0001c5c0: 6169 7227 290a 2020 2020 2020 2020 7261  air').        ra
+0001c5d0: 7753 6964 6520 3d20 7365 6c66 2e73 6166  wSide = self.saf
+0001c5e0: 655f 7374 7269 6e67 2870 6f73 6974 696f  e_string(positio
+0001c5f0: 6e2c 2027 7479 7065 2729 0a20 2020 2020  n, 'type').     
+0001c600: 2020 2073 6964 6520 3d20 276c 6f6e 6727     side = 'long'
+0001c610: 2069 6620 2872 6177 5369 6465 203d 3d20   if (rawSide == 
+0001c620: 2762 7579 2729 2065 6c73 6520 2773 686f  'buy') else 'sho
+0001c630: 7274 270a 2020 2020 2020 2020 7265 7475  rt'.        retu
+0001c640: 726e 2073 656c 662e 7361 6665 5f70 6f73  rn self.safe_pos
+0001c650: 6974 696f 6e28 7b0a 2020 2020 2020 2020  ition({.        
+0001c660: 2020 2020 2769 6e66 6f27 3a20 706f 7369      'info': posi
+0001c670: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
+0001c680: 2020 2769 6427 3a20 4e6f 6e65 2c0a 2020    'id': None,.  
+0001c690: 2020 2020 2020 2020 2020 2773 796d 626f            'symbo
+0001c6a0: 6c27 3a20 7365 6c66 2e73 6166 655f 7379  l': self.safe_sy
+0001c6b0: 6d62 6f6c 286d 6172 6b65 7449 642c 206d  mbol(marketId, m
+0001c6c0: 6172 6b65 7429 2c0a 2020 2020 2020 2020  arket),.        
+0001c6d0: 2020 2020 276e 6f74 696f 6e61 6c27 3a20      'notional': 
+0001c6e0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+0001c6f0: 2020 276d 6172 6769 6e4d 6f64 6527 3a20    'marginMode': 
+0001c700: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+0001c710: 2020 276c 6971 7569 6461 7469 6f6e 5072    'liquidationPr
+0001c720: 6963 6527 3a20 4e6f 6e65 2c0a 2020 2020  ice': None,.    
+0001c730: 2020 2020 2020 2020 2765 6e74 7279 5072          'entryPr
+0001c740: 6963 6527 3a20 4e6f 6e65 2c0a 2020 2020  ice': None,.    
+0001c750: 2020 2020 2020 2020 2775 6e72 6561 6c69          'unreali
+0001c760: 7a65 6450 6e6c 273a 2073 656c 662e 7361  zedPnl': self.sa
+0001c770: 6665 5f6e 756d 6265 7228 706f 7369 7469  fe_number(positi
+0001c780: 6f6e 2c20 276e 6574 2729 2c0a 2020 2020  on, 'net'),.    
+0001c790: 2020 2020 2020 2020 2772 6561 6c69 7a65          'realize
+0001c7a0: 6450 6e6c 273a 204e 6f6e 652c 0a20 2020  dPnl': None,.   
+0001c7b0: 2020 2020 2020 2020 2027 7065 7263 656e           'percen
+0001c7c0: 7461 6765 273a 204e 6f6e 652c 0a20 2020  tage': None,.   
+0001c7d0: 2020 2020 2020 2020 2027 636f 6e74 7261           'contra
+0001c7e0: 6374 7327 3a20 7365 6c66 2e73 6166 655f  cts': self.safe_
+0001c7f0: 6e75 6d62 6572 2870 6f73 6974 696f 6e2c  number(position,
+0001c800: 2027 766f 6c27 292c 0a20 2020 2020 2020   'vol'),.       
+0001c810: 2020 2020 2027 636f 6e74 7261 6374 5369       'contractSi
+0001c820: 7a65 273a 204e 6f6e 652c 0a20 2020 2020  ze': None,.     
+0001c830: 2020 2020 2020 2027 6d61 726b 5072 6963         'markPric
+0001c840: 6527 3a20 4e6f 6e65 2c0a 2020 2020 2020  e': None,.      
+0001c850: 2020 2020 2020 276c 6173 7450 7269 6365        'lastPrice
+0001c860: 273a 204e 6f6e 652c 0a20 2020 2020 2020  ': None,.       
+0001c870: 2020 2020 2027 7369 6465 273a 2073 6964       'side': sid
+0001c880: 652c 0a20 2020 2020 2020 2020 2020 2027  e,.            '
+0001c890: 6865 6467 6564 273a 204e 6f6e 652c 0a20  hedged': None,. 
+0001c8a0: 2020 2020 2020 2020 2020 2027 7469 6d65             'time
+0001c8b0: 7374 616d 7027 3a20 4e6f 6e65 2c0a 2020  stamp': None,.  
+0001c8c0: 2020 2020 2020 2020 2020 2764 6174 6574            'datet
+0001c8d0: 696d 6527 3a20 4e6f 6e65 2c0a 2020 2020  ime': None,.    
+0001c8e0: 2020 2020 2020 2020 276c 6173 7455 7064          'lastUpd
+0001c8f0: 6174 6554 696d 6573 7461 6d70 273a 204e  ateTimestamp': N
+0001c900: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+0001c910: 2027 6d61 696e 7465 6e61 6e63 654d 6172   'maintenanceMar
+0001c920: 6769 6e27 3a20 4e6f 6e65 2c0a 2020 2020  gin': None,.    
+0001c930: 2020 2020 2020 2020 276d 6169 6e74 656e          'mainten
+0001c940: 616e 6365 4d61 7267 696e 5065 7263 656e  anceMarginPercen
+0001c950: 7461 6765 273a 204e 6f6e 652c 0a20 2020  tage': None,.   
+0001c960: 2020 2020 2020 2020 2027 636f 6c6c 6174           'collat
+0001c970: 6572 616c 273a 204e 6f6e 652c 0a20 2020  eral': None,.   
+0001c980: 2020 2020 2020 2020 2027 696e 6974 6961           'initia
+0001c990: 6c4d 6172 6769 6e27 3a20 7365 6c66 2e73  lMargin': self.s
+0001c9a0: 6166 655f 6e75 6d62 6572 2870 6f73 6974  afe_number(posit
+0001c9b0: 696f 6e2c 2027 6d61 7267 696e 2729 2c0a  ion, 'margin'),.
+0001c9c0: 2020 2020 2020 2020 2020 2020 2769 6e69              'ini
+0001c9d0: 7469 616c 4d61 7267 696e 5065 7263 656e  tialMarginPercen
+0001c9e0: 7461 6765 273a 204e 6f6e 652c 0a20 2020  tage': None,.   
+0001c9f0: 2020 2020 2020 2020 2027 6c65 7665 7261           'levera
+0001ca00: 6765 273a 2073 656c 662e 7361 6665 5f6e  ge': self.safe_n
+0001ca10: 756d 6265 7228 706f 7369 7469 6f6e 2c20  umber(position, 
+0001ca20: 276c 6576 6572 6167 6527 292c 0a20 2020  'leverage'),.   
+0001ca30: 2020 2020 2020 2020 2027 6d61 7267 696e           'margin
+0001ca40: 5261 7469 6f27 3a20 4e6f 6e65 2c0a 2020  Ratio': None,.  
+0001ca50: 2020 2020 2020 2020 2020 2773 746f 704c            'stopL
+0001ca60: 6f73 7350 7269 6365 273a 204e 6f6e 652c  ossPrice': None,
+0001ca70: 0a20 2020 2020 2020 2020 2020 2027 7461  .            'ta
+0001ca80: 6b65 5072 6f66 6974 5072 6963 6527 3a20  keProfitPrice': 
+0001ca90: 4e6f 6e65 2c0a 2020 2020 2020 2020 7d29  None,.        })
+0001caa0: 0a0a 2020 2020 6465 6620 7061 7273 655f  ..    def parse_
+0001cab0: 6163 636f 756e 745f 7479 7065 2873 656c  account_type(sel
+0001cac0: 662c 2061 6363 6f75 6e74 293a 0a20 2020  f, account):.   
+0001cad0: 2020 2020 2061 6363 6f75 6e74 4279 5479       accountByTy
+0001cae0: 7065 203d 207b 0a20 2020 2020 2020 2020  pe = {.         
+0001caf0: 2020 2027 7370 6f74 273a 2027 5370 6f74     'spot': 'Spot
+0001cb00: 2057 616c 6c65 7427 2c0a 2020 2020 2020   Wallet',.      
+0001cb10: 2020 2020 2020 2773 7761 7027 3a20 2746        'swap': 'F
+0001cb20: 7574 7572 6573 2057 616c 6c65 7427 2c0a  utures Wallet',.
+0001cb30: 2020 2020 2020 2020 2020 2020 2766 7574              'fut
+0001cb40: 7572 6527 3a20 2746 7574 7572 6573 2057  ure': 'Futures W
+0001cb50: 616c 6c65 7427 2c0a 2020 2020 2020 2020  allet',.        
+0001cb60: 7d0a 2020 2020 2020 2020 7265 7475 726e  }.        return
+0001cb70: 2073 656c 662e 7361 6665 5f73 7472 696e   self.safe_strin
+0001cb80: 6728 6163 636f 756e 7442 7954 7970 652c  g(accountByType,
+0001cb90: 2061 6363 6f75 6e74 2c20 6163 636f 756e   account, accoun
+0001cba0: 7429 0a0a 2020 2020 6465 6620 7472 616e  t)..    def tran
+0001cbb0: 7366 6572 5f6f 7574 2873 656c 662c 2063  sfer_out(self, c
+0001cbc0: 6f64 653a 2073 7472 2c20 616d 6f75 6e74  ode: str, amount
+0001cbd0: 2c20 7061 7261 6d73 3d7b 7d29 3a0a 2020  , params={}):.  
+0001cbe0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0001cbf0: 2020 7472 616e 7366 6572 2066 726f 6d20    transfer from 
+0001cc00: 7370 6f74 2077 616c 6c65 7420 746f 2066  spot wallet to f
+0001cc10: 7574 7572 6573 2077 616c 6c65 740a 2020  utures wallet.  
+0001cc20: 2020 2020 2020 3a73 6565 3a20 6874 7470        :see: http
+0001cc30: 733a 2f2f 646f 6373 2e6b 7261 6b65 6e2e  s://docs.kraken.
+0001cc40: 636f 6d2f 7265 7374 2f23 7461 672f 5573  com/rest/#tag/Us
+0001cc50: 6572 2d46 756e 6469 6e67 2f6f 7065 7261  er-Funding/opera
+0001cc60: 7469 6f6e 2f77 616c 6c65 7454 7261 6e73  tion/walletTrans
+0001cc70: 6665 720a 2020 2020 2020 2020 3a70 6172  fer.        :par
+0001cc80: 616d 2073 7472 2063 6f64 653a 2055 6e69  am str code: Uni
+0001cc90: 6669 6564 2063 7572 7265 6e63 7920 636f  fied currency co
+0001cca0: 6465 0a20 2020 2020 2020 203a 7061 7261  de.        :para
+0001ccb0: 6d20 666c 6f61 7420 616d 6f75 6e74 3a20  m float amount: 
+0001ccc0: 5369 7a65 206f 6620 7468 6520 7472 616e  Size of the tran
+0001ccd0: 7366 6572 0a20 2020 2020 2020 203a 7061  sfer.        :pa
+0001cce0: 7261 6d20 6469 6374 205b 7061 7261 6d73  ram dict [params
+0001ccf0: 5d3a 2045 7863 6861 6e67 6520 7370 6563  ]: Exchange spec
+0001cd00: 6966 6963 2070 6172 616d 6574 6572 730a  ific parameters.
+0001cd10: 2020 2020 2020 2020 3a72 6574 7572 6e73          :returns
+0001cd20: 3a20 6120 6074 7261 6e73 6665 7220 7374  : a `transfer st
+0001cd30: 7275 6374 7572 6520 3c68 7474 7073 3a2f  ructure <https:/
+0001cd40: 2f64 6f63 732e 6363 7874 2e63 6f6d 2f23  /docs.ccxt.com/#
+0001cd50: 2f3f 6964 3d74 7261 6e73 6665 722d 7374  /?id=transfer-st
+0001cd60: 7275 6374 7572 653e 600a 2020 2020 2020  ructure>`.      
+0001cd70: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+0001cd80: 7475 726e 2073 656c 662e 7472 616e 7366  turn self.transf
+0001cd90: 6572 2863 6f64 652c 2061 6d6f 756e 742c  er(code, amount,
+0001cda0: 2027 7370 6f74 272c 2027 7377 6170 272c   'spot', 'swap',
+0001cdb0: 2070 6172 616d 7329 0a0a 2020 2020 6465   params)..    de
+0001cdc0: 6620 7472 616e 7366 6572 2873 656c 662c  f transfer(self,
+0001cdd0: 2063 6f64 653a 2073 7472 2c20 616d 6f75   code: str, amou
+0001cde0: 6e74 3a20 666c 6f61 742c 2066 726f 6d41  nt: float, fromA
+0001cdf0: 6363 6f75 6e74 3a20 7374 722c 2074 6f41  ccount: str, toA
+0001ce00: 6363 6f75 6e74 3a20 7374 722c 2070 6172  ccount: str, par
+0001ce10: 616d 733d 7b7d 2920 2d3e 2054 7261 6e73  ams={}) -> Trans
+0001ce20: 6665 7245 6e74 7279 3a0a 2020 2020 2020  ferEntry:.      
+0001ce30: 2020 2222 220a 2020 2020 2020 2020 3a73    """.        :s
+0001ce40: 6565 3a20 6874 7470 733a 2f2f 646f 6373  ee: https://docs
+0001ce50: 2e6b 7261 6b65 6e2e 636f 6d2f 7265 7374  .kraken.com/rest
+0001ce60: 2f23 7461 672f 5573 6572 2d46 756e 6469  /#tag/User-Fundi
+0001ce70: 6e67 2f6f 7065 7261 7469 6f6e 2f77 616c  ng/operation/wal
+0001ce80: 6c65 7454 7261 6e73 6665 720a 2020 2020  letTransfer.    
+0001ce90: 2020 2020 7472 616e 7366 6572 7320 6375      transfers cu
+0001cea0: 7272 656e 6369 6573 2062 6574 7765 656e  rrencies between
+0001ceb0: 2073 7562 2d61 6363 6f75 6e74 7328 6f6e   sub-accounts(on
+0001cec0: 6c79 2073 706f 742d 3e73 7761 7020 6469  ly spot->swap di
+0001ced0: 7265 6374 696f 6e20 6973 2073 7570 706f  rection is suppo
+0001cee0: 7274 6564 290a 2020 2020 2020 2020 3a70  rted).        :p
+0001cef0: 6172 616d 2073 7472 2063 6f64 653a 2055  aram str code: U
+0001cf00: 6e69 6669 6564 2063 7572 7265 6e63 7920  nified currency 
+0001cf10: 636f 6465 0a20 2020 2020 2020 203a 7061  code.        :pa
+0001cf20: 7261 6d20 666c 6f61 7420 616d 6f75 6e74  ram float amount
+0001cf30: 3a20 5369 7a65 206f 6620 7468 6520 7472  : Size of the tr
+0001cf40: 616e 7366 6572 0a20 2020 2020 2020 203a  ansfer.        :
+0001cf50: 7061 7261 6d20 7374 7220 6672 6f6d 4163  param str fromAc
+0001cf60: 636f 756e 743a 2027 7370 6f74 2720 6f72  count: 'spot' or
+0001cf70: 2027 5370 6f74 2057 616c 6c65 7427 0a20   'Spot Wallet'. 
+0001cf80: 2020 2020 2020 203a 7061 7261 6d20 7374         :param st
+0001cf90: 7220 746f 4163 636f 756e 743a 2027 7377  r toAccount: 'sw
+0001cfa0: 6170 2720 6f72 2027 4675 7475 7265 7320  ap' or 'Futures 
+0001cfb0: 5761 6c6c 6574 270a 2020 2020 2020 2020  Wallet'.        
+0001cfc0: 3a70 6172 616d 2064 6963 7420 5b70 6172  :param dict [par
+0001cfd0: 616d 735d 3a20 4578 6368 616e 6765 2073  ams]: Exchange s
+0001cfe0: 7065 6369 6669 6320 7061 7261 6d65 7465  pecific paramete
+0001cff0: 7273 0a20 2020 2020 2020 203a 7265 7475  rs.        :retu
+0001d000: 726e 733a 2061 2060 7472 616e 7366 6572  rns: a `transfer
+0001d010: 2073 7472 7563 7475 7265 203c 6874 7470   structure <http
+0001d020: 733a 2f2f 646f 6373 2e63 6378 742e 636f  s://docs.ccxt.co
+0001d030: 6d2f 232f 3f69 643d 7472 616e 7366 6572  m/#/?id=transfer
+0001d040: 2d73 7472 7563 7475 7265 3e60 0a20 2020  -structure>`.   
+0001d050: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0001d060: 2073 656c 662e 6c6f 6164 5f6d 6172 6b65   self.load_marke
+0001d070: 7473 2829 0a20 2020 2020 2020 2063 7572  ts().        cur
+0001d080: 7265 6e63 7920 3d20 7365 6c66 2e63 7572  rency = self.cur
+0001d090: 7265 6e63 7928 636f 6465 290a 2020 2020  rency(code).    
+0001d0a0: 2020 2020 6672 6f6d 4163 636f 756e 7420      fromAccount 
+0001d0b0: 3d20 7365 6c66 2e70 6172 7365 5f61 6363  = self.parse_acc
+0001d0c0: 6f75 6e74 5f74 7970 6528 6672 6f6d 4163  ount_type(fromAc
+0001d0d0: 636f 756e 7429 0a20 2020 2020 2020 2074  count).        t
+0001d0e0: 6f41 6363 6f75 6e74 203d 2073 656c 662e  oAccount = self.
+0001d0f0: 7061 7273 655f 6163 636f 756e 745f 7479  parse_account_ty
+0001d100: 7065 2874 6f41 6363 6f75 6e74 290a 2020  pe(toAccount).  
+0001d110: 2020 2020 2020 7265 7175 6573 7420 3d20        request = 
+0001d120: 7b0a 2020 2020 2020 2020 2020 2020 2761  {.            'a
+0001d130: 6d6f 756e 7427 3a20 7365 6c66 2e63 7572  mount': self.cur
+0001d140: 7265 6e63 795f 746f 5f70 7265 6369 7369  rency_to_precisi
+0001d150: 6f6e 2863 6f64 652c 2061 6d6f 756e 7429  on(code, amount)
+0001d160: 2c0a 2020 2020 2020 2020 2020 2020 2766  ,.            'f
+0001d170: 726f 6d27 3a20 6672 6f6d 4163 636f 756e  rom': fromAccoun
+0001d180: 742c 0a20 2020 2020 2020 2020 2020 2027  t,.            '
+0001d190: 746f 273a 2074 6f41 6363 6f75 6e74 2c0a  to': toAccount,.
+0001d1a0: 2020 2020 2020 2020 2020 2020 2761 7373              'ass
+0001d1b0: 6574 273a 2063 7572 7265 6e63 795b 2769  et': currency['i
+0001d1c0: 6427 5d2c 0a20 2020 2020 2020 207d 0a20  d'],.        }. 
+0001d1d0: 2020 2020 2020 2069 6620 6672 6f6d 4163         if fromAc
+0001d1e0: 636f 756e 7420 213d 2027 5370 6f74 2057  count != 'Spot W
+0001d1f0: 616c 6c65 7427 3a0a 2020 2020 2020 2020  allet':.        
+0001d200: 2020 2020 7261 6973 6520 4261 6452 6571      raise BadReq
+0001d210: 7565 7374 2873 656c 662e 6964 202b 2027  uest(self.id + '
+0001d220: 2074 7261 6e73 6665 7220 6361 6e6e 6f74   transfer cannot
+0001d230: 2074 7261 6e73 6665 7220 6672 6f6d 2027   transfer from '
+0001d240: 202b 2066 726f 6d41 6363 6f75 6e74 202b   + fromAccount +
+0001d250: 2027 2074 6f20 2720 2b20 746f 4163 636f   ' to ' + toAcco
+0001d260: 756e 7420 2b20 272e 2055 7365 206b 7261  unt + '. Use kra
+0001d270: 6b65 6e66 7574 7572 6573 2069 6e73 7465  kenfutures inste
+0001d280: 6164 2074 6f20 7472 616e 7366 6572 2066  ad to transfer f
+0001d290: 726f 6d20 7468 6520 6675 7475 7265 7320  rom the futures 
+0001d2a0: 6163 636f 756e 742e 2729 0a20 2020 2020  account.').     
+0001d2b0: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
+0001d2c0: 6c66 2e70 7269 7661 7465 506f 7374 5761  lf.privatePostWa
+0001d2d0: 6c6c 6574 5472 616e 7366 6572 2873 656c  lletTransfer(sel
+0001d2e0: 662e 6578 7465 6e64 2872 6571 7565 7374  f.extend(request
+0001d2f0: 2c20 7061 7261 6d73 2929 0a20 2020 2020  , params)).     
+0001d300: 2020 2023 0a20 2020 2020 2020 2023 2020     #.        #  
+0001d310: 207b 0a20 2020 2020 2020 2023 2020 2020   {.        #    
+0001d320: 2020 2022 6572 726f 7222 3a5b 0a20 2020     "error":[.   
+0001d330: 2020 2020 2023 2020 2020 2020 205d 2c0a       #       ],.
+0001d340: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0001d350: 2272 6573 756c 7422 3a7b 0a20 2020 2020  "result":{.     
+0001d360: 2020 2023 2020 2020 2020 2020 2020 2272     #          "r
+0001d370: 6566 6964 223a 2242 4f49 5553 4946 2d4d  efid":"BOIUSIF-M
+0001d380: 3744 4c4d 4e2d 5558 5a33 5035 220a 2020  7DLMN-UXZ3P5".  
+0001d390: 2020 2020 2020 2320 2020 2020 2020 7d0a        #       }.
+0001d3a0: 2020 2020 2020 2020 2320 2020 7d0a 2020          #   }.  
+0001d3b0: 2020 2020 2020 230a 2020 2020 2020 2020        #.        
+0001d3c0: 7472 616e 7366 6572 203d 2073 656c 662e  transfer = self.
+0001d3d0: 7061 7273 655f 7472 616e 7366 6572 2872  parse_transfer(r
+0001d3e0: 6573 706f 6e73 652c 2063 7572 7265 6e63  esponse, currenc
+0001d3f0: 7929 0a20 2020 2020 2020 2072 6574 7572  y).        retur
+0001d400: 6e20 7365 6c66 2e65 7874 656e 6428 7472  n self.extend(tr
+0001d410: 616e 7366 6572 2c20 7b0a 2020 2020 2020  ansfer, {.      
+0001d420: 2020 2020 2020 2761 6d6f 756e 7427 3a20        'amount': 
+0001d430: 616d 6f75 6e74 2c0a 2020 2020 2020 2020  amount,.        
+0001d440: 2020 2020 2766 726f 6d41 6363 6f75 6e74      'fromAccount
+0001d450: 273a 2066 726f 6d41 6363 6f75 6e74 2c0a  ': fromAccount,.
+0001d460: 2020 2020 2020 2020 2020 2020 2774 6f41              'toA
+0001d470: 6363 6f75 6e74 273a 2074 6f41 6363 6f75  ccount': toAccou
+0001d480: 6e74 2c0a 2020 2020 2020 2020 7d29 0a0a  nt,.        })..
+0001d490: 2020 2020 6465 6620 7061 7273 655f 7472      def parse_tr
+0001d4a0: 616e 7366 6572 2873 656c 662c 2074 7261  ansfer(self, tra
+0001d4b0: 6e73 6665 722c 2063 7572 7265 6e63 793a  nsfer, currency:
+0001d4c0: 2043 7572 7265 6e63 7920 3d20 4e6f 6e65   Currency = None
+0001d4d0: 293a 0a20 2020 2020 2020 2023 0a20 2020  ):.        #.   
+0001d4e0: 2020 2020 2023 2074 7261 6e73 6665 720a       # transfer.
+0001d4f0: 2020 2020 2020 2020 230a 2020 2020 2020          #.      
+0001d500: 2020 2320 2020 207b 0a20 2020 2020 2020    #    {.       
+0001d510: 2023 2020 2020 2020 2020 2265 7272 6f72   #        "error
+0001d520: 223a 5b0a 2020 2020 2020 2020 2320 2020  ":[.        #   
+0001d530: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+0001d540: 2320 2020 2020 2020 2022 7265 7375 6c74  #        "result
+0001d550: 223a 7b0a 2020 2020 2020 2020 2320 2020  ":{.        #   
+0001d560: 2020 2020 2020 2020 2272 6566 6964 223a          "refid":
+0001d570: 2242 4f49 5553 4946 2d4d 3744 4c4d 4e2d  "BOIUSIF-M7DLMN-
+0001d580: 5558 5a33 5035 220a 2020 2020 2020 2020  UXZ3P5".        
+0001d590: 2320 2020 2020 2020 207d 0a20 2020 2020  #        }.     
+0001d5a0: 2020 2023 2020 2020 7d0a 2020 2020 2020     #    }.      
+0001d5b0: 2020 230a 2020 2020 2020 2020 7265 7375    #.        resu
+0001d5c0: 6c74 203d 2073 656c 662e 7361 6665 5f76  lt = self.safe_v
+0001d5d0: 616c 7565 2874 7261 6e73 6665 722c 2027  alue(transfer, '
+0001d5e0: 7265 7375 6c74 272c 207b 7d29 0a20 2020  result', {}).   
+0001d5f0: 2020 2020 2072 6566 6964 203d 2073 656c       refid = sel
+0001d600: 662e 7361 6665 5f73 7472 696e 6728 7265  f.safe_string(re
+0001d610: 7375 6c74 2c20 2772 6566 6964 2729 0a20  sult, 'refid'). 
+0001d620: 2020 2020 2020 2072 6574 7572 6e20 7b0a         return {.
+0001d630: 2020 2020 2020 2020 2020 2020 2769 6e66              'inf
+0001d640: 6f27 3a20 7472 616e 7366 6572 2c0a 2020  o': transfer,.  
+0001d650: 2020 2020 2020 2020 2020 2769 6427 3a20            'id': 
+0001d660: 7265 6669 642c 0a20 2020 2020 2020 2020  refid,.         
+0001d670: 2020 2027 7469 6d65 7374 616d 7027 3a20     'timestamp': 
+0001d680: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+0001d690: 2020 2764 6174 6574 696d 6527 3a20 4e6f    'datetime': No
+0001d6a0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+0001d6b0: 2763 7572 7265 6e63 7927 3a20 7365 6c66  'currency': self
+0001d6c0: 2e73 6166 655f 7374 7269 6e67 2863 7572  .safe_string(cur
+0001d6d0: 7265 6e63 792c 2027 636f 6465 2729 2c0a  rency, 'code'),.
+0001d6e0: 2020 2020 2020 2020 2020 2020 2761 6d6f              'amo
+0001d6f0: 756e 7427 3a20 4e6f 6e65 2c0a 2020 2020  unt': None,.    
+0001d700: 2020 2020 2020 2020 2766 726f 6d41 6363          'fromAcc
+0001d710: 6f75 6e74 273a 204e 6f6e 652c 0a20 2020  ount': None,.   
+0001d720: 2020 2020 2020 2020 2027 746f 4163 636f           'toAcco
+0001d730: 756e 7427 3a20 4e6f 6e65 2c0a 2020 2020  unt': None,.    
+0001d740: 2020 2020 2020 2020 2773 7461 7475 7327          'status'
+0001d750: 3a20 2773 7563 6573 7327 2c0a 2020 2020  : 'sucess',.    
+0001d760: 2020 2020 7d0a 0a20 2020 2064 6566 2073      }..    def s
+0001d770: 6967 6e28 7365 6c66 2c20 7061 7468 2c20  ign(self, path, 
+0001d780: 6170 693d 2770 7562 6c69 6327 2c20 6d65  api='public', me
+0001d790: 7468 6f64 3d27 4745 5427 2c20 7061 7261  thod='GET', para
+0001d7a0: 6d73 3d7b 7d2c 2068 6561 6465 7273 3d4e  ms={}, headers=N
+0001d7b0: 6f6e 652c 2062 6f64 793d 4e6f 6e65 293a  one, body=None):
+0001d7c0: 0a20 2020 2020 2020 2075 726c 203d 2027  .        url = '
+0001d7d0: 2f27 202b 2073 656c 662e 7665 7273 696f  /' + self.versio
+0001d7e0: 6e20 2b20 272f 2720 2b20 6170 6920 2b20  n + '/' + api + 
+0001d7f0: 272f 2720 2b20 7061 7468 0a20 2020 2020  '/' + path.     
+0001d800: 2020 2069 6620 6170 6920 3d3d 2027 7075     if api == 'pu
+0001d810: 626c 6963 273a 0a20 2020 2020 2020 2020  blic':.         
+0001d820: 2020 2069 6620 7061 7261 6d73 3a0a 2020     if params:.  
+0001d830: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0001d840: 7572 6c65 6e63 6f64 654e 6573 7465 6420  urlencodeNested 
+0001d850: 6973 2075 7365 6420 746f 2061 6464 7265  is used to addre
+0001d860: 7373 2068 7474 7073 3a2f 2f67 6974 6875  ss https://githu
+0001d870: 622e 636f 6d2f 6363 7874 2f63 6378 742f  b.com/ccxt/ccxt/
+0001d880: 6973 7375 6573 2f31 3238 3732 0a20 2020  issues/12872.   
+0001d890: 2020 2020 2020 2020 2020 2020 2075 726c               url
+0001d8a0: 202b 3d20 273f 2720 2b20 7365 6c66 2e75   += '?' + self.u
+0001d8b0: 726c 656e 636f 6465 5f6e 6573 7465 6428  rlencode_nested(
+0001d8c0: 7061 7261 6d73 290a 2020 2020 2020 2020  params).        
+0001d8d0: 656c 6966 2061 7069 203d 3d20 2770 7269  elif api == 'pri
+0001d8e0: 7661 7465 273a 0a20 2020 2020 2020 2020  vate':.         
+0001d8f0: 2020 2069 7343 616e 6365 6c4f 7264 6572     isCancelOrder
+0001d900: 4261 7463 6820 3d20 2870 6174 6820 3d3d  Batch = (path ==
+0001d910: 2027 4361 6e63 656c 4f72 6465 7242 6174   'CancelOrderBat
+0001d920: 6368 2729 0a20 2020 2020 2020 2020 2020  ch').           
+0001d930: 2073 656c 662e 6368 6563 6b5f 7265 7175   self.check_requ
+0001d940: 6972 6564 5f63 7265 6465 6e74 6961 6c73  ired_credentials
+0001d950: 2829 0a20 2020 2020 2020 2020 2020 206e  ().            n
+0001d960: 6f6e 6365 203d 2073 7472 2873 656c 662e  once = str(self.
+0001d970: 6e6f 6e63 6528 2929 0a20 2020 2020 2020  nonce()).       
+0001d980: 2020 2020 2023 2075 726c 656e 636f 6465       # urlencode
+0001d990: 4e65 7374 6564 2069 7320 7573 6564 2074  Nested is used t
+0001d9a0: 6f20 6164 6472 6573 7320 6874 7470 733a  o address https:
+0001d9b0: 2f2f 6769 7468 7562 2e63 6f6d 2f63 6378  //github.com/ccx
+0001d9c0: 742f 6363 7874 2f69 7373 7565 732f 3132  t/ccxt/issues/12
+0001d9d0: 3837 320a 2020 2020 2020 2020 2020 2020  872.            
+0001d9e0: 6966 2069 7343 616e 6365 6c4f 7264 6572  if isCancelOrder
+0001d9f0: 4261 7463 683a 0a20 2020 2020 2020 2020  Batch:.         
+0001da00: 2020 2020 2020 2062 6f64 7920 3d20 7365         body = se
+0001da10: 6c66 2e6a 736f 6e28 7365 6c66 2e65 7874  lf.json(self.ext
+0001da20: 656e 6428 7b27 6e6f 6e63 6527 3a20 6e6f  end({'nonce': no
+0001da30: 6e63 657d 2c20 7061 7261 6d73 2929 0a20  nce}, params)). 
+0001da40: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0001da50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001da60: 2062 6f64 7920 3d20 7365 6c66 2e75 726c   body = self.url
+0001da70: 656e 636f 6465 5f6e 6573 7465 6428 7365  encode_nested(se
+0001da80: 6c66 2e65 7874 656e 6428 7b27 6e6f 6e63  lf.extend({'nonc
+0001da90: 6527 3a20 6e6f 6e63 657d 2c20 7061 7261  e': nonce}, para
+0001daa0: 6d73 2929 0a20 2020 2020 2020 2020 2020  ms)).           
+0001dab0: 2061 7574 6820 3d20 7365 6c66 2e65 6e63   auth = self.enc
+0001dac0: 6f64 6528 6e6f 6e63 6520 2b20 626f 6479  ode(nonce + body
+0001dad0: 290a 2020 2020 2020 2020 2020 2020 6861  ).            ha
+0001dae0: 7368 203d 2073 656c 662e 6861 7368 2861  sh = self.hash(a
+0001daf0: 7574 682c 2027 7368 6132 3536 272c 2027  uth, 'sha256', '
+0001db00: 6269 6e61 7279 2729 0a20 2020 2020 2020  binary').       
+0001db10: 2020 2020 2062 696e 6172 7920 3d20 7365       binary = se
+0001db20: 6c66 2e65 6e63 6f64 6528 7572 6c29 0a20  lf.encode(url). 
+0001db30: 2020 2020 2020 2020 2020 2062 696e 6861             binha
+0001db40: 7368 203d 2073 656c 662e 6269 6e61 7279  sh = self.binary
+0001db50: 5f63 6f6e 6361 7428 6269 6e61 7279 2c20  _concat(binary, 
+0001db60: 6861 7368 290a 2020 2020 2020 2020 2020  hash).          
+0001db70: 2020 7365 6372 6574 203d 2073 656c 662e    secret = self.
+0001db80: 6261 7365 3634 5f74 6f5f 6269 6e61 7279  base64_to_binary
+0001db90: 2873 656c 662e 7365 6372 6574 290a 2020  (self.secret).  
+0001dba0: 2020 2020 2020 2020 2020 7369 676e 6174            signat
+0001dbb0: 7572 6520 3d20 7365 6c66 2e68 6d61 6328  ure = self.hmac(
+0001dbc0: 6269 6e68 6173 682c 2073 6563 7265 742c  binhash, secret,
+0001dbd0: 2068 6173 686c 6962 2e73 6861 3531 322c   hashlib.sha512,
+0001dbe0: 2027 6261 7365 3634 2729 0a20 2020 2020   'base64').     
+0001dbf0: 2020 2020 2020 2068 6561 6465 7273 203d         headers =
+0001dc00: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+0001dc10: 2020 2027 4150 492d 4b65 7927 3a20 7365     'API-Key': se
+0001dc20: 6c66 2e61 7069 4b65 792c 0a20 2020 2020  lf.apiKey,.     
+0001dc30: 2020 2020 2020 2020 2020 2027 4150 492d             'API-
+0001dc40: 5369 676e 273a 2073 6967 6e61 7475 7265  Sign': signature
+0001dc50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001dc60: 2020 2320 2743 6f6e 7465 6e74 2d54 7970    # 'Content-Typ
+0001dc70: 6527 3a20 2761 7070 6c69 6361 7469 6f6e  e': 'application
+0001dc80: 2f78 2d77 7777 2d66 6f72 6d2d 7572 6c65  /x-www-form-urle
+0001dc90: 6e63 6f64 6564 272c 0a20 2020 2020 2020  ncoded',.       
+0001dca0: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
+0001dcb0: 2020 2069 6620 6973 4361 6e63 656c 4f72     if isCancelOr
+0001dcc0: 6465 7242 6174 6368 3a0a 2020 2020 2020  derBatch:.      
+0001dcd0: 2020 2020 2020 2020 2020 6865 6164 6572            header
+0001dce0: 735b 2743 6f6e 7465 6e74 2d54 7970 6527  s['Content-Type'
+0001dcf0: 5d20 3d20 2761 7070 6c69 6361 7469 6f6e  ] = 'application
+0001dd00: 2f6a 736f 6e27 0a20 2020 2020 2020 2020  /json'.         
+0001dd10: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0001dd20: 2020 2020 2020 2020 2068 6561 6465 7273           headers
+0001dd30: 5b27 436f 6e74 656e 742d 5479 7065 275d  ['Content-Type']
+0001dd40: 203d 2027 6170 706c 6963 6174 696f 6e2f   = 'application/
+0001dd50: 782d 7777 772d 666f 726d 2d75 726c 656e  x-www-form-urlen
+0001dd60: 636f 6465 6427 0a20 2020 2020 2020 2065  coded'.        e
+0001dd70: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0001dd80: 2075 726c 203d 2027 2f27 202b 2070 6174   url = '/' + pat
+0001dd90: 680a 2020 2020 2020 2020 7572 6c20 3d20  h.        url = 
+0001dda0: 7365 6c66 2e75 726c 735b 2761 7069 275d  self.urls['api']
+0001ddb0: 5b61 7069 5d20 2b20 7572 6c0a 2020 2020  [api] + url.    
+0001ddc0: 2020 2020 7265 7475 726e 207b 2775 726c      return {'url
+0001ddd0: 273a 2075 726c 2c20 276d 6574 686f 6427  ': url, 'method'
+0001dde0: 3a20 6d65 7468 6f64 2c20 2762 6f64 7927  : method, 'body'
+0001ddf0: 3a20 626f 6479 2c20 2768 6561 6465 7273  : body, 'headers
+0001de00: 273a 2068 6561 6465 7273 7d0a 0a20 2020  ': headers}..   
+0001de10: 2064 6566 206e 6f6e 6365 2873 656c 6629   def nonce(self)
+0001de20: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0001de30: 2073 656c 662e 6d69 6c6c 6973 6563 6f6e   self.millisecon
+0001de40: 6473 2829 0a0a 2020 2020 6465 6620 6861  ds()..    def ha
+0001de50: 6e64 6c65 5f65 7272 6f72 7328 7365 6c66  ndle_errors(self
+0001de60: 2c20 636f 6465 2c20 7265 6173 6f6e 2c20  , code, reason, 
+0001de70: 7572 6c2c 206d 6574 686f 642c 2068 6561  url, method, hea
+0001de80: 6465 7273 2c20 626f 6479 2c20 7265 7370  ders, body, resp
+0001de90: 6f6e 7365 2c20 7265 7175 6573 7448 6561  onse, requestHea
+0001dea0: 6465 7273 2c20 7265 7175 6573 7442 6f64  ders, requestBod
+0001deb0: 7929 3a0a 2020 2020 2020 2020 6966 2063  y):.        if c
+0001dec0: 6f64 6520 3d3d 2035 3230 3a0a 2020 2020  ode == 520:.    
+0001ded0: 2020 2020 2020 2020 7261 6973 6520 4578          raise Ex
+0001dee0: 6368 616e 6765 4e6f 7441 7661 696c 6162  changeNotAvailab
+0001def0: 6c65 2873 656c 662e 6964 202b 2027 2027  le(self.id + ' '
+0001df00: 202b 2073 7472 2863 6f64 6529 202b 2027   + str(code) + '
+0001df10: 2027 202b 2072 6561 736f 6e29 0a20 2020   ' + reason).   
+0001df20: 2020 2020 2023 2074 6f64 6f3a 2072 6577       # todo: rew
+0001df30: 7269 7465 2073 656c 6620 666f 7220 2262  rite self for "b
+0001df40: 726f 6164 2220 6578 6365 7074 696f 6e73  road" exceptions
+0001df50: 206d 6174 6368 696e 670a 2020 2020 2020   matching.      
+0001df60: 2020 6966 2062 6f64 792e 6669 6e64 2827    if body.find('
+0001df70: 496e 7661 6c69 6420 6f72 6465 7227 2920  Invalid order') 
+0001df80: 3e3d 2030 3a0a 2020 2020 2020 2020 2020  >= 0:.          
+0001df90: 2020 7261 6973 6520 496e 7661 6c69 644f    raise InvalidO
+0001dfa0: 7264 6572 2873 656c 662e 6964 202b 2027  rder(self.id + '
+0001dfb0: 2027 202b 2062 6f64 7929 0a20 2020 2020   ' + body).     
+0001dfc0: 2020 2069 6620 626f 6479 2e66 696e 6428     if body.find(
+0001dfd0: 2749 6e76 616c 6964 206e 6f6e 6365 2729  'Invalid nonce')
+0001dfe0: 203e 3d20 303a 0a20 2020 2020 2020 2020   >= 0:.         
+0001dff0: 2020 2072 6169 7365 2049 6e76 616c 6964     raise Invalid
+0001e000: 4e6f 6e63 6528 7365 6c66 2e69 6420 2b20  Nonce(self.id + 
+0001e010: 2720 2720 2b20 626f 6479 290a 2020 2020  ' ' + body).    
+0001e020: 2020 2020 6966 2062 6f64 792e 6669 6e64      if body.find
+0001e030: 2827 496e 7375 6666 6963 6965 6e74 2066  ('Insufficient f
+0001e040: 756e 6473 2729 203e 3d20 303a 0a20 2020  unds') >= 0:.   
+0001e050: 2020 2020 2020 2020 2072 6169 7365 2049           raise I
+0001e060: 6e73 7566 6669 6369 656e 7446 756e 6473  nsufficientFunds
+0001e070: 2873 656c 662e 6964 202b 2027 2027 202b  (self.id + ' ' +
+0001e080: 2062 6f64 7929 0a20 2020 2020 2020 2069   body).        i
+0001e090: 6620 626f 6479 2e66 696e 6428 2743 616e  f body.find('Can
+0001e0a0: 6365 6c20 7065 6e64 696e 6727 2920 3e3d  cel pending') >=
+0001e0b0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+0001e0c0: 7261 6973 6520 4361 6e63 656c 5065 6e64  raise CancelPend
+0001e0d0: 696e 6728 7365 6c66 2e69 6420 2b20 2720  ing(self.id + ' 
+0001e0e0: 2720 2b20 626f 6479 290a 2020 2020 2020  ' + body).      
+0001e0f0: 2020 6966 2062 6f64 792e 6669 6e64 2827    if body.find('
+0001e100: 496e 7661 6c69 6420 6172 6775 6d65 6e74  Invalid argument
+0001e110: 733a 766f 6c75 6d65 2729 203e 3d20 303a  s:volume') >= 0:
+0001e120: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+0001e130: 7365 2049 6e76 616c 6964 4f72 6465 7228  se InvalidOrder(
+0001e140: 7365 6c66 2e69 6420 2b20 2720 2720 2b20  self.id + ' ' + 
+0001e150: 626f 6479 290a 2020 2020 2020 2020 6966  body).        if
+0001e160: 2062 6f64 792e 6669 6e64 2827 5261 7465   body.find('Rate
+0001e170: 206c 696d 6974 2065 7863 6565 6465 6427   limit exceeded'
+0001e180: 2920 3e3d 2030 3a0a 2020 2020 2020 2020  ) >= 0:.        
+0001e190: 2020 2020 7261 6973 6520 5261 7465 4c69      raise RateLi
+0001e1a0: 6d69 7445 7863 6565 6465 6428 7365 6c66  mitExceeded(self
+0001e1b0: 2e69 6420 2b20 2720 2720 2b20 626f 6479  .id + ' ' + body
+0001e1c0: 290a 2020 2020 2020 2020 6966 2072 6573  ).        if res
+0001e1d0: 706f 6e73 6520 6973 204e 6f6e 653a 0a20  ponse is None:. 
+0001e1e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0001e1f0: 6e20 4e6f 6e65 0a20 2020 2020 2020 2069  n None.        i
+0001e200: 6620 626f 6479 5b30 5d20 3d3d 2027 7b27  f body[0] == '{'
+0001e210: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0001e220: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
+0001e230: 7265 7370 6f6e 7365 2c20 7374 7229 3a0a  response, str):.
+0001e240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e250: 6966 2027 6572 726f 7227 2069 6e20 7265  if 'error' in re
+0001e260: 7370 6f6e 7365 3a0a 2020 2020 2020 2020  sponse:.        
+0001e270: 2020 2020 2020 2020 2020 2020 6e75 6d45              numE
+0001e280: 7272 6f72 7320 3d20 6c65 6e28 7265 7370  rrors = len(resp
+0001e290: 6f6e 7365 5b27 6572 726f 7227 5d29 0a20  onse['error']). 
+0001e2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e2b0: 2020 2069 6620 6e75 6d45 7272 6f72 733a     if numErrors:
+0001e2c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e2d0: 2020 2020 2020 2020 206d 6573 7361 6765           message
+0001e2e0: 203d 2073 656c 662e 6964 202b 2027 2027   = self.id + ' '
+0001e2f0: 202b 2062 6f64 790a 2020 2020 2020 2020   + body.        
+0001e300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e310: 666f 7220 6920 696e 2072 616e 6765 2830  for i in range(0
+0001e320: 2c20 6c65 6e28 7265 7370 6f6e 7365 5b27  , len(response['
+0001e330: 6572 726f 7227 5d29 293a 0a20 2020 2020  error'])):.     
+0001e340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e350: 2020 2020 2020 2065 7272 6f72 203d 2072         error = r
+0001e360: 6573 706f 6e73 655b 2765 7272 6f72 275d  esponse['error']
+0001e370: 5b69 5d0a 2020 2020 2020 2020 2020 2020  [i].            
+0001e380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e390: 7365 6c66 2e74 6872 6f77 5f65 7861 6374  self.throw_exact
+0001e3a0: 6c79 5f6d 6174 6368 6564 5f65 7863 6570  ly_matched_excep
+0001e3b0: 7469 6f6e 2873 656c 662e 6578 6365 7074  tion(self.except
+0001e3c0: 696f 6e73 2c20 6572 726f 722c 206d 6573  ions, error, mes
+0001e3d0: 7361 6765 290a 2020 2020 2020 2020 2020  sage).          
+0001e3e0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+0001e3f0: 6973 6520 4578 6368 616e 6765 4572 726f  ise ExchangeErro
+0001e400: 7228 6d65 7373 6167 6529 0a20 2020 2020  r(message).     
+0001e410: 2020 2072 6574 7572 6e20 4e6f 6e65 0a       return None.
```

### Comparing `ccxt-4.2.91/ccxt/krakenfutures.py` & `ccxt-4.2.92/ccxt/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/kucoin.py` & `ccxt-4.2.92/ccxt/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/kucoinfutures.py` & `ccxt-4.2.92/ccxt/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/kuna.py` & `ccxt-4.2.92/ccxt/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/latoken.py` & `ccxt-4.2.92/ccxt/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/lbank.py` & `ccxt-4.2.92/ccxt/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/luno.py` & `ccxt-4.2.92/ccxt/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/lykke.py` & `ccxt-4.2.92/ccxt/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/mercado.py` & `ccxt-4.2.92/ccxt/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/mexc.py` & `ccxt-4.2.92/ccxt/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/ndax.py` & `ccxt-4.2.92/ccxt/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/novadax.py` & `ccxt-4.2.92/ccxt/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/oceanex.py` & `ccxt-4.2.92/ccxt/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/okcoin.py` & `ccxt-4.2.92/ccxt/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/okx.py` & `ccxt-4.2.92/ccxt/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/onetrading.py` & `ccxt-4.2.92/ccxt/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/p2b.py` & `ccxt-4.2.92/ccxt/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/paymium.py` & `ccxt-4.2.92/ccxt/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/phemex.py` & `ccxt-4.2.92/ccxt/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/poloniex.py` & `ccxt-4.2.92/ccxt/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/poloniexfutures.py` & `ccxt-4.2.92/ccxt/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/__init__.py` & `ccxt-4.2.92/ccxt/pro/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """CCXT: CryptoCurrency eXchange Trading Library (Async)"""
 
 # ----------------------------------------------------------------------------
 
-__version__ = '4.2.91'
+__version__ = '4.2.92'
 
 # ----------------------------------------------------------------------------
 
 from ccxt.async_support.base.exchange import Exchange  # noqa: F401
 
 # CCXT Pro exchanges (now this is mainly used for importing exchanges in WS tests)
```

### Comparing `ccxt-4.2.91/ccxt/pro/alpaca.py` & `ccxt-4.2.92/ccxt/pro/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/ascendex.py` & `ccxt-4.2.92/ccxt/pro/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/bequant.py` & `ccxt-4.2.92/ccxt/pro/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/binance.py` & `ccxt-4.2.92/ccxt/pro/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/binancecoinm.py` & `ccxt-4.2.92/ccxt/pro/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/binanceus.py` & `ccxt-4.2.92/ccxt/pro/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/binanceusdm.py` & `ccxt-4.2.92/ccxt/pro/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/bingx.py` & `ccxt-4.2.92/ccxt/pro/bingx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/bitcoincom.py` & `ccxt-4.2.92/ccxt/pro/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/bitfinex.py` & `ccxt-4.2.92/ccxt/pro/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/bitfinex2.py` & `ccxt-4.2.92/ccxt/pro/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/bitget.py` & `ccxt-4.2.92/ccxt/pro/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/bithumb.py` & `ccxt-4.2.92/ccxt/pro/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/bitmart.py` & `ccxt-4.2.92/ccxt/pro/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/bitmex.py` & `ccxt-4.2.92/ccxt/pro/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/bitopro.py` & `ccxt-4.2.92/ccxt/pro/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/bitrue.py` & `ccxt-4.2.92/ccxt/pro/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/bitstamp.py` & `ccxt-4.2.92/ccxt/pro/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/bitvavo.py` & `ccxt-4.2.92/ccxt/pro/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/blockchaincom.py` & `ccxt-4.2.92/ccxt/pro/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/bybit.py` & `ccxt-4.2.92/ccxt/pro/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/cex.py` & `ccxt-4.2.92/ccxt/pro/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/coinbase.py` & `ccxt-4.2.92/ccxt/pro/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/coinbaseinternational.py` & `ccxt-4.2.92/ccxt/pro/coinbaseinternational.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/coinbasepro.py` & `ccxt-4.2.92/ccxt/pro/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/coincheck.py` & `ccxt-4.2.92/ccxt/pro/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/coinex.py` & `ccxt-4.2.92/ccxt/pro/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/coinone.py` & `ccxt-4.2.92/ccxt/pro/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/cryptocom.py` & `ccxt-4.2.92/ccxt/pro/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/currencycom.py` & `ccxt-4.2.92/ccxt/pro/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/deribit.py` & `ccxt-4.2.92/ccxt/pro/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/exmo.py` & `ccxt-4.2.92/ccxt/pro/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/gate.py` & `ccxt-4.2.92/ccxt/pro/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/gemini.py` & `ccxt-4.2.92/ccxt/pro/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/hitbtc.py` & `ccxt-4.2.92/ccxt/pro/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/hollaex.py` & `ccxt-4.2.92/ccxt/pro/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/htx.py` & `ccxt-4.2.92/ccxt/pro/htx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/huobijp.py` & `ccxt-4.2.92/ccxt/pro/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/hyperliquid.py` & `ccxt-4.2.92/ccxt/pro/hyperliquid.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/idex.py` & `ccxt-4.2.92/ccxt/pro/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/independentreserve.py` & `ccxt-4.2.92/ccxt/pro/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/kraken.py` & `ccxt-4.2.92/ccxt/pro/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/krakenfutures.py` & `ccxt-4.2.92/ccxt/pro/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/kucoin.py` & `ccxt-4.2.92/ccxt/pro/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/kucoinfutures.py` & `ccxt-4.2.92/ccxt/pro/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/lbank.py` & `ccxt-4.2.92/ccxt/pro/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/luno.py` & `ccxt-4.2.92/ccxt/pro/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/mexc.py` & `ccxt-4.2.92/ccxt/pro/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/ndax.py` & `ccxt-4.2.92/ccxt/pro/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/okcoin.py` & `ccxt-4.2.92/ccxt/pro/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/okx.py` & `ccxt-4.2.92/ccxt/pro/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/onetrading.py` & `ccxt-4.2.92/ccxt/pro/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/p2b.py` & `ccxt-4.2.92/ccxt/pro/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/phemex.py` & `ccxt-4.2.92/ccxt/pro/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/poloniex.py` & `ccxt-4.2.92/ccxt/pro/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/poloniexfutures.py` & `ccxt-4.2.92/ccxt/pro/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/probit.py` & `ccxt-4.2.92/ccxt/pro/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/upbit.py` & `ccxt-4.2.92/ccxt/pro/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/wazirx.py` & `ccxt-4.2.92/ccxt/pro/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/whitebit.py` & `ccxt-4.2.92/ccxt/pro/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/pro/woo.py` & `ccxt-4.2.92/ccxt/pro/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/probit.py` & `ccxt-4.2.92/ccxt/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ecdsa/__init__.py` & `ccxt-4.2.92/ccxt/static_dependencies/ecdsa/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ecdsa/_version.py` & `ccxt-4.2.92/ccxt/static_dependencies/ecdsa/_version.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ecdsa/curves.py` & `ccxt-4.2.92/ccxt/static_dependencies/ecdsa/curves.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ecdsa/der.py` & `ccxt-4.2.92/ccxt/static_dependencies/ecdsa/der.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ecdsa/ecdsa.py` & `ccxt-4.2.92/ccxt/static_dependencies/ecdsa/ecdsa.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ecdsa/ellipticcurve.py` & `ccxt-4.2.92/ccxt/static_dependencies/ecdsa/ellipticcurve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ecdsa/keys.py` & `ccxt-4.2.92/ccxt/static_dependencies/ecdsa/keys.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ecdsa/numbertheory.py` & `ccxt-4.2.92/ccxt/static_dependencies/ecdsa/numbertheory.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ecdsa/rfc6979.py` & `ccxt-4.2.92/ccxt/static_dependencies/ecdsa/rfc6979.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ecdsa/util.py` & `ccxt-4.2.92/ccxt/static_dependencies/ecdsa/util.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/base.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/base.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/codec.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/codec.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/decoding.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/decoding.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/encoding.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/encoding.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/exceptions.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/grammar.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/grammar.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/registry.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/registry.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/abi/utils/numeric.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/abi/utils/numeric.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/account/messages.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/account/messages.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/hexbytes/_utils.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/hexbytes/_utils.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/hexbytes/main.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/hexbytes/main.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/typing/__init__.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/typing/evm.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/typing/evm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/typing/networks.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/typing/networks.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/__init__.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/abi.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/abi.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/address.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/address.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/applicators.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/applicators.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/conversions.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/conversions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/currency.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/currency.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/curried/__init__.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/curried/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/decorators.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/functional.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/functional.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/hexadecimal.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/hexadecimal.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/humanize.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/logging.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/module_loading.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/numeric.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/numeric.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/toolz.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/toolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/types.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/types.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/ethereum/utils/units.py` & `ccxt-4.2.92/ccxt/static_dependencies/ethereum/utils/units.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/keccak/keccak.py` & `ccxt-4.2.92/ccxt/static_dependencies/keccak/keccak.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/msgpack/__init__.py` & `ccxt-4.2.92/ccxt/static_dependencies/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/msgpack/exceptions.py` & `ccxt-4.2.92/ccxt/static_dependencies/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/msgpack/ext.py` & `ccxt-4.2.92/ccxt/static_dependencies/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/msgpack/fallback.py` & `ccxt-4.2.92/ccxt/static_dependencies/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/parsimonious/exceptions.py` & `ccxt-4.2.92/ccxt/static_dependencies/parsimonious/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/parsimonious/expressions.py` & `ccxt-4.2.92/ccxt/static_dependencies/parsimonious/expressions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/parsimonious/grammar.py` & `ccxt-4.2.92/ccxt/static_dependencies/parsimonious/grammar.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/parsimonious/nodes.py` & `ccxt-4.2.92/ccxt/static_dependencies/parsimonious/nodes.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/parsimonious/utils.py` & `ccxt-4.2.92/ccxt/static_dependencies/parsimonious/utils.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/toolz/_signatures.py` & `ccxt-4.2.92/ccxt/static_dependencies/toolz/_signatures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/toolz/_version.py` & `ccxt-4.2.92/ccxt/static_dependencies/toolz/_version.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/toolz/compatibility.py` & `ccxt-4.2.92/ccxt/static_dependencies/toolz/compatibility.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/toolz/curried/__init__.py` & `ccxt-4.2.92/ccxt/static_dependencies/toolz/curried/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/toolz/curried/operator.py` & `ccxt-4.2.92/ccxt/static_dependencies/toolz/curried/operator.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/toolz/dicttoolz.py` & `ccxt-4.2.92/ccxt/static_dependencies/toolz/dicttoolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/toolz/functoolz.py` & `ccxt-4.2.92/ccxt/static_dependencies/toolz/functoolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/toolz/itertoolz.py` & `ccxt-4.2.92/ccxt/static_dependencies/toolz/itertoolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/static_dependencies/toolz/recipes.py` & `ccxt-4.2.92/ccxt/static_dependencies/toolz/recipes.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/__init__.py` & `ccxt-4.2.92/ccxt/test/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_account.py` & `ccxt-4.2.92/ccxt/test/base/test_account.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_balance.py` & `ccxt-4.2.92/ccxt/test/base/test_balance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_borrow_interest.py` & `ccxt-4.2.92/ccxt/test/base/test_borrow_interest.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_borrow_rate.py` & `ccxt-4.2.92/ccxt/test/base/test_borrow_rate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_calculate_fee.py` & `ccxt-4.2.92/ccxt/test/base/test_calculate_fee.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_crypto.py` & `ccxt-4.2.92/ccxt/test/base/test_crypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_currency.py` & `ccxt-4.2.92/ccxt/test/base/test_currency.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_datetime.py` & `ccxt-4.2.92/ccxt/test/base/test_datetime.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_decimal_to_precision.py` & `ccxt-4.2.92/ccxt/test/base/test_decimal_to_precision.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_deep_extend.py` & `ccxt-4.2.92/ccxt/test/base/test_deep_extend.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_deposit_withdrawal.py` & `ccxt-4.2.92/ccxt/test/base/test_deposit_withdrawal.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_exchange_datetime_functions.py` & `ccxt-4.2.92/ccxt/test/base/test_exchange_datetime_functions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_funding_rate_history.py` & `ccxt-4.2.92/ccxt/test/base/test_funding_rate_history.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_last_price.py` & `ccxt-4.2.92/ccxt/test/base/test_last_price.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_ledger_entry.py` & `ccxt-4.2.92/ccxt/test/base/test_ledger_entry.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_ledger_item.py` & `ccxt-4.2.92/ccxt/test/base/test_ledger_item.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_leverage_tier.py` & `ccxt-4.2.92/ccxt/test/base/test_leverage_tier.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_margin_mode.py` & `ccxt-4.2.92/ccxt/test/base/test_margin_mode.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_margin_modification.py` & `ccxt-4.2.92/ccxt/test/base/test_margin_modification.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_market.py` & `ccxt-4.2.92/ccxt/test/base/test_market.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_number.py` & `ccxt-4.2.92/ccxt/test/base/test_number.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_ohlcv.py` & `ccxt-4.2.92/ccxt/test/base/test_ohlcv.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_open_interest.py` & `ccxt-4.2.92/ccxt/test/base/test_open_interest.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_order.py` & `ccxt-4.2.92/ccxt/test/base/test_order.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_order_book.py` & `ccxt-4.2.92/ccxt/test/base/test_order_book.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_position.py` & `ccxt-4.2.92/ccxt/test/base/test_position.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_shared_methods.py` & `ccxt-4.2.92/ccxt/test/base/test_shared_methods.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_status.py` & `ccxt-4.2.92/ccxt/test/base/test_status.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_throttle.py` & `ccxt-4.2.92/ccxt/test/base/test_throttle.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_ticker.py` & `ccxt-4.2.92/ccxt/test/base/test_ticker.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_trade.py` & `ccxt-4.2.92/ccxt/test/base/test_trade.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_trading_fee.py` & `ccxt-4.2.92/ccxt/test/base/test_trading_fee.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/base/test_transaction.py` & `ccxt-4.2.92/ccxt/test/base/test_transaction.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/test_async.py` & `ccxt-4.2.92/ccxt/test/test_async.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/test/test_sync.py` & `ccxt-4.2.92/ccxt/test/test_sync.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/timex.py` & `ccxt-4.2.92/ccxt/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/tokocrypto.py` & `ccxt-4.2.92/ccxt/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/tradeogre.py` & `ccxt-4.2.92/ccxt/tradeogre.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/upbit.py` & `ccxt-4.2.92/ccxt/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/wavesexchange.py` & `ccxt-4.2.92/ccxt/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/wazirx.py` & `ccxt-4.2.92/ccxt/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/whitebit.py` & `ccxt-4.2.92/ccxt/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/woo.py` & `ccxt-4.2.92/ccxt/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/yobit.py` & `ccxt-4.2.92/ccxt/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/zaif.py` & `ccxt-4.2.92/ccxt/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt/zonda.py` & `ccxt-4.2.92/ccxt/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/ccxt.egg-info/PKG-INFO` & `ccxt-4.2.92/ccxt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccxt
-Version: 4.2.91
+Version: 4.2.92
 Summary: A JavaScript / TypeScript / Python / C# / PHP cryptocurrency trading library with support for 100+ exchanges
 Home-page: https://ccxt.com
 Author: Igor Kroitor
 Author-email: igor.kroitor@gmail.com
 License: MIT
 Project-URL: Homepage, https://ccxt.com
 Project-URL: Documentation, https://github.com/ccxt/ccxt/wiki
@@ -221,21 +221,21 @@
         console.log(version, Object.keys(exchanges));
         ```
         
         ### JavaScript (for use with the `<script>` tag):
         
         All-in-one browser bundle (dependencies included), served from a CDN of your choice:
         
-        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@4.2.91/dist/ccxt.browser.js
-        * unpkg: https://unpkg.com/ccxt@4.2.91/dist/ccxt.browser.js
+        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@4.2.92/dist/ccxt.browser.js
+        * unpkg: https://unpkg.com/ccxt@4.2.92/dist/ccxt.browser.js
         
         CDNs are not updated in real-time and may have delays. Defaulting to the most recent version without specifying the version number is not recommended. Please, keep in mind that we are not responsible for the correct operation of those CDN servers.
         
         ```HTML
-        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@4.2.91/dist/ccxt.browser.js"></script>
+        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@4.2.92/dist/ccxt.browser.js"></script>
         ```
         
         Creates a global `ccxt` object:
         
         ```JavaScript
         console.log (ccxt.exchanges) // print all available exchanges
         ```
```

### Comparing `ccxt-4.2.91/ccxt.egg-info/SOURCES.txt` & `ccxt-4.2.92/ccxt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.91/package.json` & `ccxt-4.2.92/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'4.2.92'"}*

```diff
@@ -265,9 +265,9 @@
         "update-links": "node build/update-links",
         "validate-types": "node --loader ts-node/esm build/validate-types.ts",
         "vss": "node build/vss"
     },
     "type": "module",
     "types": "./js/ccxt.d.ts",
     "unpkg": "dist/ccxt.browser.js",
-    "version": "4.2.91"
+    "version": "4.2.92"
 }
```

### Comparing `ccxt-4.2.91/setup.py` & `ccxt-4.2.92/setup.py`

 * *Files identical despite different names*

