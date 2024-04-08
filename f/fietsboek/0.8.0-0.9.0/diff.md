# Comparing `tmp/fietsboek-0.8.0.tar.gz` & `tmp/fietsboek-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fietsboek-0.8.0.tar", max compression
+gzip compressed data, was "fietsboek-0.9.0.tar", max compression
```

## Comparing `fietsboek-0.8.0.tar` & `fietsboek-0.9.0.tar`

### file list

```diff
@@ -1,202 +1,209 @@
--rw-r--r--   0        0        0    34523 2022-07-04 18:57:32.078542 fietsboek-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0     2711 2023-01-25 18:49:03.881246 fietsboek-0.8.0/README.md
--rw-r--r--   0        0        0     6287 2023-04-12 21:05:27.144201 fietsboek-0.8.0/fietsboek/__init__.py
--rw-r--r--   0        0        0     9706 2023-06-02 18:42:21.377174 fietsboek-0.8.0/fietsboek/actions.py
--rw-r--r--   0        0        0     1430 2022-12-13 21:14:10.387413 fietsboek-0.8.0/fietsboek/alembic/env.py
--rw-r--r--   0        0        0      492 2022-06-26 19:26:28.000000 fietsboek-0.8.0/fietsboek/alembic/script.py.mako
--rw-r--r--   0        0        0     7221 2022-12-29 14:02:02.600329 fietsboek-0.8.0/fietsboek/alembic/versions/20220702_1b4b1c179e5a.py
--rw-r--r--   0        0        0     1326 2022-12-29 14:02:02.598329 fietsboek-0.8.0/fietsboek/alembic/versions/20220706_c89d9bdbfa68.py
--rw-r--r--   0        0        0      910 2022-12-29 14:02:02.595329 fietsboek-0.8.0/fietsboek/alembic/versions/20220721_091ce24409fe.py
--rw-r--r--   0        0        0      541 2022-12-29 14:02:02.597329 fietsboek-0.8.0/fietsboek/alembic/versions/20220808_d085998b49ca.py
--rw-r--r--   0        0        0     1418 2022-12-29 14:02:02.596329 fietsboek-0.8.0/fietsboek/alembic/versions/20221214_c939800af428.py
--rw-r--r--   0        0        0      520 2023-03-07 19:07:52.859104 fietsboek-0.8.0/fietsboek/alembic/versions/20230203_3149aa2d0114.py
--rw-r--r--   0        0        0       33 2022-06-26 19:26:28.000000 fietsboek-0.8.0/fietsboek/alembic/versions/README.txt
--rw-r--r--   0        0        0    10094 2023-04-26 15:50:29.247401 fietsboek-0.8.0/fietsboek/config.py
--rw-r--r--   0        0        0     1513 2023-05-31 19:17:03.317788 fietsboek-0.8.0/fietsboek/convert.py
--rw-r--r--   0        0        0    14349 2023-06-02 18:37:35.903419 fietsboek-0.8.0/fietsboek/data.py
--rw-r--r--   0        0        0     2330 2022-12-29 16:02:59.213304 fietsboek-0.8.0/fietsboek/email.py
--rw-r--r--   0        0        0     4056 2023-06-02 18:32:17.215271 fietsboek-0.8.0/fietsboek/hittekaart.py
--rw-r--r--   0        0        0     3698 2023-04-13 18:12:32.568709 fietsboek-0.8.0/fietsboek/jinja2.py
--rw-r--r--   0        0        0    14476 2023-05-31 19:16:57.788790 fietsboek-0.8.0/fietsboek/locale/de/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0    24955 2023-05-31 19:16:57.789790 fietsboek-0.8.0/fietsboek/locale/de/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      484 2022-07-07 11:19:31.236253 fietsboek-0.8.0/fietsboek/locale/de/html/home.html
--rw-r--r--   0        0        0    13505 2023-05-31 19:16:57.789790 fietsboek-0.8.0/fietsboek/locale/en/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0    23949 2023-05-31 19:16:57.790790 fietsboek-0.8.0/fietsboek/locale/en/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      439 2022-07-07 11:17:06.866340 fietsboek-0.8.0/fietsboek/locale/en/html/home.html
--rw-r--r--   0        0        0    20222 2023-05-31 19:16:57.791790 fietsboek-0.8.0/fietsboek/locale/fietslog.pot
--rw-r--r--   0        0        0     4991 2022-12-29 14:02:02.545329 fietsboek-0.8.0/fietsboek/models/__init__.py
--rw-r--r--   0        0        0     1770 2023-06-02 17:51:09.655921 fietsboek-0.8.0/fietsboek/models/badge.py
--rw-r--r--   0        0        0     1427 2023-06-02 17:48:17.227377 fietsboek-0.8.0/fietsboek/models/comment.py
--rw-r--r--   0        0        0     2061 2023-06-02 17:48:00.727228 fietsboek-0.8.0/fietsboek/models/image.py
--rw-r--r--   0        0        0      732 2023-03-07 19:07:19.490784 fietsboek-0.8.0/fietsboek/models/meta.py
--rw-r--r--   0        0        0    29507 2023-06-02 18:40:04.354872 fietsboek-0.8.0/fietsboek/models/track.py
--rw-r--r--   0        0        0    16939 2023-06-02 18:07:29.693912 fietsboek-0.8.0/fietsboek/models/user.py
--rw-r--r--   0        0        0     7386 2023-01-25 17:19:24.857216 fietsboek-0.8.0/fietsboek/pages.py
--rw-r--r--   0        0        0      462 2022-12-13 21:14:10.397413 fietsboek-0.8.0/fietsboek/pshell.py
--rw-r--r--   0        0        0     2848 2023-05-31 19:16:57.792790 fietsboek-0.8.0/fietsboek/routes.py
--rw-r--r--   0        0        0     1707 2023-04-12 21:05:27.149201 fietsboek-0.8.0/fietsboek/scripts/__init__.py
--rw-r--r--   0        0        0     5873 2023-06-02 19:07:31.657561 fietsboek-0.8.0/fietsboek/scripts/fietscron.py
--rw-r--r--   0        0        0    14808 2023-05-31 19:16:44.775795 fietsboek-0.8.0/fietsboek/scripts/fietsctl.py
--rw-r--r--   0        0        0     3663 2022-12-29 14:02:02.535329 fietsboek-0.8.0/fietsboek/security.py
--rw-r--r--   0        0        0     3033 2023-02-06 18:03:03.267372 fietsboek-0.8.0/fietsboek/static/GM_Utils/GPX2GM.css
--rw-r--r--   0        0        0   111993 2023-02-06 18:03:03.270372 fietsboek-0.8.0/fietsboek/static/GM_Utils/GPX2GM.js
--rw-r--r--   0        0        0    32768 2023-02-06 18:03:03.271372 fietsboek-0.8.0/fietsboek/static/GM_Utils/GPX2GM_Defs.js
--rw-r--r--   0        0        0      147 2023-02-06 18:03:03.276372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/Grau256x256.png
--rw-r--r--   0        0        0     7209 2023-02-06 18:03:03.277372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/Loading_icon.gif
--rw-r--r--   0        0        0    17490 2023-02-06 18:03:03.278372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/Loading_icon_V1.gif
--rw-r--r--   0        0        0     1775 2023-02-06 18:03:03.280372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/Loading_icon_V2.gif
--rw-r--r--   0        0        0      877 2023-02-06 18:03:03.284372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/airport.png
--rw-r--r--   0        0        0      698 2023-02-06 18:03:03.285372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/bar.png
--rw-r--r--   0        0        0      873 2023-02-06 18:03:03.285372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/boat.png
--rw-r--r--   0        0        0      624 2023-02-06 18:03:03.286372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/bridge.png
--rw-r--r--   0        0        0      715 2023-02-06 18:03:03.286372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/castle.png
--rw-r--r--   0        0        0      648 2023-02-06 18:03:03.287372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/church2.png
--rw-r--r--   0        0        0      428 2023-02-06 18:03:03.288372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/circle_green.svg
--rw-r--r--   0        0        0      421 2023-02-06 18:03:03.288372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/circle_red.svg
--rw-r--r--   0        0        0     1138 2023-02-06 18:03:03.289372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/cluster.png
--rw-r--r--   0        0        0      604 2023-02-06 18:03:03.290372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/cluster.svg
--rw-r--r--   0        0        0     1050 2023-02-06 18:03:03.291372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/current_location - Kopie.svg
--rw-r--r--   0        0        0     1050 2023-02-06 18:03:03.291372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/current_location.svg
--rw-r--r--   0        0        0     1270 2023-02-06 18:03:03.292372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/cycling.png
--rw-r--r--   0        0        0      780 2023-02-06 18:03:03.292372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/finish.png
--rw-r--r--   0        0        0      482 2023-02-06 18:03:03.293372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/flag.png
--rw-r--r--   0        0        0      428 2023-02-06 18:03:03.293372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/fullscreen_m.svg
--rw-r--r--   0        0        0      410 2023-02-06 18:03:03.295372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/fullscreen_p.svg
--rw-r--r--   0        0        0      710 2023-02-06 18:03:03.295372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/harbor.png
--rw-r--r--   0        0        0     1325 2023-02-06 18:03:03.296372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/hiking.png
--rw-r--r--   0        0        0      309 2023-02-06 18:03:03.296372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/hotel.png
--rw-r--r--   0        0        0      892 2023-02-06 18:03:03.297372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/hotel2.png
--rw-r--r--   0        0        0     3311 2023-02-06 18:03:03.298372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/kreis.png
--rw-r--r--   0        0        0      650 2023-02-06 18:03:03.298372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/library.png
--rw-r--r--   0        0        0      204 2023-02-06 18:03:03.299372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/lupe_m.png
--rw-r--r--   0        0        0      392 2023-02-06 18:03:03.299372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/lupe_m_32.png
--rw-r--r--   0        0        0      200 2023-02-06 18:03:03.300372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/lupe_p.png
--rw-r--r--   0        0        0      405 2023-02-06 18:03:03.300372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/lupe_p_32.png
--rw-r--r--   0        0        0      645 2023-02-06 18:03:03.301372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/marker-icon_bw.png
--rw-r--r--   0        0        0      495 2023-02-06 18:03:03.301372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/marker-icon_bw_41x25.png
--rw-r--r--   0        0        0      345 2023-02-06 18:03:03.302372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/marker-icon_bw_small.png
--rw-r--r--   0        0        0       77 2023-02-06 18:03:03.302372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/marker.gif
--rw-r--r--   0        0        0      699 2023-02-06 18:03:03.303372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/marker.svg
--rw-r--r--   0        0        0      849 2023-02-06 18:03:03.303372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/museum.png
--rw-r--r--   0        0        0     1390 2023-02-06 18:03:03.304372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/panorama.png
--rw-r--r--   0        0        0     1100 2023-02-06 18:03:03.304372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/park.png
--rw-r--r--   0        0        0      545 2023-02-06 18:03:03.305372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/peak.png
--rw-r--r--   0        0        0      720 2023-02-06 18:03:03.305372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/photo.png
--rw-r--r--   0        0        0      642 2023-02-06 18:03:03.306372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/pin_red.png
--rw-r--r--   0        0        0      650 2023-02-06 18:03:03.306372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/pin_red_shadow.png
--rw-r--r--   0        0        0     1003 2023-02-06 18:03:03.307372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/restaurant.png
--rw-r--r--   0        0        0      394 2023-02-06 18:03:03.308372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/scenic.png
--rw-r--r--   0        0        0      770 2023-02-06 18:03:03.308372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/shadow.png
--rw-r--r--   0        0        0      570 2023-02-06 18:03:03.308372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/shadow50.png
--rw-r--r--   0        0        0      643 2023-02-06 18:03:03.309372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/shoppingmall.png
--rw-r--r--   0        0        0      438 2023-02-06 18:03:03.309372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/square_green.svg
--rw-r--r--   0        0        0      431 2023-02-06 18:03:03.310372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/square_red.svg
--rw-r--r--   0        0        0      449 2023-02-06 18:03:03.310372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/start.png
--rw-r--r--   0        0        0      603 2023-02-06 18:03:03.310372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/streckenmarker - Kopie.svg
--rw-r--r--   0        0        0      603 2023-02-06 18:03:03.310372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/streckenmarker.svg
--rw-r--r--   0        0        0      795 2023-02-06 18:03:03.311372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/subway.png
--rw-r--r--   0        0        0      642 2023-02-06 18:03:03.311372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/tent.png
--rw-r--r--   0        0        0      947 2023-02-06 18:03:03.311372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/train.png
--rw-r--r--   0        0        0     1290 2023-02-06 18:03:03.312372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/video.png
--rw-r--r--   0        0        0      626 2023-02-06 18:03:03.312372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/villa.png
--rw-r--r--   0        0        0      657 2023-02-06 18:03:03.312372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/whereami.svg
--rw-r--r--   0        0        0     1121 2023-02-06 18:03:03.313372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/whereami_V1.svg
--rw-r--r--   0        0        0    37589 2023-02-06 18:03:03.314372 fietsboek-0.8.0/fietsboek/static/GM_Utils/gmutils.js
--rw-r--r--   0        0        0     3736 2023-02-06 18:03:03.314372 fietsboek-0.8.0/fietsboek/static/GM_Utils/gra_canvas.js
--rw-r--r--   0        0        0     6095 2023-02-06 18:03:03.314372 fietsboek-0.8.0/fietsboek/static/GM_Utils/gra_svg.js
--rw-r--r--   0        0        0     1259 2022-10-04 14:03:38.000000 fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/images/layers-2x.png
--rw-r--r--   0        0        0      696 2022-10-04 14:03:38.000000 fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/images/layers.png
--rw-r--r--   0        0        0     2464 2022-10-04 14:03:38.000000 fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/images/marker-icon-2x.png
--rw-r--r--   0        0        0     1466 2022-10-04 14:03:38.000000 fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/images/marker-icon.png
--rw-r--r--   0        0        0      618 2022-10-04 14:03:38.000000 fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/images/marker-shadow.png
--rw-r--r--   0        0        0    14670 2022-10-04 14:03:38.000000 fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/leaflet.css
--rw-r--r--   0        0        0   146315 2022-10-04 14:05:32.000000 fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/leaflet.js
--rw-r--r--   0        0        0   223367 2022-10-04 14:05:32.000000 fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/leaflet.js.map
--rw-r--r--   0        0        0    39191 2023-02-06 18:03:03.315372 fietsboek-0.8.0/fietsboek/static/GM_Utils/osmutils.js
--rw-r--r--   0        0        0    20687 2023-02-06 18:03:03.316372 fietsboek-0.8.0/fietsboek/static/GM_Utils/plot.js
--rw-r--r--   0        0        0     3594 2023-02-06 18:03:03.316372 fietsboek-0.8.0/fietsboek/static/GM_Utils/shimg.js
--rw-r--r--   0        0        0    93729 2023-04-24 18:24:31.965712 fietsboek-0.8.0/fietsboek/static/bootstrap-icons.css
--rw-r--r--   0        0        0    80420 2023-04-24 18:24:31.965712 fietsboek-0.8.0/fietsboek/static/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   237950 2023-04-24 18:24:31.966712 fietsboek-0.8.0/fietsboek/static/bootstrap.css
--rw-r--r--   0        0        0    25053 2022-06-30 00:22:45.000000 fietsboek-0.8.0/fietsboek/static/favicon.png
--rw-r--r--   0        0        0    13942 2023-05-15 18:19:43.117312 fietsboek-0.8.0/fietsboek/static/fietsboek.js
--rw-r--r--   0        0        0    11482 2023-05-15 18:19:43.118312 fietsboek-0.8.0/fietsboek/static/fietsboek.js.map
--rw-r--r--   0        0        0   164360 2023-04-24 18:24:31.966712 fietsboek-0.8.0/fietsboek/static/fonts/bootstrap-icons.woff
--rw-r--r--   0        0        0   121340 2023-04-24 18:24:31.966712 fietsboek-0.8.0/fietsboek/static/fonts/bootstrap-icons.woff2
--rw-r--r--   0        0        0    20748 2022-07-04 18:57:32.170543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-300.woff
--rw-r--r--   0        0        0    16812 2022-07-04 18:57:32.170543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-300.woff2
--rw-r--r--   0        0        0    21928 2022-07-04 18:57:32.170543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-300italic.woff
--rw-r--r--   0        0        0    17828 2022-07-04 18:57:32.170543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-300italic.woff2
--rw-r--r--   0        0        0    20772 2022-07-04 18:57:32.171543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-500.woff
--rw-r--r--   0        0        0    16812 2022-07-04 18:57:32.171543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-500.woff2
--rw-r--r--   0        0        0    21868 2022-07-04 18:57:32.171543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-500italic.woff
--rw-r--r--   0        0        0    17896 2022-07-04 18:57:32.171543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-500italic.woff2
--rw-r--r--   0        0        0    20664 2022-07-04 18:57:32.172543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-600.woff
--rw-r--r--   0        0        0    16796 2022-07-04 18:57:32.172543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-600.woff2
--rw-r--r--   0        0        0    21812 2022-07-04 18:57:32.172543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-600italic.woff
--rw-r--r--   0        0        0    17836 2022-07-04 18:57:32.172543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-600italic.woff2
--rw-r--r--   0        0        0    20164 2022-07-04 18:57:32.173543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-700.woff
--rw-r--r--   0        0        0    16360 2022-07-04 18:57:32.173543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-700.woff2
--rw-r--r--   0        0        0    21244 2022-07-04 18:57:32.173543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-700italic.woff
--rw-r--r--   0        0        0    17396 2022-07-04 18:57:32.174543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-700italic.woff2
--rw-r--r--   0        0        0    20656 2022-07-04 18:57:32.174543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-800.woff
--rw-r--r--   0        0        0    16724 2022-07-04 18:57:32.174543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-800.woff2
--rw-r--r--   0        0        0    21520 2022-07-04 18:57:32.175543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-800italic.woff
--rw-r--r--   0        0        0    17704 2022-07-04 18:57:32.175543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-800italic.woff2
--rw-r--r--   0        0        0    21848 2022-07-04 18:57:32.175543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-italic.woff
--rw-r--r--   0        0        0    17816 2022-07-04 18:57:32.176543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-italic.woff2
--rw-r--r--   0        0        0    20704 2022-07-04 18:57:32.176543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-regular.woff
--rw-r--r--   0        0        0    16720 2022-07-04 18:57:32.176543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-regular.woff2
--rw-r--r--   0        0        0     4473 2022-07-04 18:57:32.169543 fietsboek-0.8.0/fietsboek/static/fonts.css
--rw-r--r--   0        0        0    14075 2022-12-13 21:14:10.403414 fietsboek-0.8.0/fietsboek/static/osm-monkeypatch.js
--rw-r--r--   0        0        0     2476 2023-05-31 19:16:44.776795 fietsboek-0.8.0/fietsboek/static/theme.css
--rw-r--r--   0        0        0      650 2023-05-31 19:16:44.776795 fietsboek-0.8.0/fietsboek/static/theme.css.map
--rw-r--r--   0        0        0     4795 2023-06-02 18:35:40.418284 fietsboek-0.8.0/fietsboek/summaries.py
--rw-r--r--   0        0        0      280 2022-06-26 19:26:28.000000 fietsboek-0.8.0/fietsboek/templates/404.jinja2
--rw-r--r--   0        0        0     2056 2022-07-14 14:18:13.964884 fietsboek-0.8.0/fietsboek/templates/admin.jinja2
--rw-r--r--   0        0        0     9969 2023-05-15 18:19:43.120312 fietsboek-0.8.0/fietsboek/templates/browse.jinja2
--rw-r--r--   0        0        0     2628 2022-12-13 21:14:10.405413 fietsboek-0.8.0/fietsboek/templates/create_account.jinja2
--rw-r--r--   0        0        0     8519 2023-03-07 19:07:52.862105 fietsboek-0.8.0/fietsboek/templates/details.jinja2
--rw-r--r--   0        0        0     1055 2022-12-13 21:14:10.410414 fietsboek-0.8.0/fietsboek/templates/edit.jinja2
--rw-r--r--   0        0        0     9803 2023-03-07 19:07:52.863104 fietsboek-0.8.0/fietsboek/templates/edit_form.jinja2
--rw-r--r--   0        0        0     1128 2022-12-13 21:14:10.411414 fietsboek-0.8.0/fietsboek/templates/finish_upload.jinja2
--rw-r--r--   0        0        0     2617 2023-05-31 19:16:44.777795 fietsboek-0.8.0/fietsboek/templates/home.jinja2
--rw-r--r--   0        0        0     6362 2023-05-31 19:16:44.777795 fietsboek-0.8.0/fietsboek/templates/layout.jinja2
--rw-r--r--   0        0        0     1938 2023-05-31 19:16:57.792790 fietsboek-0.8.0/fietsboek/templates/login.jinja2
--rw-r--r--   0        0        0     1479 2022-07-14 14:18:13.965884 fietsboek-0.8.0/fietsboek/templates/password_reset.jinja2
--rw-r--r--   0        0        0     5894 2023-04-13 18:12:32.578709 fietsboek-0.8.0/fietsboek/templates/profile.jinja2
--rw-r--r--   0        0        0      766 2022-07-14 14:18:13.966884 fietsboek-0.8.0/fietsboek/templates/request_password.jinja2
--rw-r--r--   0        0        0      780 2023-05-31 19:16:57.792790 fietsboek-0.8.0/fietsboek/templates/resend_verification.jinja2
--rw-r--r--   0        0        0      171 2022-12-13 21:14:10.413414 fietsboek-0.8.0/fietsboek/templates/static-page.jinja2
--rw-r--r--   0        0        0      603 2022-07-14 14:18:13.966884 fietsboek-0.8.0/fietsboek/templates/upload.jinja2
--rw-r--r--   0        0        0     3832 2023-04-13 18:12:32.579709 fietsboek-0.8.0/fietsboek/templates/user_data.jinja2
--rw-r--r--   0        0        0      318 2022-07-14 14:18:13.966884 fietsboek-0.8.0/fietsboek/templates/util.jinja2
--rw-r--r--   0        0        0     4926 2023-05-22 20:39:44.459891 fietsboek-0.8.0/fietsboek/transformers/__init__.py
--rw-r--r--   0        0        0     4085 2023-04-24 18:24:31.971712 fietsboek-0.8.0/fietsboek/transformers/breaks.py
--rw-r--r--   0        0        0     4456 2023-05-22 20:39:44.460891 fietsboek-0.8.0/fietsboek/transformers/elevation.py
--rw-r--r--   0        0        0    15166 2023-04-12 21:05:27.159201 fietsboek-0.8.0/fietsboek/updater/__init__.py
--rw-r--r--   0        0        0     6574 2023-03-26 20:32:32.915788 fietsboek-0.8.0/fietsboek/updater/cli.py
--rw-r--r--   0        0        0     1087 2022-12-14 21:36:27.533733 fietsboek-0.8.0/fietsboek/updater/script.py
--rw-r--r--   0        0        0     2378 2023-01-10 20:57:15.559281 fietsboek-0.8.0/fietsboek/updater/scripts/upd_20230103_lu8w3rwlz4ddcpms.py
--rw-r--r--   0        0        0      475 2023-01-12 19:33:34.761460 fietsboek-0.8.0/fietsboek/updater/scripts/upd_20230112_v0.5.0.py
--rw-r--r--   0        0        0      465 2023-03-08 18:25:33.078353 fietsboek-0.8.0/fietsboek/updater/scripts/upd_20230308_v0.6.0.py
--rw-r--r--   0        0        0      465 2023-04-24 18:26:24.398858 fietsboek-0.8.0/fietsboek/updater/scripts/upd_20230424_v0.7.0.py
--rw-r--r--   0        0        0      465 2023-06-05 19:05:41.679195 fietsboek-0.8.0/fietsboek/updater/scripts/upd_20230605_v0.8.0.py
--rw-r--r--   0        0        0     2104 2022-12-29 14:02:02.591329 fietsboek-0.8.0/fietsboek/updater/scripts/upd_30ppwg8zi4ujb46f.py
--rw-r--r--   0        0        0      454 2022-12-13 21:14:10.416414 fietsboek-0.8.0/fietsboek/updater/scripts/upd_initial.py
--rw-r--r--   0        0        0      466 2022-12-13 21:14:10.417414 fietsboek-0.8.0/fietsboek/updater/scripts/upd_v0.4.0.py
--rw-r--r--   0        0        0    15418 2023-06-02 18:44:14.706240 fietsboek-0.8.0/fietsboek/util.py
--rw-r--r--   0        0        0        0 2022-06-26 19:26:27.000000 fietsboek-0.8.0/fietsboek/views/__init__.py
--rw-r--r--   0        0        0     2245 2023-05-31 19:16:57.793790 fietsboek-0.8.0/fietsboek/views/account.py
--rw-r--r--   0        0        0     2828 2022-12-29 14:02:02.572329 fietsboek-0.8.0/fietsboek/views/admin.py
--rw-r--r--   0        0        0    15572 2023-06-02 19:14:24.818521 fietsboek-0.8.0/fietsboek/views/browse.py
--rw-r--r--   0        0        0     9500 2023-05-31 19:16:57.793790 fietsboek-0.8.0/fietsboek/views/default.py
--rw-r--r--   0        0        0     7231 2023-05-31 19:16:44.779795 fietsboek-0.8.0/fietsboek/views/detail.py
--rw-r--r--   0        0        0     3553 2023-03-07 19:11:04.652006 fietsboek-0.8.0/fietsboek/views/edit.py
--rw-r--r--   0        0        0      404 2022-12-13 21:14:10.420414 fietsboek-0.8.0/fietsboek/views/notfound.py
--rw-r--r--   0        0        0     7846 2023-05-31 19:16:44.780795 fietsboek-0.8.0/fietsboek/views/profile.py
--rw-r--r--   0        0        0    14574 2023-03-08 18:45:52.332655 fietsboek-0.8.0/fietsboek/views/tileproxy.py
--rw-r--r--   0        0        0     7258 2023-05-31 19:17:03.317788 fietsboek-0.8.0/fietsboek/views/upload.py
--rw-r--r--   0        0        0     5737 2023-04-13 18:12:32.583709 fietsboek-0.8.0/fietsboek/views/user_data.py
--rw-r--r--   0        0        0     2340 2023-06-05 18:56:38.304813 fietsboek-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4677 1970-01-01 00:00:00.000000 fietsboek-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-08 19:04:10.819843 fietsboek-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0     2711 2024-04-08 19:04:10.819843 fietsboek-0.9.0/README.md
+-rw-r--r--   0        0        0     6579 2024-04-08 19:04:10.820843 fietsboek-0.9.0/fietsboek/__init__.py
+-rw-r--r--   0        0        0    10166 2024-04-08 19:04:10.821843 fietsboek-0.9.0/fietsboek/actions.py
+-rw-r--r--   0        0        0     1431 2024-04-08 19:04:10.821843 fietsboek-0.9.0/fietsboek/alembic/env.py
+-rw-r--r--   0        0        0      492 2024-04-08 19:04:10.821843 fietsboek-0.9.0/fietsboek/alembic/script.py.mako
+-rw-r--r--   0        0        0     7221 2024-04-08 19:04:10.821843 fietsboek-0.9.0/fietsboek/alembic/versions/20220702_1b4b1c179e5a.py
+-rw-r--r--   0        0        0     1326 2024-04-08 19:04:10.821843 fietsboek-0.9.0/fietsboek/alembic/versions/20220706_c89d9bdbfa68.py
+-rw-r--r--   0        0        0      910 2024-04-08 19:04:10.821843 fietsboek-0.9.0/fietsboek/alembic/versions/20220721_091ce24409fe.py
+-rw-r--r--   0        0        0      541 2024-04-08 19:04:10.821843 fietsboek-0.9.0/fietsboek/alembic/versions/20220808_d085998b49ca.py
+-rw-r--r--   0        0        0     1418 2024-04-08 19:04:10.821843 fietsboek-0.9.0/fietsboek/alembic/versions/20221214_c939800af428.py
+-rw-r--r--   0        0        0      520 2024-04-08 19:04:10.821843 fietsboek-0.9.0/fietsboek/alembic/versions/20230203_3149aa2d0114.py
+-rw-r--r--   0        0        0     1069 2024-04-08 19:04:10.821843 fietsboek-0.9.0/fietsboek/alembic/versions/20230830_8f4e4eae5eb2.py
+-rw-r--r--   0        0        0     1062 2024-04-08 19:04:10.821843 fietsboek-0.9.0/fietsboek/alembic/versions/20230914_4566843039d6.py
+-rw-r--r--   0        0        0       33 2024-04-08 19:04:10.821843 fietsboek-0.9.0/fietsboek/alembic/versions/README.txt
+-rw-r--r--   0        0        0    10416 2024-04-08 19:04:10.821843 fietsboek-0.9.0/fietsboek/config.py
+-rw-r--r--   0        0        0     1514 2024-04-08 19:04:10.821843 fietsboek-0.9.0/fietsboek/convert.py
+-rw-r--r--   0        0        0    14552 2024-04-08 19:04:10.821843 fietsboek-0.9.0/fietsboek/data.py
+-rw-r--r--   0        0        0     2331 2024-04-08 19:04:10.821843 fietsboek-0.9.0/fietsboek/email.py
+-rw-r--r--   0        0        0     4098 2024-04-08 19:04:10.821843 fietsboek-0.9.0/fietsboek/hittekaart.py
+-rw-r--r--   0        0        0     4056 2024-04-08 19:04:10.821843 fietsboek-0.9.0/fietsboek/jinja2.py
+-rw-r--r--   0        0        0       17 2024-04-08 19:04:10.821843 fietsboek-0.9.0/fietsboek/locale/de/DISPLAY_NAME
+-rw-r--r--   0        0        0    15685 2024-04-08 19:04:10.821843 fietsboek-0.9.0/fietsboek/locale/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    26780 2024-04-08 19:04:10.821843 fietsboek-0.9.0/fietsboek/locale/de/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      484 2024-04-08 19:04:10.821843 fietsboek-0.9.0/fietsboek/locale/de/html/home.html
+-rw-r--r--   0        0        0       17 2024-04-08 19:04:10.821843 fietsboek-0.9.0/fietsboek/locale/en/DISPLAY_NAME
+-rw-r--r--   0        0        0    14656 2024-04-08 19:04:10.821843 fietsboek-0.9.0/fietsboek/locale/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    25719 2024-04-08 19:04:10.821843 fietsboek-0.9.0/fietsboek/locale/en/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      439 2024-04-08 19:04:10.822843 fietsboek-0.9.0/fietsboek/locale/en/html/home.html
+-rw-r--r--   0        0        0    21507 2024-04-08 19:04:10.822843 fietsboek-0.9.0/fietsboek/locale/fietslog.pot
+-rw-r--r--   0        0        0     4992 2024-04-08 19:04:10.822843 fietsboek-0.9.0/fietsboek/models/__init__.py
+-rw-r--r--   0        0        0     1771 2024-04-08 19:04:10.822843 fietsboek-0.9.0/fietsboek/models/badge.py
+-rw-r--r--   0        0        0     1428 2024-04-08 19:04:10.822843 fietsboek-0.9.0/fietsboek/models/comment.py
+-rw-r--r--   0        0        0     2062 2024-04-08 19:04:10.822843 fietsboek-0.9.0/fietsboek/models/image.py
+-rw-r--r--   0        0        0      733 2024-04-08 19:04:10.822843 fietsboek-0.9.0/fietsboek/models/meta.py
+-rw-r--r--   0        0        0    30690 2024-04-08 19:04:10.822843 fietsboek-0.9.0/fietsboek/models/track.py
+-rw-r--r--   0        0        0    20168 2024-04-08 19:04:10.822843 fietsboek-0.9.0/fietsboek/models/user.py
+-rw-r--r--   0        0        0     7387 2024-04-08 19:04:10.822843 fietsboek-0.9.0/fietsboek/pages.py
+-rw-r--r--   0        0        0      463 2024-04-08 19:04:10.822843 fietsboek-0.9.0/fietsboek/pshell.py
+-rw-r--r--   0        0        0     3043 2024-04-08 19:04:10.822843 fietsboek-0.9.0/fietsboek/routes.py
+-rw-r--r--   0        0        0     1708 2024-04-08 19:04:10.822843 fietsboek-0.9.0/fietsboek/scripts/__init__.py
+-rw-r--r--   0        0        0     5874 2024-04-08 19:04:10.822843 fietsboek-0.9.0/fietsboek/scripts/fietscron.py
+-rw-r--r--   0        0        0    15457 2024-04-08 19:04:10.822843 fietsboek-0.9.0/fietsboek/scripts/fietsctl.py
+-rw-r--r--   0        0        0     3602 2024-04-08 19:04:10.822843 fietsboek-0.9.0/fietsboek/security.py
+-rw-r--r--   0        0        0     3033 2024-04-08 19:04:10.822843 fietsboek-0.9.0/fietsboek/static/GM_Utils/GPX2GM.css
+-rw-r--r--   0        0        0   111993 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/GPX2GM.js
+-rw-r--r--   0        0        0    32768 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/GPX2GM_Defs.js
+-rw-r--r--   0        0        0      147 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/Grau256x256.png
+-rw-r--r--   0        0        0     7209 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/Loading_icon.gif
+-rw-r--r--   0        0        0    17490 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/Loading_icon_V1.gif
+-rw-r--r--   0        0        0     1775 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/Loading_icon_V2.gif
+-rw-r--r--   0        0        0      877 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/airport.png
+-rw-r--r--   0        0        0      698 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/bar.png
+-rw-r--r--   0        0        0      873 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/boat.png
+-rw-r--r--   0        0        0      624 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/bridge.png
+-rw-r--r--   0        0        0      715 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/castle.png
+-rw-r--r--   0        0        0      648 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/church2.png
+-rw-r--r--   0        0        0      428 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/circle_green.svg
+-rw-r--r--   0        0        0      421 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/circle_red.svg
+-rw-r--r--   0        0        0     1138 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/cluster.png
+-rw-r--r--   0        0        0      604 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/cluster.svg
+-rw-r--r--   0        0        0     1050 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/current_location - Kopie.svg
+-rw-r--r--   0        0        0     1050 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/current_location.svg
+-rw-r--r--   0        0        0     1270 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/cycling.png
+-rw-r--r--   0        0        0      780 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/finish.png
+-rw-r--r--   0        0        0      482 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/flag.png
+-rw-r--r--   0        0        0      428 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/fullscreen_m.svg
+-rw-r--r--   0        0        0      410 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/fullscreen_p.svg
+-rw-r--r--   0        0        0      710 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/harbor.png
+-rw-r--r--   0        0        0     1325 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/hiking.png
+-rw-r--r--   0        0        0      309 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/hotel.png
+-rw-r--r--   0        0        0      892 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/hotel2.png
+-rw-r--r--   0        0        0     3311 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/kreis.png
+-rw-r--r--   0        0        0      650 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/library.png
+-rw-r--r--   0        0        0      204 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/lupe_m.png
+-rw-r--r--   0        0        0      392 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/lupe_m_32.png
+-rw-r--r--   0        0        0      200 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/lupe_p.png
+-rw-r--r--   0        0        0      405 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/lupe_p_32.png
+-rw-r--r--   0        0        0      645 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/marker-icon_bw.png
+-rw-r--r--   0        0        0      495 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/marker-icon_bw_41x25.png
+-rw-r--r--   0        0        0      345 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/marker-icon_bw_small.png
+-rw-r--r--   0        0        0       77 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/marker.gif
+-rw-r--r--   0        0        0      699 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/marker.svg
+-rw-r--r--   0        0        0      849 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/museum.png
+-rw-r--r--   0        0        0     1390 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/panorama.png
+-rw-r--r--   0        0        0     1100 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/park.png
+-rw-r--r--   0        0        0      545 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/peak.png
+-rw-r--r--   0        0        0      720 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/photo.png
+-rw-r--r--   0        0        0      642 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/pin_red.png
+-rw-r--r--   0        0        0      650 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/pin_red_shadow.png
+-rw-r--r--   0        0        0     1003 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/restaurant.png
+-rw-r--r--   0        0        0      394 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/scenic.png
+-rw-r--r--   0        0        0      770 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/shadow.png
+-rw-r--r--   0        0        0      570 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/shadow50.png
+-rw-r--r--   0        0        0      643 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/shoppingmall.png
+-rw-r--r--   0        0        0      438 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/square_green.svg
+-rw-r--r--   0        0        0      431 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/square_red.svg
+-rw-r--r--   0        0        0      449 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/start.png
+-rw-r--r--   0        0        0      603 2024-04-08 19:04:10.823843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/streckenmarker - Kopie.svg
+-rw-r--r--   0        0        0      603 2024-04-08 19:04:10.824843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/streckenmarker.svg
+-rw-r--r--   0        0        0      795 2024-04-08 19:04:10.824843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/subway.png
+-rw-r--r--   0        0        0      642 2024-04-08 19:04:10.824843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/tent.png
+-rw-r--r--   0        0        0      947 2024-04-08 19:04:10.824843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/train.png
+-rw-r--r--   0        0        0     1290 2024-04-08 19:04:10.824843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/video.png
+-rw-r--r--   0        0        0      626 2024-04-08 19:04:10.824843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/villa.png
+-rw-r--r--   0        0        0      657 2024-04-08 19:04:10.824843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/whereami.svg
+-rw-r--r--   0        0        0     1121 2024-04-08 19:04:10.824843 fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/whereami_V1.svg
+-rw-r--r--   0        0        0    37589 2024-04-08 19:04:10.824843 fietsboek-0.9.0/fietsboek/static/GM_Utils/gmutils.js
+-rw-r--r--   0        0        0     3736 2024-04-08 19:04:10.824843 fietsboek-0.9.0/fietsboek/static/GM_Utils/gra_canvas.js
+-rw-r--r--   0        0        0     6095 2024-04-08 19:04:10.824843 fietsboek-0.9.0/fietsboek/static/GM_Utils/gra_svg.js
+-rw-r--r--   0        0        0     1259 2024-04-08 19:04:10.824843 fietsboek-0.9.0/fietsboek/static/GM_Utils/leaflet/images/layers-2x.png
+-rw-r--r--   0        0        0      696 2024-04-08 19:04:10.824843 fietsboek-0.9.0/fietsboek/static/GM_Utils/leaflet/images/layers.png
+-rw-r--r--   0        0        0     2464 2024-04-08 19:04:10.824843 fietsboek-0.9.0/fietsboek/static/GM_Utils/leaflet/images/marker-icon-2x.png
+-rw-r--r--   0        0        0     1466 2024-04-08 19:04:10.824843 fietsboek-0.9.0/fietsboek/static/GM_Utils/leaflet/images/marker-icon.png
+-rw-r--r--   0        0        0      618 2024-04-08 19:04:10.824843 fietsboek-0.9.0/fietsboek/static/GM_Utils/leaflet/images/marker-shadow.png
+-rw-r--r--   0        0        0    14670 2024-04-08 19:04:10.824843 fietsboek-0.9.0/fietsboek/static/GM_Utils/leaflet/leaflet.css
+-rw-r--r--   0        0        0   146315 2024-04-08 19:04:10.825843 fietsboek-0.9.0/fietsboek/static/GM_Utils/leaflet/leaflet.js
+-rw-r--r--   0        0        0   223367 2024-04-08 19:04:10.826843 fietsboek-0.9.0/fietsboek/static/GM_Utils/leaflet/leaflet.js.map
+-rw-r--r--   0        0        0    39191 2024-04-08 19:04:10.826843 fietsboek-0.9.0/fietsboek/static/GM_Utils/osmutils.js
+-rw-r--r--   0        0        0    20687 2024-04-08 19:04:10.826843 fietsboek-0.9.0/fietsboek/static/GM_Utils/plot.js
+-rw-r--r--   0        0        0     3594 2024-04-08 19:04:10.826843 fietsboek-0.9.0/fietsboek/static/GM_Utils/shimg.js
+-rw-r--r--   0        0        0    93734 2024-04-08 19:04:10.826843 fietsboek-0.9.0/fietsboek/static/bootstrap-icons.css
+-rw-r--r--   0        0        0    80668 2024-04-08 19:04:10.826843 fietsboek-0.9.0/fietsboek/static/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   280715 2024-04-08 19:04:10.827843 fietsboek-0.9.0/fietsboek/static/bootstrap.css
+-rw-r--r--   0        0        0   205214 2024-04-08 19:04:10.828843 fietsboek-0.9.0/fietsboek/static/chart.umd.js
+-rw-r--r--   0        0        0   953847 2024-04-08 19:04:10.832843 fietsboek-0.9.0/fietsboek/static/chart.umd.js.map
+-rw-r--r--   0        0        0    25053 2024-04-08 19:04:10.832843 fietsboek-0.9.0/fietsboek/static/favicon.png
+-rw-r--r--   0        0        0    17796 2024-04-08 19:04:10.832843 fietsboek-0.9.0/fietsboek/static/fietsboek.js
+-rw-r--r--   0        0        0    14486 2024-04-08 19:04:10.832843 fietsboek-0.9.0/fietsboek/static/fietsboek.js.map
+-rw-r--r--   0        0        0   164360 2024-04-08 19:04:10.832843 fietsboek-0.9.0/fietsboek/static/fonts/bootstrap-icons.woff
+-rw-r--r--   0        0        0   121340 2024-04-08 19:04:10.833843 fietsboek-0.9.0/fietsboek/static/fonts/bootstrap-icons.woff2
+-rw-r--r--   0        0        0    20748 2024-04-08 19:04:10.833843 fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-300.woff
+-rw-r--r--   0        0        0    16812 2024-04-08 19:04:10.833843 fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-300.woff2
+-rw-r--r--   0        0        0    21928 2024-04-08 19:04:10.833843 fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-300italic.woff
+-rw-r--r--   0        0        0    17828 2024-04-08 19:04:10.833843 fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-300italic.woff2
+-rw-r--r--   0        0        0    20772 2024-04-08 19:04:10.833843 fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-500.woff
+-rw-r--r--   0        0        0    16812 2024-04-08 19:04:10.833843 fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-500.woff2
+-rw-r--r--   0        0        0    21868 2024-04-08 19:04:10.833843 fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-500italic.woff
+-rw-r--r--   0        0        0    17896 2024-04-08 19:04:10.833843 fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-500italic.woff2
+-rw-r--r--   0        0        0    20664 2024-04-08 19:04:10.833843 fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-600.woff
+-rw-r--r--   0        0        0    16796 2024-04-08 19:04:10.833843 fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-600.woff2
+-rw-r--r--   0        0        0    21812 2024-04-08 19:04:10.833843 fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-600italic.woff
+-rw-r--r--   0        0        0    17836 2024-04-08 19:04:10.833843 fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-600italic.woff2
+-rw-r--r--   0        0        0    20164 2024-04-08 19:04:10.833843 fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-700.woff
+-rw-r--r--   0        0        0    16360 2024-04-08 19:04:10.833843 fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-700.woff2
+-rw-r--r--   0        0        0    21244 2024-04-08 19:04:10.833843 fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-700italic.woff
+-rw-r--r--   0        0        0    17396 2024-04-08 19:04:10.833843 fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-700italic.woff2
+-rw-r--r--   0        0        0    20656 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-800.woff
+-rw-r--r--   0        0        0    16724 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-800.woff2
+-rw-r--r--   0        0        0    21520 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-800italic.woff
+-rw-r--r--   0        0        0    17704 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-800italic.woff2
+-rw-r--r--   0        0        0    21848 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-italic.woff
+-rw-r--r--   0        0        0    17816 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-italic.woff2
+-rw-r--r--   0        0        0    20704 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-regular.woff
+-rw-r--r--   0        0        0    16720 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-regular.woff2
+-rw-r--r--   0        0        0     4473 2024-04-08 19:04:10.832843 fietsboek-0.9.0/fietsboek/static/fonts.css
+-rw-r--r--   0        0        0    14075 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/static/osm-monkeypatch.js
+-rw-r--r--   0        0        0     2920 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/static/theme.css
+-rw-r--r--   0        0        0      770 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/static/theme.css.map
+-rw-r--r--   0        0        0     4796 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/summaries.py
+-rw-r--r--   0        0        0      280 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/templates/404.jinja2
+-rw-r--r--   0        0        0     2056 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/templates/admin.jinja2
+-rw-r--r--   0        0        0    10947 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/templates/browse.jinja2
+-rw-r--r--   0        0        0     2628 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/templates/create_account.jinja2
+-rw-r--r--   0        0        0     8921 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/templates/details.jinja2
+-rw-r--r--   0        0        0     1055 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/templates/edit.jinja2
+-rw-r--r--   0        0        0    10104 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/templates/edit_form.jinja2
+-rw-r--r--   0        0        0     1128 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/templates/finish_upload.jinja2
+-rw-r--r--   0        0        0     3109 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/templates/home.jinja2
+-rw-r--r--   0        0        0     6853 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/templates/layout.jinja2
+-rw-r--r--   0        0        0     1938 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/templates/login.jinja2
+-rw-r--r--   0        0        0     1479 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/templates/password_reset.jinja2
+-rw-r--r--   0        0        0     7722 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/templates/profile.jinja2
+-rw-r--r--   0        0        0      766 2024-04-08 19:04:10.834843 fietsboek-0.9.0/fietsboek/templates/request_password.jinja2
+-rw-r--r--   0        0        0      780 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/templates/resend_verification.jinja2
+-rw-r--r--   0        0        0      171 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/templates/static-page.jinja2
+-rw-r--r--   0        0        0      603 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/templates/upload.jinja2
+-rw-r--r--   0        0        0     4229 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/templates/user_data.jinja2
+-rw-r--r--   0        0        0      318 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/templates/util.jinja2
+-rw-r--r--   0        0        0     4926 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/transformers/__init__.py
+-rw-r--r--   0        0        0     4086 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/transformers/breaks.py
+-rw-r--r--   0        0        0     4457 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/transformers/elevation.py
+-rw-r--r--   0        0        0    15167 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/updater/__init__.py
+-rw-r--r--   0        0        0     6575 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/updater/cli.py
+-rw-r--r--   0        0        0     1088 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/updater/script.py
+-rw-r--r--   0        0        0     2416 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/updater/scripts/upd_20230103_lu8w3rwlz4ddcpms.py
+-rw-r--r--   0        0        0      475 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/updater/scripts/upd_20230112_v0.5.0.py
+-rw-r--r--   0        0        0      465 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/updater/scripts/upd_20230308_v0.6.0.py
+-rw-r--r--   0        0        0      465 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/updater/scripts/upd_20230424_v0.7.0.py
+-rw-r--r--   0        0        0      465 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/updater/scripts/upd_20230605_v0.8.0.py
+-rw-r--r--   0        0        0      465 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/updater/scripts/upd_20240408_v0.9.0.py
+-rw-r--r--   0        0        0     2110 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/updater/scripts/upd_30ppwg8zi4ujb46f.py
+-rw-r--r--   0        0        0      454 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/updater/scripts/upd_initial.py
+-rw-r--r--   0        0        0      466 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/updater/scripts/upd_v0.4.0.py
+-rw-r--r--   0        0        0    16774 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/util.py
+-rw-r--r--   0        0        0        0 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/views/__init__.py
+-rw-r--r--   0        0        0     2277 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/views/account.py
+-rw-r--r--   0        0        0     2829 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/views/admin.py
+-rw-r--r--   0        0        0    16818 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/views/browse.py
+-rw-r--r--   0        0        0     9534 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/views/default.py
+-rw-r--r--   0        0        0     7527 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/views/detail.py
+-rw-r--r--   0        0        0     3554 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/views/edit.py
+-rw-r--r--   0        0        0      405 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/views/notfound.py
+-rw-r--r--   0        0        0     9270 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/views/profile.py
+-rw-r--r--   0        0        0    15000 2024-04-08 19:04:10.835843 fietsboek-0.9.0/fietsboek/views/tileproxy.py
+-rw-r--r--   0        0        0     7259 2024-04-08 19:04:10.836843 fietsboek-0.9.0/fietsboek/views/upload.py
+-rw-r--r--   0        0        0     7085 2024-04-08 19:04:10.836843 fietsboek-0.9.0/fietsboek/views/user_data.py
+-rw-r--r--   0        0        0     2320 2024-04-08 19:04:10.837843 fietsboek-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4699 1970-01-01 00:00:00.000000 fietsboek-0.9.0/PKG-INFO
```

### Comparing `fietsboek-0.8.0/LICENSE.txt` & `fietsboek-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/README.md` & `fietsboek-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/__init__.py` & `fietsboek-0.9.0/fietsboek/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 * The documentation index: :doc:`../../../index`
 
 .. _Fietsboek repository: https://gitlab.com/dunj3/fietsboek
 
 Content
 -------
 """
+
 import importlib.metadata
 import logging
 from pathlib import Path
 from typing import Callable, Optional
 
 import redis
 from pyramid.config import Configurator
@@ -44,26 +45,32 @@
 def locale_negotiator(request: Request) -> Optional[str]:
     """Negotiates the right locale to use.
 
     This tries the following:
 
     1. It runs the default negotiator. This allows the locale to be overriden
        by using the ``_LOCALE_`` query parameter.
-    2. It uses the `Accept-Language`_ header.
+    2. It checks for the presence of a ``fietsboek_locale`` cookie.
+    3. It uses the `Accept-Language`_ header.
 
     .. _Accept-Language: https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Accept-Language
 
     :param request: The request for which to get the language.
     :return: The determined locale, or ``None`` if the default should be used.
     """
     locale = default_locale_negotiator(request)
     if locale:
         return locale
 
     installed_locales = request.config.available_locales
+
+    if cookie_locale := request.cookies.get("fietsboek_locale"):
+        if cookie_locale in installed_locales:
+            return cookie_locale
+
     sentinel = object()
     negotiated = request.accept_language.lookup(installed_locales, default=sentinel)
     if negotiated is sentinel:
         return None
     return negotiated
 
 
@@ -170,10 +177,11 @@
     config.registry.registerUtility(TileRequester())
 
     jinja2_env = config.get_jinja2_environment()
     jinja2_env.filters["format_decimal"] = mod_jinja2.filter_format_decimal
     jinja2_env.filters["format_datetime"] = mod_jinja2.filter_format_datetime
     jinja2_env.filters["local_datetime"] = mod_jinja2.filter_local_datetime
     jinja2_env.globals["embed_tile_layers"] = mod_jinja2.global_embed_tile_layers
+    jinja2_env.globals["list_languages"] = mod_jinja2.global_list_languages
     jinja2_env.globals["list_transformers"] = transformers.list_transformers
 
     return config.make_wsgi_app()
```

### Comparing `fietsboek-0.8.0/fietsboek/actions.py` & `fietsboek-0.9.0/fietsboek/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """High-level actions.
 
 This module implements the basic logic for high level intents such as "add a
 track", "delete a track", ... It combines the low-level APIs of the ORM and the
 data manager, and provides functions that can be used by the views, the API and
 the test functions.
 """
+
 import datetime
 import logging
 import re
 from typing import List, Optional
 
 import brotli
 import gpxpy
@@ -91,15 +92,17 @@
         manager.compress_gpx(gpx_data)
         manager.backup()
 
         gpx = gpxpy.parse(gpx_data)
         for transformer in transformers:
             LOGGER.debug("Running %s with %r", transformer, transformer.parameters)
             transformer.execute(gpx)
-        track.transformers = [[tfm.identifier(), tfm.parameters.dict()] for tfm in transformers]
+        track.transformers = [
+            [tfm.identifier(), tfm.parameters.model_dump()] for tfm in transformers
+        ]
 
         # Best time to build the cache is right after the upload, but *after* the
         # transformers have been applied!
         track.ensure_cache(gpx)
         dbsession.add(track.cache)
 
         manager.engrave_metadata(
@@ -133,25 +136,34 @@
         image_meta = request.dbsession.execute(
             select(models.ImageMetadata).filter_by(track_id=track.id, image_name=image)
         ).scalar_one_or_none()
         LOGGER.debug("Deleted image %s %s (metadata: %s)", track.id, image, image_meta)
         if image_meta:
             request.dbsession.delete(image_meta)
 
-    # Add new images
+    # Add new images, but only if the setting allows for it
     set_descriptions = set()
     for param_name, image in request.params.items():
         match = re.match("image\\[(\\d+)\\]$", param_name)
         if not match:
             continue
         # Sent for the multi input
         if image == b"":
             continue
 
         upload_id = match.group(1)
+
+        # If the uploads are disabled, we still add the image to
+        # set_descriptions so that later down below we don't try to set the
+        # description for it.
+        if not request.config.enable_image_uploads:
+            set_descriptions.add(upload_id)
+            LOGGER.debug("Tried to upload image but uploads are disabled (track %s)", track.id)
+            continue
+
         image_name = manager.add_image(image.file, image.filename)
         image_meta = models.ImageMetadata(track=track, image_name=image_name)
         image_meta.description = request.params.get(f"image-description[{upload_id}]", "")
         request.dbsession.add(image_meta)
         LOGGER.debug("Uploaded image %s %s", track.id, image_name)
         set_descriptions.add(upload_id)
 
@@ -189,15 +201,15 @@
     :return: The transformed track.
     """
     # pylint: disable=too-many-locals
     LOGGER.debug("Executing transformers for %d", track.id)
 
     settings = mod_transformers.extract_from_request(request)
 
-    serialized = [[tfm.identifier(), tfm.parameters.dict()] for tfm in settings]
+    serialized = [[tfm.identifier(), tfm.parameters.model_dump()] for tfm in settings]
     if serialized == track.transformers:
         LOGGER.debug("Applied transformations match on %d, skipping", track.id)
         return None
 
     # We always start with the backup, that way we don't get "deepfried GPX"
     # files by having the same filters run multiple times on the same input.
     # They are not idempotent after all.
```

### Comparing `fietsboek-0.8.0/fietsboek/alembic/env.py` & `fietsboek-0.9.0/fietsboek/alembic/env.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Pyramid bootstrap environment. """
+
 from alembic import context
 from pyramid.paster import get_appsettings, setup_logging
 from sqlalchemy import engine_from_config
 
 from fietsboek.models.meta import Base
 
 config = context.config
```

### Comparing `fietsboek-0.8.0/fietsboek/alembic/versions/20220702_1b4b1c179e5a.py` & `fietsboek-0.9.0/fietsboek/alembic/versions/20220702_1b4b1c179e5a.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/alembic/versions/20220706_c89d9bdbfa68.py` & `fietsboek-0.9.0/fietsboek/alembic/versions/20220706_c89d9bdbfa68.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/alembic/versions/20220721_091ce24409fe.py` & `fietsboek-0.9.0/fietsboek/alembic/versions/20220721_091ce24409fe.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/alembic/versions/20220808_d085998b49ca.py` & `fietsboek-0.9.0/fietsboek/alembic/versions/20220808_d085998b49ca.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/alembic/versions/20221214_c939800af428.py` & `fietsboek-0.9.0/fietsboek/alembic/versions/20221214_c939800af428.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/alembic/versions/20230203_3149aa2d0114.py` & `fietsboek-0.9.0/fietsboek/alembic/versions/20230203_3149aa2d0114.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/config.py` & `fietsboek-0.9.0/fietsboek/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,24 +7,33 @@
 provide the user with good feedback if they aren't, and set the default values
 in a single place.
 
 Most of the logic is handled by pydantic_.
 
 .. _pydantic: https://pydantic-docs.helpmanual.io/
 """
+
 # pylint: disable=no-name-in-module,no-self-argument,too-few-public-methods
 import hashlib
 import logging
 import re
 import typing
 import urllib.parse
 from enum import Enum
 
 import pydantic
-from pydantic import AnyUrl, BaseModel, DirectoryPath, Field, SecretStr, validator
+from pydantic import (
+    AnyUrl,
+    BaseModel,
+    BeforeValidator,
+    DirectoryPath,
+    Field,
+    SecretStr,
+    field_validator,
+)
 from pyramid import settings
 from termcolor import colored
 
 LOGGER = logging.getLogger(__name__)
 
 KNOWN_PYRAMID_SETTINGS = {
     "pyramid.reload_templates",
@@ -86,30 +95,25 @@
     Note that in the future, a finer-grained distinction might be possible.
     """
 
     PUBLIC = "public"
     RESTRICTED = "restricted"
 
 
-class PyramidList(list):
-    """A pydantic field type that uses pyramid.settings.aslist as a parser."""
+def _validate_pyramid_list(value):
+    """Parses the list with pyramid.settings.aslist."""
+    if not isinstance(value, str):
+        raise TypeError("string required")
+    return settings.aslist(value)
 
-    @classmethod
-    def __get_validators__(cls):
-        yield cls.validate
 
-    @classmethod
-    def validate(cls, value):
-        """Parses the list with pyramid.settings.aslist."""
-        if not isinstance(value, str):
-            raise TypeError("string required")
-        return settings.aslist(value)
+PyramidList = typing.Annotated[list, BeforeValidator(_validate_pyramid_list)]
 
 
-class TileLayerConfig(BaseModel, allow_population_by_field_name=True):
+class TileLayerConfig(BaseModel, populate_by_name=True):
     """Object representing a single tile layer."""
 
     layer_id: str
     """ID of the layer."""
 
     name: str
     """Human-readable name of the layer."""
@@ -141,14 +145,17 @@
 
     data_dir: DirectoryPath = Field(alias="fietsboek.data_dir")
     """Fietsboek data directory."""
 
     enable_account_registration: bool = False
     """Enable registration of new accounts."""
 
+    enable_image_uploads: bool = Field(True, alias="fietsboek.enable_image_uploads")
+    """Allow track uploaders to also upload images for tracks."""
+
     session_key: str
     """Session key."""
 
     language_packs: PyramidList = Field([], alias="fietsboek.language_packs")
     """Additional language packs to load."""
 
     available_locales: PyramidList = PyramidList(["en", "de"])
@@ -203,42 +210,46 @@
 
     hittekaart_threads: int = Field(0, alias="hittekaart.threads")
     """Number of threads that hittekaart should use.
 
     Defaults to 0, which makes it use as many threads as there are CPU cores.
     """
 
-    @validator("session_key")
+    @field_validator("session_key")
+    @classmethod
     def _good_session_key(cls, value):
         """Ensures that the session key has been changed from its default
         value.
         """
         if value == "<EDIT THIS>":
             raise ValueError("You need to edit the default session key!")
         return value
 
-    @validator("email_smtp_url")
+    @field_validator("email_smtp_url")
+    @classmethod
     def _known_smtp_url(cls, value):
         """Ensures that the SMTP URL is valid."""
         parsed = urllib.parse.urlparse(value)
         if parsed.scheme not in {"debug", "smtp", "smtp+ssl", "smtp+starttls"}:
             raise ValueError(f"Unknown mailing scheme {parsed.scheme}".strip())
         return value
 
-    @validator("stamen_maps")
+    @field_validator("stamen_maps")
+    @classmethod
     def _known_stamen(cls, value):
         """Ensures that the stamen maps are known."""
         maps = set(value)
         known_maps = {"toner", "terrain", "watercolor"}
         bad_maps = maps - known_maps
         if bad_maps:
             raise ValueError("Unknown stamen maps: " + ", ".join(bad_maps))
         return value
 
-    @validator("hittekaart_autogenerate")
+    @field_validator("hittekaart_autogenerate")
+    @classmethod
     def _known_hittekaart_modes(cls, value):
         """Ensures that the hittekaart modes are valid."""
         # pylint: disable=import-outside-toplevel
         from . import hittekaart
 
         modes = set(value)
         known_modes = {mode.value for mode in hittekaart.Mode}
@@ -281,47 +292,50 @@
     tile_layers = []
     for key, value in config.items():
         match = re.match("^fietsboek\\.tile_layer\\.([A-Za-z0-9_-]+)$", key)
         if not match:
             continue
         provider_id = match.group(1)
 
-        prefix = f"{value}."
+        prefix = f"{key}."
         inner = {k[len(prefix) :]: v for (k, v) in config.items() if k.startswith(prefix)}
         inner["layer_id"] = provider_id
         inner["name"] = value
         try:
-            layer_config = TileLayerConfig.parse_obj(inner)
+            layer_config = TileLayerConfig.model_validate(inner)
             tile_layers.append(layer_config)
         except pydantic.ValidationError as validation_error:
             errors.append((f"tile layer {provider_id}", validation_error))
 
         keys.discard(key)
-        for field in TileLayerConfig.__fields__.values():
-            keys.discard(f"{prefix}{_field_name(field)}")
+        for field_name, field in TileLayerConfig.model_fields.items():
+            keys.discard(f"{prefix}{_field_name(field_name, field)}")
 
     config["tile_layers"] = tile_layers
 
     # Now we can parse the main config
     try:
-        parsed_config = Config.parse_obj(config)
+        parsed_config = Config.model_validate(config)
     except pydantic.ValidationError as validation_error:
         errors.append(("configuration", validation_error))
 
     if errors:
         raise ValidationError(errors)
 
-    for field in Config.__fields__.values():
-        keys.discard(_field_name(field))
+    for field_name, field in Config.model_fields.items():
+        keys.discard(_field_name(field_name, field))
     keys -= KNOWN_PYRAMID_SETTINGS
 
     for key in keys:
         LOGGER.warning("Unknown configuration key: %r", key)
 
     return parsed_config
 
 
-def _field_name(field):
+def _field_name(field_name, field):
+    """Returns the field's alias, or the original name if the alias does not
+    exist.
+    """
     alias = getattr(field, "alias", None)
     if alias:
         return alias
-    return field.name
+    return field_name
```

### Comparing `fietsboek-0.8.0/fietsboek/convert.py` & `fietsboek-0.9.0/fietsboek/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Conversion functions to convert between various recording formats."""
+
 import fitparse
 from gpxpy.gpx import GPX, GPXTrack, GPXTrackPoint, GPXTrackSegment
 
 FIT_RECORD_FIELDS = ["position_lat", "position_long", "altitude", "timestamp"]
 
 
 def semicircles_to_deg(circles: int) -> float:
```

### Comparing `fietsboek-0.8.0/fietsboek/data.py` & `fietsboek-0.9.0/fietsboek/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 """Data manager for fietsboek.
 
 Data are objects that belong to a track (such as images), but are not stored in
 the database itself. This module makes access to such data objects easier.
 """
+
+# We don't have onexc yet in all supported versions, so let's ignore the
+# deprecation for now and stick with onerror:
+# pylint: disable=deprecated-argument
 import datetime
 import logging
 import os
 import random
 import shutil
 import string
 import uuid
@@ -310,14 +314,15 @@
 
         :param title: The title of the track.
         :param description: The description of the track.
         :param creator: Name of the track's creator.
         :param time: Time of the track.
         :param gpx: The pre-parsed GPX track, to save time if it is already parsed.
         """
+        # pylint: disable=too-many-arguments
         if gpx is None:
             gpx = gpxpy.parse(self.decompress_gpx())
         # First we delete the existing metadata
         for track in gpx.tracks:
             track.name = None
             track.description = None
```

### Comparing `fietsboek-0.8.0/fietsboek/email.py` & `fietsboek-0.9.0/fietsboek/email.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utility functions for email sending."""
+
 import logging
 import smtplib
 import sys
 from email.message import EmailMessage
 from typing import Optional
 from urllib.parse import urlparse
```

### Comparing `fietsboek-0.8.0/fietsboek/hittekaart.py` & `fietsboek-0.9.0/fietsboek/hittekaart.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Interface to the hittekaart_ application to generate heatmaps.
 
 .. _hittekaart: https://gitlab.com/dunj3/hittekaart
 """
+
 import enum
 import logging
 import shutil
 import subprocess
 import tempfile
 from pathlib import Path
 from typing import Optional
@@ -102,14 +103,15 @@
     :param user: The user for which to generate the map.
     :param dbsession: The database session.
     :param data_manager: The data manager.
     :param mode: The mode of the heatmap.
     :param exe_path: See :meth:`generate`.
     :param threads: See :meth:`generate`.
     """
+    # pylint: disable=too-many-arguments
     if user.id is None:
         raise ValueError("User has no ID, cannot generate a heatmap yet")
 
     query = user.all_tracks_query()
     query = select(aliased(models.Track, query)).where(query.c.type == TrackType.ORGANIC)
     input_paths = []
     for track in dbsession.execute(query).scalars():
```

### Comparing `fietsboek-0.8.0/fietsboek/jinja2.py` & `fietsboek-0.9.0/fietsboek/jinja2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Custom filters for Jinja2."""
+
 import datetime
 import json
 
 import jinja2
 from babel.dates import format_datetime
 from babel.numbers import format_decimal
 from jinja2.runtime import Context
@@ -108,7 +109,19 @@
                     "type": source.layer_type.value,
                     "zoom": source.zoom,
                 }
                 for source in tile_sources
             ]
         )
     )
+
+
+def global_list_languages(request: Request) -> list[tuple[str, str]]:
+    """Returns a list of available languages.
+
+    The first element of each tuple is the (technical) locale name, the second
+    element is the display name.
+
+    :param request: The Pyramid request.
+    :return: The available languages.
+    """
+    return util.list_locales(request)
```

### Comparing `fietsboek-0.8.0/fietsboek/locale/de/LC_MESSAGES/messages.mo` & `fietsboek-0.9.0/fietsboek/locale/de/LC_MESSAGES/messages.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-31 20:46+0200\n"
+"POT-Creation-Date: 2024-04-06 21:57+0200\n"
 "PO-Revision-Date: 2022-07-02 17:35+0200\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "email.verify.text"
 msgstr ""
 "Um Dein Fietsboek-Konto zu bestätigen, nutze diesen Link: {}\n"
 "\n"
 "Falls Du kein Konto angelegt hast, ignoriere diese E-Mail."
 
@@ -84,14 +84,18 @@
 
 msgid "flash.resend_verification_email_fail"
 msgstr "Ungültige E-Mail-Adresse angegeben"
 
 msgid "flash.reset_invalid_email"
 msgstr "Ungültige E-Mail-Adresse angegeben"
 
+msgid "flash.sessions_logged_out"
+msgstr ""
+"Die Sitzungen wurden beendet. Melde Dich bitte erneut an, um fortzufahren."
+
 msgid "flash.token_expired"
 msgstr "Der Link ist nicht mehr gültig"
 
 msgid "flash.track_deleted"
 msgstr "Strecke gelöscht"
 
 msgid "flash.upload_cancelled"
@@ -126,14 +130,23 @@
 
 msgid "page.browse.download_multiple"
 msgstr "ausgewählte Herunterladen"
 
 msgid "page.browse.filter.date_boundaries"
 msgstr "Datumsgrenzen"
 
+msgid "page.browse.filter.favourite.all"
+msgstr "Alle Strecken"
+
+msgid "page.browse.filter.favourite.no"
+msgstr "Keine Favoriten"
+
+msgid "page.browse.filter.favourite.yes"
+msgstr "Nur Favoriten"
+
 msgid "page.browse.filter.friends_tracks_only"
 msgstr "Zeige nur Strecken von Freunden"
 
 msgid "page.browse.filter.length_boundaries"
 msgstr "Längenbeschränkungen"
 
 msgid "page.browse.filter.length_maximum"
@@ -394,14 +407,26 @@
 
 msgid "page.my_profile.personal_data.save"
 msgstr "Speichern"
 
 msgid "page.my_profile.send_friend_request"
 msgstr "Freundschaftsanfrage senden"
 
+msgid "page.my_profile.session_logout.button"
+msgstr "Alle Sitzungen beenden"
+
+msgid "page.my_profile.session_logout.explanation"
+msgstr ""
+"Mit dieser Funktion können alle Sitzungen beendet werden. Dies ist nützlich, "
+"wenn Du vergessen hast, dich auf einem fremden Gerät abzumelden. Beachte, "
+"dass Du dich erneut anmelden musst, wenn Du diese Funktion nutzt!"
+
+msgid "page.my_profile.session_logout.title"
+msgstr "Sitzungen abmelden"
+
 msgid "page.my_profile.title"
 msgstr "Mein Profil"
 
 msgid "page.my_profile.unfriend"
 msgstr "Entfreunden"
 
 msgid "page.navbar.admin"
@@ -469,20 +494,29 @@
 
 msgid "page.password_reset.reset"
 msgstr "Zurücksetzen"
 
 msgid "page.password_reset.title"
 msgstr "Passwort Zurücksetzen"
 
+msgid "page.profile.avg_duration"
+msgstr "durchschnittliche Dauer"
+
+msgid "page.profile.avg_length"
+msgstr "durchschnittliche Länge"
+
 msgid "page.profile.avg_speed"
 msgstr "durchschnittliche Geschwindigkeit"
 
 msgid "page.profile.downhill"
 msgstr "Bergab"
 
+msgid "page.profile.graph.km_per_month"
+msgstr "Kilometer pro Monat"
+
 msgid "page.profile.heatmap"
 msgstr "Heatmap"
 
 msgid "page.profile.length"
 msgstr "Länge"
 
 msgid "page.profile.longest_distance_track"
@@ -505,14 +539,20 @@
 
 msgid "page.profile.shortest_duration_track"
 msgstr "Am Kürzesten Dauernde Strecke"
 
 msgid "page.profile.stopped_time"
 msgstr "Haltezeit"
 
+msgid "page.profile.tabbar.graphs"
+msgstr "Diagramme"
+
+msgid "page.profile.tabbar.overview"
+msgstr "Übersicht"
+
 msgid "page.profile.tilehunt"
 msgstr "Kacheljäger"
 
 msgid "page.profile.uphill"
 msgstr "Bergauf"
 
 msgid "page.request_password.email"
@@ -559,14 +599,17 @@
 
 msgid "page.track.form.image_description_modal"
 msgstr "Bildbeschreibung"
 
 msgid "page.track.form.image_description_modal.save"
 msgstr "Übernehmen"
 
+msgid "page.track.form.image_uploads_disabled"
+msgstr "Das Hochladen von Bildern ist auf diesem Fietsboek deaktiviert"
+
 msgid "page.track.form.remove_image"
 msgstr "Bild entfernen"
 
 msgid "page.track.form.select_images"
 msgstr "Bilder auswählen"
 
 msgid "page.track.form.tagged_people"
@@ -642,14 +685,17 @@
 
 msgid "tooltip.table.max_speed"
 msgstr "Maximalgeschwindigkeit"
 
 msgid "tooltip.table.moving_time"
 msgstr "Fahrzeit"
 
+msgid "tooltip.table.people"
+msgstr "# Personen"
+
 msgid "tooltip.table.stopped_time"
 msgstr "Haltezeit"
 
 msgid "tooltip.table.uphill"
 msgstr "Bergauf"
 
 msgid "transformers.fix-elevation-jumps"
```

### Comparing `fietsboek-0.8.0/fietsboek/locale/de/LC_MESSAGES/messages.po` & `fietsboek-0.9.0/fietsboek/locale/de/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,69 +3,73 @@
 # This file is distributed under the same license as the Fietsboek project.
 # Daniel Schadt, 2022.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-31 20:46+0200\n"
+"POT-Creation-Date: 2024-04-06 21:57+0200\n"
 "PO-Revision-Date: 2022-07-02 17:35+0200\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
+"Generated-By: Babel 2.14.0\n"
 
-#: fietsboek/actions.py:250
+#: fietsboek/actions.py:267
 msgid "email.verify_mail.subject"
 msgstr "Fietsboek Konto Bestätigung"
 
-#: fietsboek/actions.py:253
+#: fietsboek/actions.py:270
 msgid "email.verify.text"
 msgstr ""
 "Um Dein Fietsboek-Konto zu bestätigen, nutze diesen Link: {}\n"
 "\n"
 "Falls Du kein Konto angelegt hast, ignoriere diese E-Mail."
 
-#: fietsboek/util.py:304
+#: fietsboek/util.py:310
 msgid "password_constraint.mismatch"
 msgstr "Passwörter stimmen nicht überein"
 
-#: fietsboek/util.py:306
+#: fietsboek/util.py:312
 msgid "password_constraint.length"
 msgstr "Passwort zu kurz"
 
-#: fietsboek/models/track.py:579
+#: fietsboek/models/track.py:603
 msgid "tooltip.table.length"
 msgstr "Länge"
 
-#: fietsboek/models/track.py:580
+#: fietsboek/models/track.py:604
+msgid "tooltip.table.people"
+msgstr "# Personen"
+
+#: fietsboek/models/track.py:605
 msgid "tooltip.table.uphill"
 msgstr "Bergauf"
 
-#: fietsboek/models/track.py:581
+#: fietsboek/models/track.py:606
 msgid "tooltip.table.downhill"
 msgstr "Bergab"
 
-#: fietsboek/models/track.py:582
+#: fietsboek/models/track.py:607
 msgid "tooltip.table.moving_time"
 msgstr "Fahrzeit"
 
-#: fietsboek/models/track.py:583
+#: fietsboek/models/track.py:608
 msgid "tooltip.table.stopped_time"
 msgstr "Haltezeit"
 
-#: fietsboek/models/track.py:585
+#: fietsboek/models/track.py:610
 msgid "tooltip.table.max_speed"
 msgstr "Maximalgeschwindigkeit"
 
-#: fietsboek/models/track.py:589
+#: fietsboek/models/track.py:614
 msgid "tooltip.table.avg_speed"
 msgstr "Durchschnittsgeschwindigkeit"
 
 #: fietsboek/templates/admin.jinja2:5
 msgid "page.admin.title"
 msgstr "Administration"
 
@@ -129,117 +133,129 @@
 msgid "page.browse.filter.type.organic"
 msgstr "Aufnahme (natürlich)"
 
 #: fietsboek/templates/browse.jinja2:74
 msgid "page.browse.filter.type.synthetic"
 msgstr "Vorlage (synthetisch)"
 
-#: fietsboek/templates/browse.jinja2:86
+#: fietsboek/templates/browse.jinja2:82
+msgid "page.browse.filter.favourite.all"
+msgstr "Alle Strecken"
+
+#: fietsboek/templates/browse.jinja2:83
+msgid "page.browse.filter.favourite.yes"
+msgstr "Nur Favoriten"
+
+#: fietsboek/templates/browse.jinja2:84
+msgid "page.browse.filter.favourite.no"
+msgstr "Keine Favoriten"
+
+#: fietsboek/templates/browse.jinja2:97
 msgid "page.browse.filter.my_tracks.only"
 msgstr "Zeige nur eigene Strecken"
 
-#: fietsboek/templates/browse.jinja2:87
+#: fietsboek/templates/browse.jinja2:98
 msgid "page.browse.filter.friends_tracks_only"
 msgstr "Zeige nur Strecken von Freunden"
 
-#: fietsboek/templates/browse.jinja2:88
+#: fietsboek/templates/browse.jinja2:99
 msgid "page.browse.filter.me_tagged_only"
 msgstr "Zeige nur Strecken, in denen ich markiert bin"
 
-#: fietsboek/templates/browse.jinja2:98
+#: fietsboek/templates/browse.jinja2:109
 msgid "page.browse.filters.apply"
 msgstr "Filter anwenden"
 
-#: fietsboek/templates/browse.jinja2:102
+#: fietsboek/templates/browse.jinja2:113
 msgid "page.browse.filters.clear_all"
 msgstr "Filter zurücksetzen"
 
-#: fietsboek/templates/browse.jinja2:105
+#: fietsboek/templates/browse.jinja2:116
 msgid "page.browse.filters.expand_advanced"
 msgstr "Erweitert"
 
-#: fietsboek/templates/browse.jinja2:110 fietsboek/templates/browse.jinja2:111
+#: fietsboek/templates/browse.jinja2:121 fietsboek/templates/browse.jinja2:122
 msgid "page.browse.sort.date"
 msgstr "Nach Datum sortieren"
 
-#: fietsboek/templates/browse.jinja2:112 fietsboek/templates/browse.jinja2:113
+#: fietsboek/templates/browse.jinja2:123 fietsboek/templates/browse.jinja2:124
 msgid "page.browse.sort.length"
 msgstr "Nach Länge sortieren"
 
-#: fietsboek/templates/browse.jinja2:114 fietsboek/templates/browse.jinja2:115
+#: fietsboek/templates/browse.jinja2:125 fietsboek/templates/browse.jinja2:126
 msgid "page.browse.sort.duration"
 msgstr "Nach Dauer sortieren"
 
-#: fietsboek/templates/browse.jinja2:132
+#: fietsboek/templates/browse.jinja2:148
 msgid "page.browse.organic_tooltip"
 msgstr "Dies ist eine Aufnahme einer Strecke"
 
-#: fietsboek/templates/browse.jinja2:134
+#: fietsboek/templates/browse.jinja2:150
 msgid "page.browse.synthetic_tooltip"
 msgstr "Dies ist eine geplante Strecke"
 
-#: fietsboek/templates/browse.jinja2:142 fietsboek/templates/details.jinja2:90
+#: fietsboek/templates/browse.jinja2:158 fietsboek/templates/details.jinja2:103
 #: fietsboek/templates/profile.jinja2:15
 msgid "page.details.date"
 msgstr "Datum"
 
-#: fietsboek/templates/browse.jinja2:144 fietsboek/templates/details.jinja2:104
+#: fietsboek/templates/browse.jinja2:160 fietsboek/templates/details.jinja2:117
 #: fietsboek/templates/profile.jinja2:17
 msgid "page.details.length"
 msgstr "Länge"
 
-#: fietsboek/templates/browse.jinja2:149 fietsboek/templates/details.jinja2:95
+#: fietsboek/templates/browse.jinja2:165 fietsboek/templates/details.jinja2:108
 #: fietsboek/templates/profile.jinja2:21
 msgid "page.details.start_time"
 msgstr "Startzeit"
 
-#: fietsboek/templates/browse.jinja2:151 fietsboek/templates/details.jinja2:99
+#: fietsboek/templates/browse.jinja2:167 fietsboek/templates/details.jinja2:112
 #: fietsboek/templates/profile.jinja2:23
 msgid "page.details.end_time"
 msgstr "Endzeit"
 
-#: fietsboek/templates/browse.jinja2:156 fietsboek/templates/details.jinja2:108
+#: fietsboek/templates/browse.jinja2:172 fietsboek/templates/details.jinja2:121
 #: fietsboek/templates/profile.jinja2:27
 msgid "page.details.uphill"
 msgstr "Bergauf"
 
-#: fietsboek/templates/browse.jinja2:158 fietsboek/templates/details.jinja2:112
+#: fietsboek/templates/browse.jinja2:174 fietsboek/templates/details.jinja2:125
 #: fietsboek/templates/profile.jinja2:29
 msgid "page.details.downhill"
 msgstr "Bergab"
 
-#: fietsboek/templates/browse.jinja2:163 fietsboek/templates/details.jinja2:117
+#: fietsboek/templates/browse.jinja2:179 fietsboek/templates/details.jinja2:130
 #: fietsboek/templates/profile.jinja2:33
 msgid "page.details.moving_time"
 msgstr "Fahrzeit"
 
-#: fietsboek/templates/browse.jinja2:165 fietsboek/templates/details.jinja2:121
+#: fietsboek/templates/browse.jinja2:181 fietsboek/templates/details.jinja2:134
 #: fietsboek/templates/profile.jinja2:35
 msgid "page.details.stopped_time"
 msgstr "Haltezeit"
 
-#: fietsboek/templates/browse.jinja2:169 fietsboek/templates/details.jinja2:125
+#: fietsboek/templates/browse.jinja2:185 fietsboek/templates/details.jinja2:138
 #: fietsboek/templates/profile.jinja2:39
 msgid "page.details.max_speed"
 msgstr "maximale Geschwindigkeit"
 
-#: fietsboek/templates/browse.jinja2:171 fietsboek/templates/details.jinja2:129
+#: fietsboek/templates/browse.jinja2:187 fietsboek/templates/details.jinja2:142
 #: fietsboek/templates/profile.jinja2:41
 msgid "page.details.avg_speed"
 msgstr "durchschnittliche Geschwindigkeit"
 
-#: fietsboek/templates/browse.jinja2:189
+#: fietsboek/templates/browse.jinja2:205
 msgid "page.browse.download_multiple"
 msgstr "ausgewählte Herunterladen"
 
-#: fietsboek/templates/browse.jinja2:191
+#: fietsboek/templates/browse.jinja2:207
 msgid "page.browse.no_results"
 msgstr "Es wurden keine Strecken gefunden, die den Filtern entsprechen."
 
-#: fietsboek/templates/browse.jinja2:193
+#: fietsboek/templates/browse.jinja2:209
 msgid "page.browse.no_tracks"
 msgstr ""
 "Es wurden keine Strecken gefunden, auf die Du Zugriff hast. Versuche, "
 "Dich anzumelden."
 
 #: fietsboek/templates/create_account.jinja2:5
 msgid "page.create_account.title"
@@ -277,98 +293,98 @@
 msgid "page.create_account.repeat_password"
 msgstr "Passwort wiederholen"
 
 #: fietsboek/templates/create_account.jinja2:54
 msgid "page.create_account.create"
 msgstr "Erstellen"
 
-#: fietsboek/templates/details.jinja2:6
+#: fietsboek/templates/details.jinja2:7
 msgid "page.details.title"
 msgstr "Details"
 
-#: fietsboek/templates/details.jinja2:9
+#: fietsboek/templates/details.jinja2:20
 msgid "page.details.edit"
 msgstr "Bearbeiten"
 
-#: fietsboek/templates/details.jinja2:10
+#: fietsboek/templates/details.jinja2:21
 msgid "page.details.share"
 msgstr "Teilen"
 
-#: fietsboek/templates/details.jinja2:11
+#: fietsboek/templates/details.jinja2:22
 msgid "page.details.delete"
 msgstr "Löschen"
 
-#: fietsboek/templates/details.jinja2:17
+#: fietsboek/templates/details.jinja2:28
 msgid "page.details.sharelink.title"
 msgstr "Link zum Teilen"
 
-#: fietsboek/templates/details.jinja2:21
+#: fietsboek/templates/details.jinja2:32
 msgid "page.details.sharelink.info"
 msgstr "Jeder mit Zugang zu diesem Link kann die Strecke ansehen!"
 
-#: fietsboek/templates/details.jinja2:28
+#: fietsboek/templates/details.jinja2:39
 msgid "page.details.sharelink.invalidate"
 msgstr "Link invalidieren"
 
-#: fietsboek/templates/details.jinja2:30
+#: fietsboek/templates/details.jinja2:41
 msgid "page.details.sharelink.close"
 msgstr "Schließen"
 
-#: fietsboek/templates/details.jinja2:40
+#: fietsboek/templates/details.jinja2:51
 msgid "page.details.delete.title"
 msgstr "Strecke Löschen"
 
-#: fietsboek/templates/details.jinja2:44
+#: fietsboek/templates/details.jinja2:55
 msgid "page.details.delete.info"
 msgstr "Das Löschen der Strecke wird alle damit verbundenen Informationen löschen!"
 
-#: fietsboek/templates/details.jinja2:49
+#: fietsboek/templates/details.jinja2:60
 msgid "page.details.delete.delete"
 msgstr "Löschen"
 
-#: fietsboek/templates/details.jinja2:51
+#: fietsboek/templates/details.jinja2:62
 msgid "page.details.delete.close"
 msgstr "Abbrechen"
 
-#: fietsboek/templates/details.jinja2:70
+#: fietsboek/templates/details.jinja2:81
 msgid "page.details.tags"
 msgstr "Schlagwörter"
 
-#: fietsboek/templates/details.jinja2:80 fietsboek/templates/edit.jinja2:10
+#: fietsboek/templates/details.jinja2:91 fietsboek/templates/edit.jinja2:10
 #: fietsboek/templates/finish_upload.jinja2:10
 msgid "page.noscript"
 msgstr ""
 "JavaScript ist deaktiviert, zum Nutzen aller Funktionen bitte JavaScript "
 "aktivieren"
 
-#: fietsboek/templates/details.jinja2:85
+#: fietsboek/templates/details.jinja2:97
 msgid "page.details.download"
 msgstr "Herunterladen"
 
-#: fietsboek/templates/details.jinja2:174
+#: fietsboek/templates/details.jinja2:187
 msgid "page.details.comments"
 msgstr "Kommentare"
 
-#: fietsboek/templates/details.jinja2:178
+#: fietsboek/templates/details.jinja2:191
 msgid "page.details.comments.author"
 msgstr "Kommentar von {}"
 
-#: fietsboek/templates/details.jinja2:195
+#: fietsboek/templates/details.jinja2:208
 msgid "page.details.comments.new.title"
 msgstr "Kommentar erstellen"
 
-#: fietsboek/templates/details.jinja2:198
+#: fietsboek/templates/details.jinja2:211
 msgid "page.details.comments.new.input_title"
 msgstr "Titel"
 
-#: fietsboek/templates/details.jinja2:199
+#: fietsboek/templates/details.jinja2:212
 msgid "page.details.comments.new.input_comment"
 msgstr "Kommentar"
 
-#: fietsboek/templates/details.jinja2:202
+#: fietsboek/templates/details.jinja2:215
 msgid "page.details.comments.new.submit"
 msgstr "Absenden"
 
 #: fietsboek/templates/edit.jinja2:8
 msgid "page.edit.title"
 msgstr "Strecke Bearbeiten"
 
@@ -442,40 +458,44 @@
 msgid "page.track.form.tagged_people"
 msgstr "Markierte Personen"
 
 #: fietsboek/templates/edit_form.jinja2:70
 msgid "page.track.form.add_friend"
 msgstr "Freund suchen"
 
-#: fietsboek/templates/edit_form.jinja2:90
+#: fietsboek/templates/edit_form.jinja2:92
 msgid "page.track.form.badges"
 msgstr "Wappen"
 
-#: fietsboek/templates/edit_form.jinja2:101
+#: fietsboek/templates/edit_form.jinja2:103
 msgid "page.track.form.description"
 msgstr "Beschreibung"
 
-#: fietsboek/templates/edit_form.jinja2:108
-#: fietsboek/templates/edit_form.jinja2:122
+#: fietsboek/templates/edit_form.jinja2:110
+#: fietsboek/templates/edit_form.jinja2:131
 msgid "page.track.form.remove_image"
 msgstr "Bild entfernen"
 
-#: fietsboek/templates/edit_form.jinja2:117
+#: fietsboek/templates/edit_form.jinja2:120
 msgid "page.track.form.select_images"
 msgstr "Bilder auswählen"
 
-#: fietsboek/templates/edit_form.jinja2:133
+#: fietsboek/templates/edit_form.jinja2:124
+msgid "page.track.form.image_uploads_disabled"
+msgstr "Das Hochladen von Bildern ist auf diesem Fietsboek deaktiviert"
+
+#: fietsboek/templates/edit_form.jinja2:142
 msgid "page.track.form.image_description_modal"
 msgstr "Bildbeschreibung"
 
-#: fietsboek/templates/edit_form.jinja2:140
+#: fietsboek/templates/edit_form.jinja2:149
 msgid "page.track.form.image_description_modal.save"
 msgstr "Übernehmen"
 
-#: fietsboek/templates/edit_form.jinja2:166
+#: fietsboek/templates/edit_form.jinja2:175
 msgid "page.track.form.transformer.enable"
 msgstr "Transformation anwenden"
 
 #: fietsboek/templates/finish_upload.jinja2:8
 #: fietsboek/templates/upload.jinja2:6
 msgid "page.upload.title"
 msgstr "Hochladen"
@@ -496,21 +516,21 @@
 #: fietsboek/templates/home.jinja2:17
 msgid "page.home.unfinished_uploads"
 msgstr ""
 "Es sind noch nicht abgeschlossene Uploads vorhanden. Klicke auf die "
 "Links, um sie fortzusetzen:"
 
 #: fietsboek/templates/home.jinja2:31 fietsboek/templates/home.jinja2:38
-#: fietsboek/templates/home.jinja2:56
+#: fietsboek/templates/home.jinja2:66
 msgid "page.home.summary.track"
 msgid_plural "page.home.summary.tracks"
 msgstr[0] "%(num)d Strecke"
 msgstr[1] "%(num)d Strecken"
 
-#: fietsboek/templates/home.jinja2:56
+#: fietsboek/templates/home.jinja2:66
 msgid "page.home.total"
 msgstr "Gesamt"
 
 #: fietsboek/templates/layout.jinja2:43
 msgid "page.navbar.toggle"
 msgstr "Navigation umschalten"
 
@@ -606,67 +626,87 @@
 msgid "page.password_reset.password_mismatch"
 msgstr "Passwörter stimmen nicht überein"
 
 #: fietsboek/templates/password_reset.jinja2:30
 msgid "page.password_reset.reset"
 msgstr "Zurücksetzen"
 
-#: fietsboek/templates/profile.jinja2:66
+#: fietsboek/templates/profile.jinja2:64
+msgid "page.profile.tabbar.overview"
+msgstr "Übersicht"
+
+#: fietsboek/templates/profile.jinja2:69
+msgid "page.profile.tabbar.graphs"
+msgstr "Diagramme"
+
+#: fietsboek/templates/profile.jinja2:83
 msgid "page.profile.length"
 msgstr "Länge"
 
-#: fietsboek/templates/profile.jinja2:70
+#: fietsboek/templates/profile.jinja2:87
+msgid "page.profile.avg_length"
+msgstr "durchschnittliche Länge"
+
+#: fietsboek/templates/profile.jinja2:91
 msgid "page.profile.uphill"
 msgstr "Bergauf"
 
-#: fietsboek/templates/profile.jinja2:74
+#: fietsboek/templates/profile.jinja2:95
 msgid "page.profile.downhill"
 msgstr "Bergab"
 
-#: fietsboek/templates/profile.jinja2:78
+#: fietsboek/templates/profile.jinja2:99
 msgid "page.profile.moving_time"
 msgstr "Fahrzeit"
 
-#: fietsboek/templates/profile.jinja2:82
+#: fietsboek/templates/profile.jinja2:103
 msgid "page.profile.stopped_time"
 msgstr "Haltezeit"
 
-#: fietsboek/templates/profile.jinja2:86
+#: fietsboek/templates/profile.jinja2:107
+msgid "page.profile.avg_duration"
+msgstr "durchschnittliche Dauer"
+
+#: fietsboek/templates/profile.jinja2:111
 msgid "page.profile.max_speed"
 msgstr "maximale Geschwindigkeit"
 
-#: fietsboek/templates/profile.jinja2:90
+#: fietsboek/templates/profile.jinja2:115
 msgid "page.profile.avg_speed"
 msgstr "durchschnittliche Geschwindigkeit"
 
-#: fietsboek/templates/profile.jinja2:94
+#: fietsboek/templates/profile.jinja2:119
 msgid "page.profile.number_of_tracks"
 msgstr "Anzahl der Strecken"
 
-#: fietsboek/templates/profile.jinja2:100
+#: fietsboek/templates/profile.jinja2:125
 msgid "page.profile.longest_distance_track"
 msgstr "Weiteste Strecke"
 
-#: fietsboek/templates/profile.jinja2:105
+#: fietsboek/templates/profile.jinja2:130
 msgid "page.profile.shortest_distance_track"
 msgstr "Kürzeste Strecke"
 
-#: fietsboek/templates/profile.jinja2:110
+#: fietsboek/templates/profile.jinja2:135
 msgid "page.profile.longest_duration_track"
 msgstr "Am Längsten Dauernde Strecke"
 
-#: fietsboek/templates/profile.jinja2:115
+#: fietsboek/templates/profile.jinja2:140
 msgid "page.profile.shortest_duration_track"
 msgstr "Am Kürzesten Dauernde Strecke"
 
-#: fietsboek/templates/profile.jinja2:135
+#: fietsboek/templates/profile.jinja2:147
+msgid "page.profile.graph.km_per_month"
+msgstr "Kilometer pro Monat"
+
+#: fietsboek/templates/profile.jinja2:171
 msgid "page.profile.heatmap"
 msgstr "Heatmap"
 
-#: fietsboek/templates/profile.jinja2:140
+#: fietsboek/templates/profile.jinja2:176
 msgid "page.profile.tilehunt"
 msgstr "Kacheljäger"
 
 #: fietsboek/templates/request_password.jinja2:5
 msgid "page.request_password.title"
 msgstr "Passwortzurücksetzung Beantragen"
 
@@ -686,16 +726,15 @@
 
 #: fietsboek/templates/resend_verification.jinja2:5
 msgid "page.resend_verification.title"
 msgstr "Bestätigungsmail Erneut Senden"
 
 #: fietsboek/templates/resend_verification.jinja2:6
 msgid "page.resend_verification.info"
-msgstr ""
-"Hier kannst Du eine neue E-Mail zur Bestätigung Deines Kontos anfordern."
+msgstr "Hier kannst Du eine neue E-Mail zur Bestätigung Deines Kontos anfordern."
 
 #: fietsboek/templates/resend_verification.jinja2:12
 msgid "page.resend_verification.email"
 msgstr "E-Mail-Adresse"
 
 #: fietsboek/templates/resend_verification.jinja2:17
 msgid "page.resend_verification.request"
@@ -734,174 +773,194 @@
 msgstr "Passwort wiederholen"
 
 #: fietsboek/templates/user_data.jinja2:33
 msgid "page.my_profile.personal_data.save"
 msgstr "Speichern"
 
 #: fietsboek/templates/user_data.jinja2:38
+msgid "page.my_profile.session_logout.title"
+msgstr "Sitzungen abmelden"
+
+#: fietsboek/templates/user_data.jinja2:40
+msgid "page.my_profile.session_logout.explanation"
+msgstr ""
+"Mit dieser Funktion können alle Sitzungen beendet werden. Dies ist "
+"nützlich, wenn Du vergessen hast, dich auf einem fremden Gerät "
+"abzumelden. Beachte, dass Du dich erneut anmelden musst, wenn Du diese "
+"Funktion nutzt!"
+
+#: fietsboek/templates/user_data.jinja2:44
+msgid "page.my_profile.session_logout.button"
+msgstr "Alle Sitzungen beenden"
+
+#: fietsboek/templates/user_data.jinja2:49
 msgid "page.my_profile.friends"
 msgstr "Freunde"
 
-#: fietsboek/templates/user_data.jinja2:46
+#: fietsboek/templates/user_data.jinja2:57
 msgid "page.my_profile.unfriend"
 msgstr "Entfreunden"
 
-#: fietsboek/templates/user_data.jinja2:56
+#: fietsboek/templates/user_data.jinja2:67
 msgid "page.my_profile.accept_friend"
 msgstr "Annehmen"
 
-#: fietsboek/templates/user_data.jinja2:73
+#: fietsboek/templates/user_data.jinja2:84
 msgid "page.my_profile.friend_request_email"
 msgstr "E-Mail-Adresse des Freundes"
 
-#: fietsboek/templates/user_data.jinja2:77
+#: fietsboek/templates/user_data.jinja2:88
 msgid "page.my_profile.send_friend_request"
 msgstr "Freundschaftsanfrage senden"
 
-#: fietsboek/transformers/breaks.py:31
+#: fietsboek/transformers/breaks.py:32
 msgid "transformers.remove-breaks.title"
 msgstr "Pausen entfernen"
 
-#: fietsboek/transformers/breaks.py:35
+#: fietsboek/transformers/breaks.py:36
 msgid "transformers.remove-breaks.description"
 msgstr "Diese Transformation entfernt längere Pausen aus der Aufnahme."
 
-#: fietsboek/transformers/elevation.py:42
+#: fietsboek/transformers/elevation.py:43
 msgid "transformers.fix-null-elevation.title"
 msgstr "Nullhöhen beheben"
 
-#: fietsboek/transformers/elevation.py:46
+#: fietsboek/transformers/elevation.py:47
 msgid "transformers.fix-null-elevation.description"
 msgstr ""
 "Diese Transformation passt die Höhenangabe für Punkte an, bei denen die "
 "Höhenangabe fehlt."
 
-#: fietsboek/transformers/elevation.py:115
+#: fietsboek/transformers/elevation.py:116
 msgid "transformers.fix-elevation-jumps"
 msgstr "Höhensprünge beheben"
 
-#: fietsboek/transformers/elevation.py:119
+#: fietsboek/transformers/elevation.py:120
 msgid "transformers.fix-elevation-jumps.description"
 msgstr ""
 "Diese Transformation passt die Höhenangabe für Punkte an, bei denen die "
 "Höhe sprunghaft steigt oder fällt."
 
-#: fietsboek/views/account.py:53
+#: fietsboek/views/account.py:54
 msgid "flash.invalid_name"
 msgstr "Ungültiger Name"
 
-#: fietsboek/views/account.py:58
+#: fietsboek/views/account.py:59
 msgid "flash.invalid_email"
 msgstr "Ungültige E-Mail-Adresse"
 
-#: fietsboek/views/account.py:67
+#: fietsboek/views/account.py:69
 msgid "flash.a_confirmation_link_has_been_sent"
 msgstr "Ein Bestätigungslink wurde versandt"
 
-#: fietsboek/views/admin.py:48
+#: fietsboek/views/admin.py:49
 msgid "flash.badge_added"
 msgstr "Wappen hinzugefügt"
 
-#: fietsboek/views/admin.py:72
+#: fietsboek/views/admin.py:73
 msgid "flash.badge_modified"
 msgstr "Wappen bearbeitet"
 
-#: fietsboek/views/admin.py:92
+#: fietsboek/views/admin.py:93
 msgid "flash.badge_deleted"
 msgstr "Wappen gelöscht"
 
-#: fietsboek/views/default.py:115
+#: fietsboek/views/default.py:116
 msgid "flash.invalid_credentials"
 msgstr "Ungültige Nutzerdaten"
 
-#: fietsboek/views/default.py:119
+#: fietsboek/views/default.py:120
 msgid "flash.account_not_verified"
 msgstr "Konto noch nicht bestätigt"
 
-#: fietsboek/views/default.py:122
+#: fietsboek/views/default.py:123
 msgid "flash.logged_in"
 msgstr "Du bist nun angemeldet"
 
-#: fietsboek/views/default.py:142
+#: fietsboek/views/default.py:144
 msgid "flash.logged_out"
 msgstr "Du bist nun abgemeldet"
 
-#: fietsboek/views/default.py:172
+#: fietsboek/views/default.py:174
 msgid "flash.reset_invalid_email"
 msgstr "Ungültige E-Mail-Adresse angegeben"
 
-#: fietsboek/views/default.py:177
+#: fietsboek/views/default.py:179
 msgid "flash.password_token_generated"
 msgstr "Ein Link zum Zurücksetzen des Passworts wurde versandt"
 
-#: fietsboek/views/default.py:182
+#: fietsboek/views/default.py:184
 msgid "page.password_reset.email.subject"
 msgstr "Fietsboek Passwortzurücksetzung"
 
-#: fietsboek/views/default.py:185
+#: fietsboek/views/default.py:187
 msgid "page.password_reset.email.body"
 msgstr ""
 "Du kannst Dein Fietsboek-Passwort hier zurücksetzen: {}\n"
 "\n"
 "Falls Du keine Passwortzurücksetzung beantragt hast, dann ignoriere diese"
 " E-Mail."
 
-#: fietsboek/views/default.py:224
+#: fietsboek/views/default.py:226
 msgid "flash.resend_verification_email_fail"
 msgstr "Ungültige E-Mail-Adresse angegeben"
 
-#: fietsboek/views/default.py:229
+#: fietsboek/views/default.py:231
 msgid "flash.verification_token_generated"
 msgstr "Ein Link zur Bestätigung Deines Kontos wurde versandt"
 
-#: fietsboek/views/default.py:249
+#: fietsboek/views/default.py:251
 msgid "flash.token_expired"
 msgstr "Der Link ist nicht mehr gültig"
 
-#: fietsboek/views/default.py:255
+#: fietsboek/views/default.py:257
 msgid "flash.email_verified"
 msgstr "E-Mail-Adresse bestätigt"
 
-#: fietsboek/views/default.py:269
+#: fietsboek/views/default.py:271
 msgid "flash.password_updated"
 msgstr "Passwort aktualisiert"
 
-#: fietsboek/views/detail.py:155
+#: fietsboek/views/detail.py:162
 msgid "flash.track_deleted"
 msgstr "Strecke gelöscht"
 
-#: fietsboek/views/upload.py:52
+#: fietsboek/views/upload.py:53
 msgid "flash.no_file_selected"
 msgstr "Keine Datei ausgewählt"
 
-#: fietsboek/views/upload.py:62
+#: fietsboek/views/upload.py:66
 msgid "flash.invalid_file"
 msgstr "Ungültige GPX-Datei gesendet"
 
-#: fietsboek/views/upload.py:188
+#: fietsboek/views/upload.py:192
 msgid "flash.upload_success"
 msgstr "Hochladen erfolgreich"
 
-#: fietsboek/views/upload.py:207
+#: fietsboek/views/upload.py:211
 msgid "flash.upload_cancelled"
 msgstr "Hochladen abgebrochen"
 
-#: fietsboek/views/user_data.py:60
+#: fietsboek/views/user_data.py:67
 msgid "flash.personal_data_updated"
 msgstr "Persönliche Daten wurden gespeichert"
 
-#: fietsboek/views/user_data.py:78
+#: fietsboek/views/user_data.py:86
 msgid "flash.friend_not_found"
 msgstr "Das angegebene Konto wurde nicht gefunden"
 
-#: fietsboek/views/user_data.py:84
+#: fietsboek/views/user_data.py:92
 msgid "flash.friend_already_exists"
 msgstr "Dieser Freund existiert bereits"
 
-#: fietsboek/views/user_data.py:92
+#: fietsboek/views/user_data.py:100
 msgid "flash.friend_added"
 msgstr "Freund hinzugefügt"
 
-#: fietsboek/views/user_data.py:102
+#: fietsboek/views/user_data.py:110
 msgid "flash.friend_request_sent"
 msgstr "Freundschaftsanfrage gesendet"
 
+#: fietsboek/views/user_data.py:196
+msgid "flash.sessions_logged_out"
+msgstr "Die Sitzungen wurden beendet. Melde Dich bitte erneut an, um fortzufahren."
+
```

### Comparing `fietsboek-0.8.0/fietsboek/locale/en/LC_MESSAGES/messages.mo` & `fietsboek-0.9.0/fietsboek/locale/en/LC_MESSAGES/messages.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-31 20:46+0200\n"
+"POT-Creation-Date: 2024-04-06 21:57+0200\n"
 "PO-Revision-Date: 2023-04-03 20:42+0200\n"
 "Last-Translator: \n"
 "Language: en\n"
 "Language-Team: en <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "email.verify.text"
 msgstr ""
 "To verify your Fietsboek account, please use this link: {}\n"
 "\n"
 "If you did not create an account, ignore this email."
 
@@ -84,14 +84,17 @@
 
 msgid "flash.resend_verification_email_fail"
 msgstr "Invalid email address provided"
 
 msgid "flash.reset_invalid_email"
 msgstr "Invalid email address provided"
 
+msgid "flash.sessions_logged_out"
+msgstr "All sessions have been logged out. Please log in again to continue."
+
 msgid "flash.token_expired"
 msgstr "The link has expired"
 
 msgid "flash.track_deleted"
 msgstr "Track has been deleted"
 
 msgid "flash.upload_cancelled"
@@ -126,14 +129,23 @@
 
 msgid "page.browse.download_multiple"
 msgstr "Download selected"
 
 msgid "page.browse.filter.date_boundaries"
 msgstr "Date limits"
 
+msgid "page.browse.filter.favourite.all"
+msgstr "All Tracks"
+
+msgid "page.browse.filter.favourite.no"
+msgstr "No Favourites"
+
+msgid "page.browse.filter.favourite.yes"
+msgstr "Only Favourites"
+
 msgid "page.browse.filter.friends_tracks_only"
 msgstr "Show only tracks of my friends"
 
 msgid "page.browse.filter.length_boundaries"
 msgstr "Length limits"
 
 msgid "page.browse.filter.length_maximum"
@@ -389,14 +401,26 @@
 
 msgid "page.my_profile.personal_data.save"
 msgstr "Save"
 
 msgid "page.my_profile.send_friend_request"
 msgstr "Send friend request"
 
+msgid "page.my_profile.session_logout.button"
+msgstr "Close all sessions"
+
+msgid "page.my_profile.session_logout.explanation"
+msgstr ""
+"With this functionality, you can force all of your current sessions to be "
+"logged out. This is useful when you forgot to log out on a foreign device. "
+"Note that you will have to log in again after using this function."
+
+msgid "page.my_profile.session_logout.title"
+msgstr "Invalidate sessions"
+
 msgid "page.my_profile.title"
 msgstr "My Profile"
 
 msgid "page.my_profile.unfriend"
 msgstr "Unfriend"
 
 msgid "page.navbar.admin"
@@ -461,20 +485,29 @@
 
 msgid "page.password_reset.reset"
 msgstr "Reset"
 
 msgid "page.password_reset.title"
 msgstr "Reset Your Password"
 
+msgid "page.profile.avg_duration"
+msgstr "Average Duration"
+
+msgid "page.profile.avg_length"
+msgstr "Average Length"
+
 msgid "page.profile.avg_speed"
 msgstr "Average Speed"
 
 msgid "page.profile.downhill"
 msgstr "Downhill"
 
+msgid "page.profile.graph.km_per_month"
+msgstr "Kilometers per month"
+
 msgid "page.profile.heatmap"
 msgstr "Heat Map"
 
 msgid "page.profile.length"
 msgstr "Length"
 
 msgid "page.profile.longest_distance_track"
@@ -497,14 +530,20 @@
 
 msgid "page.profile.shortest_duration_track"
 msgstr "Quickest Track"
 
 msgid "page.profile.stopped_time"
 msgstr "Stopped Time"
 
+msgid "page.profile.tabbar.graphs"
+msgstr "Graphs"
+
+msgid "page.profile.tabbar.overview"
+msgstr "Overview"
+
 msgid "page.profile.tilehunt"
 msgstr "Tilehunt"
 
 msgid "page.profile.uphill"
 msgstr "Uphill"
 
 msgid "page.request_password.email"
@@ -550,14 +589,17 @@
 
 msgid "page.track.form.image_description_modal"
 msgstr "Image description"
 
 msgid "page.track.form.image_description_modal.save"
 msgstr "Apply"
 
+msgid "page.track.form.image_uploads_disabled"
+msgstr "Image uploads are disabled on this Fietsboek"
+
 msgid "page.track.form.remove_image"
 msgstr "Remove image"
 
 msgid "page.track.form.select_images"
 msgstr "Select images"
 
 msgid "page.track.form.tagged_people"
@@ -633,14 +675,17 @@
 
 msgid "tooltip.table.max_speed"
 msgstr "Max Speed"
 
 msgid "tooltip.table.moving_time"
 msgstr "Moving Time"
 
+msgid "tooltip.table.people"
+msgstr "# People"
+
 msgid "tooltip.table.stopped_time"
 msgstr "Stopped Time"
 
 msgid "tooltip.table.uphill"
 msgstr "Uphill"
 
 msgid "transformers.fix-elevation-jumps"
```

### Comparing `fietsboek-0.8.0/fietsboek/locale/en/LC_MESSAGES/messages.po` & `fietsboek-0.9.0/fietsboek/locale/en/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,69 +3,73 @@
 # This file is distributed under the same license as the Fietsboek project.
 # Daniel Schadt, 2022.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-31 20:46+0200\n"
+"POT-Creation-Date: 2024-04-06 21:57+0200\n"
 "PO-Revision-Date: 2023-04-03 20:42+0200\n"
 "Last-Translator: \n"
 "Language: en\n"
 "Language-Team: en <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
+"Generated-By: Babel 2.14.0\n"
 
-#: fietsboek/actions.py:250
+#: fietsboek/actions.py:267
 msgid "email.verify_mail.subject"
 msgstr "Fietsboek Account Verification"
 
-#: fietsboek/actions.py:253
+#: fietsboek/actions.py:270
 msgid "email.verify.text"
 msgstr ""
 "To verify your Fietsboek account, please use this link: {}\n"
 "\n"
 "If you did not create an account, ignore this email."
 
-#: fietsboek/util.py:304
+#: fietsboek/util.py:310
 msgid "password_constraint.mismatch"
 msgstr "Passwords don't match"
 
-#: fietsboek/util.py:306
+#: fietsboek/util.py:312
 msgid "password_constraint.length"
 msgstr "Password not long enough"
 
-#: fietsboek/models/track.py:579
+#: fietsboek/models/track.py:603
 msgid "tooltip.table.length"
 msgstr "Length"
 
-#: fietsboek/models/track.py:580
+#: fietsboek/models/track.py:604
+msgid "tooltip.table.people"
+msgstr "# People"
+
+#: fietsboek/models/track.py:605
 msgid "tooltip.table.uphill"
 msgstr "Uphill"
 
-#: fietsboek/models/track.py:581
+#: fietsboek/models/track.py:606
 msgid "tooltip.table.downhill"
 msgstr "Downhill"
 
-#: fietsboek/models/track.py:582
+#: fietsboek/models/track.py:607
 msgid "tooltip.table.moving_time"
 msgstr "Moving Time"
 
-#: fietsboek/models/track.py:583
+#: fietsboek/models/track.py:608
 msgid "tooltip.table.stopped_time"
 msgstr "Stopped Time"
 
-#: fietsboek/models/track.py:585
+#: fietsboek/models/track.py:610
 msgid "tooltip.table.max_speed"
 msgstr "Max Speed"
 
-#: fietsboek/models/track.py:589
+#: fietsboek/models/track.py:614
 msgid "tooltip.table.avg_speed"
 msgstr "Average Speed"
 
 #: fietsboek/templates/admin.jinja2:5
 msgid "page.admin.title"
 msgstr "Administration"
 
@@ -129,117 +133,129 @@
 msgid "page.browse.filter.type.organic"
 msgstr "Recording (organic)"
 
 #: fietsboek/templates/browse.jinja2:74
 msgid "page.browse.filter.type.synthetic"
 msgstr "Template (synthetic)"
 
-#: fietsboek/templates/browse.jinja2:86
+#: fietsboek/templates/browse.jinja2:82
+msgid "page.browse.filter.favourite.all"
+msgstr "All Tracks"
+
+#: fietsboek/templates/browse.jinja2:83
+msgid "page.browse.filter.favourite.yes"
+msgstr "Only Favourites"
+
+#: fietsboek/templates/browse.jinja2:84
+msgid "page.browse.filter.favourite.no"
+msgstr "No Favourites"
+
+#: fietsboek/templates/browse.jinja2:97
 msgid "page.browse.filter.my_tracks.only"
 msgstr "Show only my own tracks"
 
-#: fietsboek/templates/browse.jinja2:87
+#: fietsboek/templates/browse.jinja2:98
 msgid "page.browse.filter.friends_tracks_only"
 msgstr "Show only tracks of my friends"
 
-#: fietsboek/templates/browse.jinja2:88
+#: fietsboek/templates/browse.jinja2:99
 msgid "page.browse.filter.me_tagged_only"
 msgstr "Show only tracks in which I'm tagged"
 
-#: fietsboek/templates/browse.jinja2:98
+#: fietsboek/templates/browse.jinja2:109
 msgid "page.browse.filters.apply"
 msgstr "Apply filters"
 
-#: fietsboek/templates/browse.jinja2:102
+#: fietsboek/templates/browse.jinja2:113
 msgid "page.browse.filters.clear_all"
 msgstr "Remove filters"
 
-#: fietsboek/templates/browse.jinja2:105
+#: fietsboek/templates/browse.jinja2:116
 msgid "page.browse.filters.expand_advanced"
 msgstr "Advanced"
 
-#: fietsboek/templates/browse.jinja2:110 fietsboek/templates/browse.jinja2:111
+#: fietsboek/templates/browse.jinja2:121 fietsboek/templates/browse.jinja2:122
 msgid "page.browse.sort.date"
 msgstr "Sort by date"
 
-#: fietsboek/templates/browse.jinja2:112 fietsboek/templates/browse.jinja2:113
+#: fietsboek/templates/browse.jinja2:123 fietsboek/templates/browse.jinja2:124
 msgid "page.browse.sort.length"
 msgstr "Sort by length"
 
-#: fietsboek/templates/browse.jinja2:114 fietsboek/templates/browse.jinja2:115
+#: fietsboek/templates/browse.jinja2:125 fietsboek/templates/browse.jinja2:126
 msgid "page.browse.sort.duration"
 msgstr "Sort by duration"
 
-#: fietsboek/templates/browse.jinja2:132
+#: fietsboek/templates/browse.jinja2:148
 msgid "page.browse.organic_tooltip"
 msgstr "This is a recording of a track"
 
-#: fietsboek/templates/browse.jinja2:134
+#: fietsboek/templates/browse.jinja2:150
 msgid "page.browse.synthetic_tooltip"
 msgstr "This is a pre-planned track"
 
-#: fietsboek/templates/browse.jinja2:142 fietsboek/templates/details.jinja2:90
+#: fietsboek/templates/browse.jinja2:158 fietsboek/templates/details.jinja2:103
 #: fietsboek/templates/profile.jinja2:15
 msgid "page.details.date"
 msgstr "Date"
 
-#: fietsboek/templates/browse.jinja2:144 fietsboek/templates/details.jinja2:104
+#: fietsboek/templates/browse.jinja2:160 fietsboek/templates/details.jinja2:117
 #: fietsboek/templates/profile.jinja2:17
 msgid "page.details.length"
 msgstr "Length"
 
-#: fietsboek/templates/browse.jinja2:149 fietsboek/templates/details.jinja2:95
+#: fietsboek/templates/browse.jinja2:165 fietsboek/templates/details.jinja2:108
 #: fietsboek/templates/profile.jinja2:21
 msgid "page.details.start_time"
 msgstr "Record Start"
 
-#: fietsboek/templates/browse.jinja2:151 fietsboek/templates/details.jinja2:99
+#: fietsboek/templates/browse.jinja2:167 fietsboek/templates/details.jinja2:112
 #: fietsboek/templates/profile.jinja2:23
 msgid "page.details.end_time"
 msgstr "Record End"
 
-#: fietsboek/templates/browse.jinja2:156 fietsboek/templates/details.jinja2:108
+#: fietsboek/templates/browse.jinja2:172 fietsboek/templates/details.jinja2:121
 #: fietsboek/templates/profile.jinja2:27
 msgid "page.details.uphill"
 msgstr "Uphill"
 
-#: fietsboek/templates/browse.jinja2:158 fietsboek/templates/details.jinja2:112
+#: fietsboek/templates/browse.jinja2:174 fietsboek/templates/details.jinja2:125
 #: fietsboek/templates/profile.jinja2:29
 msgid "page.details.downhill"
 msgstr "Downhill"
 
-#: fietsboek/templates/browse.jinja2:163 fietsboek/templates/details.jinja2:117
+#: fietsboek/templates/browse.jinja2:179 fietsboek/templates/details.jinja2:130
 #: fietsboek/templates/profile.jinja2:33
 msgid "page.details.moving_time"
 msgstr "Moving Time"
 
-#: fietsboek/templates/browse.jinja2:165 fietsboek/templates/details.jinja2:121
+#: fietsboek/templates/browse.jinja2:181 fietsboek/templates/details.jinja2:134
 #: fietsboek/templates/profile.jinja2:35
 msgid "page.details.stopped_time"
 msgstr "Stopped Time"
 
-#: fietsboek/templates/browse.jinja2:169 fietsboek/templates/details.jinja2:125
+#: fietsboek/templates/browse.jinja2:185 fietsboek/templates/details.jinja2:138
 #: fietsboek/templates/profile.jinja2:39
 msgid "page.details.max_speed"
 msgstr "Max Speed"
 
-#: fietsboek/templates/browse.jinja2:171 fietsboek/templates/details.jinja2:129
+#: fietsboek/templates/browse.jinja2:187 fietsboek/templates/details.jinja2:142
 #: fietsboek/templates/profile.jinja2:41
 msgid "page.details.avg_speed"
 msgstr "Average Speed"
 
-#: fietsboek/templates/browse.jinja2:189
+#: fietsboek/templates/browse.jinja2:205
 msgid "page.browse.download_multiple"
 msgstr "Download selected"
 
-#: fietsboek/templates/browse.jinja2:191
+#: fietsboek/templates/browse.jinja2:207
 msgid "page.browse.no_results"
 msgstr "No results matching the filters were found."
 
-#: fietsboek/templates/browse.jinja2:193
+#: fietsboek/templates/browse.jinja2:209
 msgid "page.browse.no_tracks"
 msgstr "You currently do not have access to any tracks. Try logging in."
 
 #: fietsboek/templates/create_account.jinja2:5
 msgid "page.create_account.title"
 msgstr "Create Account"
 
@@ -275,96 +291,96 @@
 msgid "page.create_account.repeat_password"
 msgstr "Repeat password"
 
 #: fietsboek/templates/create_account.jinja2:54
 msgid "page.create_account.create"
 msgstr "Create"
 
-#: fietsboek/templates/details.jinja2:6
+#: fietsboek/templates/details.jinja2:7
 msgid "page.details.title"
 msgstr "Track Details"
 
-#: fietsboek/templates/details.jinja2:9
+#: fietsboek/templates/details.jinja2:20
 msgid "page.details.edit"
 msgstr "Edit"
 
-#: fietsboek/templates/details.jinja2:10
+#: fietsboek/templates/details.jinja2:21
 msgid "page.details.share"
 msgstr "Share"
 
-#: fietsboek/templates/details.jinja2:11
+#: fietsboek/templates/details.jinja2:22
 msgid "page.details.delete"
 msgstr "Delete"
 
-#: fietsboek/templates/details.jinja2:17
+#: fietsboek/templates/details.jinja2:28
 msgid "page.details.sharelink.title"
 msgstr "Share Link"
 
-#: fietsboek/templates/details.jinja2:21
+#: fietsboek/templates/details.jinja2:32
 msgid "page.details.sharelink.info"
 msgstr "Everyone with access to this link can view the track!"
 
-#: fietsboek/templates/details.jinja2:28
+#: fietsboek/templates/details.jinja2:39
 msgid "page.details.sharelink.invalidate"
 msgstr "Invalidate link"
 
-#: fietsboek/templates/details.jinja2:30
+#: fietsboek/templates/details.jinja2:41
 msgid "page.details.sharelink.close"
 msgstr "Close"
 
-#: fietsboek/templates/details.jinja2:40
+#: fietsboek/templates/details.jinja2:51
 msgid "page.details.delete.title"
 msgstr "Delete Track"
 
-#: fietsboek/templates/details.jinja2:44
+#: fietsboek/templates/details.jinja2:55
 msgid "page.details.delete.info"
 msgstr "Deleting this track will remove all associated information with it!"
 
-#: fietsboek/templates/details.jinja2:49
+#: fietsboek/templates/details.jinja2:60
 msgid "page.details.delete.delete"
 msgstr "Delete"
 
-#: fietsboek/templates/details.jinja2:51
+#: fietsboek/templates/details.jinja2:62
 msgid "page.details.delete.close"
 msgstr "Abort"
 
-#: fietsboek/templates/details.jinja2:70
+#: fietsboek/templates/details.jinja2:81
 msgid "page.details.tags"
 msgstr "Tagged as"
 
-#: fietsboek/templates/details.jinja2:80 fietsboek/templates/edit.jinja2:10
+#: fietsboek/templates/details.jinja2:91 fietsboek/templates/edit.jinja2:10
 #: fietsboek/templates/finish_upload.jinja2:10
 msgid "page.noscript"
 msgstr "JavaScript is disabled, please enable JavaScript"
 
-#: fietsboek/templates/details.jinja2:85
+#: fietsboek/templates/details.jinja2:97
 msgid "page.details.download"
 msgstr "Download Tour"
 
-#: fietsboek/templates/details.jinja2:174
+#: fietsboek/templates/details.jinja2:187
 msgid "page.details.comments"
 msgstr "Comments"
 
-#: fietsboek/templates/details.jinja2:178
+#: fietsboek/templates/details.jinja2:191
 msgid "page.details.comments.author"
 msgstr "Comment by {}"
 
-#: fietsboek/templates/details.jinja2:195
+#: fietsboek/templates/details.jinja2:208
 msgid "page.details.comments.new.title"
 msgstr "Create a new comment"
 
-#: fietsboek/templates/details.jinja2:198
+#: fietsboek/templates/details.jinja2:211
 msgid "page.details.comments.new.input_title"
 msgstr "Title"
 
-#: fietsboek/templates/details.jinja2:199
+#: fietsboek/templates/details.jinja2:212
 msgid "page.details.comments.new.input_comment"
 msgstr "Comment"
 
-#: fietsboek/templates/details.jinja2:202
+#: fietsboek/templates/details.jinja2:215
 msgid "page.details.comments.new.submit"
 msgstr "Submit"
 
 #: fietsboek/templates/edit.jinja2:8
 msgid "page.edit.title"
 msgstr "Edit Track"
 
@@ -438,40 +454,44 @@
 msgid "page.track.form.tagged_people"
 msgstr "Tagged People"
 
 #: fietsboek/templates/edit_form.jinja2:70
 msgid "page.track.form.add_friend"
 msgstr "Search friends"
 
-#: fietsboek/templates/edit_form.jinja2:90
+#: fietsboek/templates/edit_form.jinja2:92
 msgid "page.track.form.badges"
 msgstr "Badges"
 
-#: fietsboek/templates/edit_form.jinja2:101
+#: fietsboek/templates/edit_form.jinja2:103
 msgid "page.track.form.description"
 msgstr "Description"
 
-#: fietsboek/templates/edit_form.jinja2:108
-#: fietsboek/templates/edit_form.jinja2:122
+#: fietsboek/templates/edit_form.jinja2:110
+#: fietsboek/templates/edit_form.jinja2:131
 msgid "page.track.form.remove_image"
 msgstr "Remove image"
 
-#: fietsboek/templates/edit_form.jinja2:117
+#: fietsboek/templates/edit_form.jinja2:120
 msgid "page.track.form.select_images"
 msgstr "Select images"
 
-#: fietsboek/templates/edit_form.jinja2:133
+#: fietsboek/templates/edit_form.jinja2:124
+msgid "page.track.form.image_uploads_disabled"
+msgstr "Image uploads are disabled on this Fietsboek"
+
+#: fietsboek/templates/edit_form.jinja2:142
 msgid "page.track.form.image_description_modal"
 msgstr "Image description"
 
-#: fietsboek/templates/edit_form.jinja2:140
+#: fietsboek/templates/edit_form.jinja2:149
 msgid "page.track.form.image_description_modal.save"
 msgstr "Apply"
 
-#: fietsboek/templates/edit_form.jinja2:166
+#: fietsboek/templates/edit_form.jinja2:175
 msgid "page.track.form.transformer.enable"
 msgstr "Apply transformation"
 
 #: fietsboek/templates/finish_upload.jinja2:8
 #: fietsboek/templates/upload.jinja2:6
 msgid "page.upload.title"
 msgstr "Upload"
@@ -490,21 +510,21 @@
 msgstr "Home"
 
 #: fietsboek/templates/home.jinja2:17
 msgid "page.home.unfinished_uploads"
 msgstr "You have unfinished uploads. Click on the links below to resume them:"
 
 #: fietsboek/templates/home.jinja2:31 fietsboek/templates/home.jinja2:38
-#: fietsboek/templates/home.jinja2:56
+#: fietsboek/templates/home.jinja2:66
 msgid "page.home.summary.track"
 msgid_plural "page.home.summary.tracks"
 msgstr[0] "%(num)d track"
 msgstr[1] "%(num)d tracks"
 
-#: fietsboek/templates/home.jinja2:56
+#: fietsboek/templates/home.jinja2:66
 msgid "page.home.total"
 msgstr "Total"
 
 #: fietsboek/templates/layout.jinja2:43
 msgid "page.navbar.toggle"
 msgstr "Toggle navigation"
 
@@ -600,67 +620,87 @@
 msgid "page.password_reset.password_mismatch"
 msgstr "Passwords must match"
 
 #: fietsboek/templates/password_reset.jinja2:30
 msgid "page.password_reset.reset"
 msgstr "Reset"
 
-#: fietsboek/templates/profile.jinja2:66
+#: fietsboek/templates/profile.jinja2:64
+msgid "page.profile.tabbar.overview"
+msgstr "Overview"
+
+#: fietsboek/templates/profile.jinja2:69
+msgid "page.profile.tabbar.graphs"
+msgstr "Graphs"
+
+#: fietsboek/templates/profile.jinja2:83
 msgid "page.profile.length"
 msgstr "Length"
 
-#: fietsboek/templates/profile.jinja2:70
+#: fietsboek/templates/profile.jinja2:87
+msgid "page.profile.avg_length"
+msgstr "Average Length"
+
+#: fietsboek/templates/profile.jinja2:91
 msgid "page.profile.uphill"
 msgstr "Uphill"
 
-#: fietsboek/templates/profile.jinja2:74
+#: fietsboek/templates/profile.jinja2:95
 msgid "page.profile.downhill"
 msgstr "Downhill"
 
-#: fietsboek/templates/profile.jinja2:78
+#: fietsboek/templates/profile.jinja2:99
 msgid "page.profile.moving_time"
 msgstr "Moving Time"
 
-#: fietsboek/templates/profile.jinja2:82
+#: fietsboek/templates/profile.jinja2:103
 msgid "page.profile.stopped_time"
 msgstr "Stopped Time"
 
-#: fietsboek/templates/profile.jinja2:86
+#: fietsboek/templates/profile.jinja2:107
+msgid "page.profile.avg_duration"
+msgstr "Average Duration"
+
+#: fietsboek/templates/profile.jinja2:111
 msgid "page.profile.max_speed"
 msgstr "Max Speed"
 
-#: fietsboek/templates/profile.jinja2:90
+#: fietsboek/templates/profile.jinja2:115
 msgid "page.profile.avg_speed"
 msgstr "Average Speed"
 
-#: fietsboek/templates/profile.jinja2:94
+#: fietsboek/templates/profile.jinja2:119
 msgid "page.profile.number_of_tracks"
 msgstr "Number of tracks"
 
-#: fietsboek/templates/profile.jinja2:100
+#: fietsboek/templates/profile.jinja2:125
 msgid "page.profile.longest_distance_track"
 msgstr "Longest Track"
 
-#: fietsboek/templates/profile.jinja2:105
+#: fietsboek/templates/profile.jinja2:130
 msgid "page.profile.shortest_distance_track"
 msgstr "Shortest Track"
 
-#: fietsboek/templates/profile.jinja2:110
+#: fietsboek/templates/profile.jinja2:135
 msgid "page.profile.longest_duration_track"
 msgstr "Most Time-Consuming Track"
 
-#: fietsboek/templates/profile.jinja2:115
+#: fietsboek/templates/profile.jinja2:140
 msgid "page.profile.shortest_duration_track"
 msgstr "Quickest Track"
 
-#: fietsboek/templates/profile.jinja2:135
+#: fietsboek/templates/profile.jinja2:147
+msgid "page.profile.graph.km_per_month"
+msgstr "Kilometers per month"
+
+#: fietsboek/templates/profile.jinja2:171
 msgid "page.profile.heatmap"
 msgstr "Heat Map"
 
-#: fietsboek/templates/profile.jinja2:140
+#: fietsboek/templates/profile.jinja2:176
 msgid "page.profile.tilehunt"
 msgstr "Tilehunt"
 
 #: fietsboek/templates/request_password.jinja2:5
 msgid "page.request_password.title"
 msgstr "Request a Password Reset"
 
@@ -727,169 +767,189 @@
 msgstr "Repeat password"
 
 #: fietsboek/templates/user_data.jinja2:33
 msgid "page.my_profile.personal_data.save"
 msgstr "Save"
 
 #: fietsboek/templates/user_data.jinja2:38
+msgid "page.my_profile.session_logout.title"
+msgstr "Invalidate sessions"
+
+#: fietsboek/templates/user_data.jinja2:40
+msgid "page.my_profile.session_logout.explanation"
+msgstr ""
+"With this functionality, you can force all of your current sessions to be"
+" logged out. This is useful when you forgot to log out on a foreign "
+"device. Note that you will have to log in again after using this "
+"function."
+
+#: fietsboek/templates/user_data.jinja2:44
+msgid "page.my_profile.session_logout.button"
+msgstr "Close all sessions"
+
+#: fietsboek/templates/user_data.jinja2:49
 msgid "page.my_profile.friends"
 msgstr "Friends"
 
-#: fietsboek/templates/user_data.jinja2:46
+#: fietsboek/templates/user_data.jinja2:57
 msgid "page.my_profile.unfriend"
 msgstr "Unfriend"
 
-#: fietsboek/templates/user_data.jinja2:56
+#: fietsboek/templates/user_data.jinja2:67
 msgid "page.my_profile.accept_friend"
 msgstr "Accept"
 
-#: fietsboek/templates/user_data.jinja2:73
+#: fietsboek/templates/user_data.jinja2:84
 msgid "page.my_profile.friend_request_email"
 msgstr "Email of the friend"
 
-#: fietsboek/templates/user_data.jinja2:77
+#: fietsboek/templates/user_data.jinja2:88
 msgid "page.my_profile.send_friend_request"
 msgstr "Send friend request"
 
-#: fietsboek/transformers/breaks.py:31
+#: fietsboek/transformers/breaks.py:32
 msgid "transformers.remove-breaks.title"
 msgstr "Remove breaks"
 
-#: fietsboek/transformers/breaks.py:35
+#: fietsboek/transformers/breaks.py:36
 msgid "transformers.remove-breaks.description"
 msgstr "This transformer removes long breaks from the recording"
 
-#: fietsboek/transformers/elevation.py:42
+#: fietsboek/transformers/elevation.py:43
 msgid "transformers.fix-null-elevation.title"
 msgstr "Fix null elevation"
 
-#: fietsboek/transformers/elevation.py:46
+#: fietsboek/transformers/elevation.py:47
 msgid "transformers.fix-null-elevation.description"
 msgstr "This transformer fixes the elevation of points whose elevation is unset."
 
-#: fietsboek/transformers/elevation.py:115
+#: fietsboek/transformers/elevation.py:116
 msgid "transformers.fix-elevation-jumps"
 msgstr "Fix elevation jumps"
 
-#: fietsboek/transformers/elevation.py:119
+#: fietsboek/transformers/elevation.py:120
 msgid "transformers.fix-elevation-jumps.description"
 msgstr "This transformer fixes abrupt jumps in the elevation value."
 
-#: fietsboek/views/account.py:53
+#: fietsboek/views/account.py:54
 msgid "flash.invalid_name"
 msgstr "Invalid name"
 
-#: fietsboek/views/account.py:58
+#: fietsboek/views/account.py:59
 msgid "flash.invalid_email"
 msgstr "Invalid email"
 
-#: fietsboek/views/account.py:67
+#: fietsboek/views/account.py:69
 msgid "flash.a_confirmation_link_has_been_sent"
 msgstr "A confirmation link has been sent"
 
-#: fietsboek/views/admin.py:48
+#: fietsboek/views/admin.py:49
 msgid "flash.badge_added"
 msgstr "Badge has been added"
 
-#: fietsboek/views/admin.py:72
+#: fietsboek/views/admin.py:73
 msgid "flash.badge_modified"
 msgstr "Badge has been modified"
 
-#: fietsboek/views/admin.py:92
+#: fietsboek/views/admin.py:93
 msgid "flash.badge_deleted"
 msgstr "Badge has been deleted"
 
-#: fietsboek/views/default.py:115
+#: fietsboek/views/default.py:116
 msgid "flash.invalid_credentials"
 msgstr "Invalid login credentials"
 
-#: fietsboek/views/default.py:119
+#: fietsboek/views/default.py:120
 msgid "flash.account_not_verified"
 msgstr "Your account is not verified yet"
 
-#: fietsboek/views/default.py:122
+#: fietsboek/views/default.py:123
 msgid "flash.logged_in"
 msgstr "You are now logged in"
 
-#: fietsboek/views/default.py:142
+#: fietsboek/views/default.py:144
 msgid "flash.logged_out"
 msgstr "You have been logged out"
 
-#: fietsboek/views/default.py:172
+#: fietsboek/views/default.py:174
 msgid "flash.reset_invalid_email"
 msgstr "Invalid email address provided"
 
-#: fietsboek/views/default.py:177
+#: fietsboek/views/default.py:179
 msgid "flash.password_token_generated"
 msgstr "A password reset email has been sent"
 
-#: fietsboek/views/default.py:182
+#: fietsboek/views/default.py:184
 msgid "page.password_reset.email.subject"
 msgstr "Fietsboek Password Reset"
 
-#: fietsboek/views/default.py:185
+#: fietsboek/views/default.py:187
 msgid "page.password_reset.email.body"
 msgstr ""
 "You can reset your Fietsboek password here: {}\n"
 "\n"
 "If you did not request a password reset, ignore this email."
 
-#: fietsboek/views/default.py:224
+#: fietsboek/views/default.py:226
 msgid "flash.resend_verification_email_fail"
 msgstr "Invalid email address provided"
 
-#: fietsboek/views/default.py:229
+#: fietsboek/views/default.py:231
 msgid "flash.verification_token_generated"
 msgstr "A verification email has been sent"
 
-#: fietsboek/views/default.py:249
+#: fietsboek/views/default.py:251
 msgid "flash.token_expired"
 msgstr "The link has expired"
 
-#: fietsboek/views/default.py:255
+#: fietsboek/views/default.py:257
 msgid "flash.email_verified"
 msgstr "Your email address has been verified"
 
-#: fietsboek/views/default.py:269
+#: fietsboek/views/default.py:271
 msgid "flash.password_updated"
 msgstr "Password has been updated"
 
-#: fietsboek/views/detail.py:155
+#: fietsboek/views/detail.py:162
 msgid "flash.track_deleted"
 msgstr "Track has been deleted"
 
-#: fietsboek/views/upload.py:52
+#: fietsboek/views/upload.py:53
 msgid "flash.no_file_selected"
 msgstr "No file selected"
 
-#: fietsboek/views/upload.py:62
+#: fietsboek/views/upload.py:66
 msgid "flash.invalid_file"
 msgstr "Invalid GPX file selected"
 
-#: fietsboek/views/upload.py:188
+#: fietsboek/views/upload.py:192
 msgid "flash.upload_success"
 msgstr "Upload successful"
 
-#: fietsboek/views/upload.py:207
+#: fietsboek/views/upload.py:211
 msgid "flash.upload_cancelled"
 msgstr "Upload cancelled"
 
-#: fietsboek/views/user_data.py:60
+#: fietsboek/views/user_data.py:67
 msgid "flash.personal_data_updated"
 msgstr "Personal data has been updated"
 
-#: fietsboek/views/user_data.py:78
+#: fietsboek/views/user_data.py:86
 msgid "flash.friend_not_found"
 msgstr "The friend was not found"
 
-#: fietsboek/views/user_data.py:84
+#: fietsboek/views/user_data.py:92
 msgid "flash.friend_already_exists"
 msgstr "Friend already exists"
 
-#: fietsboek/views/user_data.py:92
+#: fietsboek/views/user_data.py:100
 msgid "flash.friend_added"
 msgstr "Friend has been added"
 
-#: fietsboek/views/user_data.py:102
+#: fietsboek/views/user_data.py:110
 msgid "flash.friend_request_sent"
 msgstr "Friend request sent"
 
+#: fietsboek/views/user_data.py:196
+msgid "flash.sessions_logged_out"
+msgstr "All sessions have been logged out. Please log in again to continue."
+
```

### Comparing `fietsboek-0.8.0/fietsboek/locale/fietslog.pot` & `fietsboek-0.9.0/fietsboek/locale/fietslog.pot`

 * *Files 2% similar despite different names*

```diff
@@ -1,67 +1,71 @@
 # Translations template for PROJECT.
-# Copyright (C) 2023 ORGANIZATION
+# Copyright (C) 2024 ORGANIZATION
 # This file is distributed under the same license as the PROJECT project.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-31 20:46+0200\n"
+"POT-Creation-Date: 2024-04-06 21:57+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
+"Generated-By: Babel 2.14.0\n"
 
-#: fietsboek/actions.py:250
+#: fietsboek/actions.py:267
 msgid "email.verify_mail.subject"
 msgstr ""
 
-#: fietsboek/actions.py:253
+#: fietsboek/actions.py:270
 msgid "email.verify.text"
 msgstr ""
 
-#: fietsboek/util.py:304
+#: fietsboek/util.py:310
 msgid "password_constraint.mismatch"
 msgstr ""
 
-#: fietsboek/util.py:306
+#: fietsboek/util.py:312
 msgid "password_constraint.length"
 msgstr ""
 
-#: fietsboek/models/track.py:579
+#: fietsboek/models/track.py:603
 msgid "tooltip.table.length"
 msgstr ""
 
-#: fietsboek/models/track.py:580
+#: fietsboek/models/track.py:604
+msgid "tooltip.table.people"
+msgstr ""
+
+#: fietsboek/models/track.py:605
 msgid "tooltip.table.uphill"
 msgstr ""
 
-#: fietsboek/models/track.py:581
+#: fietsboek/models/track.py:606
 msgid "tooltip.table.downhill"
 msgstr ""
 
-#: fietsboek/models/track.py:582
+#: fietsboek/models/track.py:607
 msgid "tooltip.table.moving_time"
 msgstr ""
 
-#: fietsboek/models/track.py:583
+#: fietsboek/models/track.py:608
 msgid "tooltip.table.stopped_time"
 msgstr ""
 
-#: fietsboek/models/track.py:585
+#: fietsboek/models/track.py:610
 msgid "tooltip.table.max_speed"
 msgstr ""
 
-#: fietsboek/models/track.py:589
+#: fietsboek/models/track.py:614
 msgid "tooltip.table.avg_speed"
 msgstr ""
 
 #: fietsboek/templates/admin.jinja2:5
 msgid "page.admin.title"
 msgstr ""
 
@@ -125,117 +129,129 @@
 msgid "page.browse.filter.type.organic"
 msgstr ""
 
 #: fietsboek/templates/browse.jinja2:74
 msgid "page.browse.filter.type.synthetic"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:86
+#: fietsboek/templates/browse.jinja2:82
+msgid "page.browse.filter.favourite.all"
+msgstr ""
+
+#: fietsboek/templates/browse.jinja2:83
+msgid "page.browse.filter.favourite.yes"
+msgstr ""
+
+#: fietsboek/templates/browse.jinja2:84
+msgid "page.browse.filter.favourite.no"
+msgstr ""
+
+#: fietsboek/templates/browse.jinja2:97
 msgid "page.browse.filter.my_tracks.only"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:87
+#: fietsboek/templates/browse.jinja2:98
 msgid "page.browse.filter.friends_tracks_only"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:88
+#: fietsboek/templates/browse.jinja2:99
 msgid "page.browse.filter.me_tagged_only"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:98
+#: fietsboek/templates/browse.jinja2:109
 msgid "page.browse.filters.apply"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:102
+#: fietsboek/templates/browse.jinja2:113
 msgid "page.browse.filters.clear_all"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:105
+#: fietsboek/templates/browse.jinja2:116
 msgid "page.browse.filters.expand_advanced"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:110 fietsboek/templates/browse.jinja2:111
+#: fietsboek/templates/browse.jinja2:121 fietsboek/templates/browse.jinja2:122
 msgid "page.browse.sort.date"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:112 fietsboek/templates/browse.jinja2:113
+#: fietsboek/templates/browse.jinja2:123 fietsboek/templates/browse.jinja2:124
 msgid "page.browse.sort.length"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:114 fietsboek/templates/browse.jinja2:115
+#: fietsboek/templates/browse.jinja2:125 fietsboek/templates/browse.jinja2:126
 msgid "page.browse.sort.duration"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:132
+#: fietsboek/templates/browse.jinja2:148
 msgid "page.browse.organic_tooltip"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:134
+#: fietsboek/templates/browse.jinja2:150
 msgid "page.browse.synthetic_tooltip"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:142 fietsboek/templates/details.jinja2:90
+#: fietsboek/templates/browse.jinja2:158 fietsboek/templates/details.jinja2:103
 #: fietsboek/templates/profile.jinja2:15
 msgid "page.details.date"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:144 fietsboek/templates/details.jinja2:104
+#: fietsboek/templates/browse.jinja2:160 fietsboek/templates/details.jinja2:117
 #: fietsboek/templates/profile.jinja2:17
 msgid "page.details.length"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:149 fietsboek/templates/details.jinja2:95
+#: fietsboek/templates/browse.jinja2:165 fietsboek/templates/details.jinja2:108
 #: fietsboek/templates/profile.jinja2:21
 msgid "page.details.start_time"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:151 fietsboek/templates/details.jinja2:99
+#: fietsboek/templates/browse.jinja2:167 fietsboek/templates/details.jinja2:112
 #: fietsboek/templates/profile.jinja2:23
 msgid "page.details.end_time"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:156 fietsboek/templates/details.jinja2:108
+#: fietsboek/templates/browse.jinja2:172 fietsboek/templates/details.jinja2:121
 #: fietsboek/templates/profile.jinja2:27
 msgid "page.details.uphill"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:158 fietsboek/templates/details.jinja2:112
+#: fietsboek/templates/browse.jinja2:174 fietsboek/templates/details.jinja2:125
 #: fietsboek/templates/profile.jinja2:29
 msgid "page.details.downhill"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:163 fietsboek/templates/details.jinja2:117
+#: fietsboek/templates/browse.jinja2:179 fietsboek/templates/details.jinja2:130
 #: fietsboek/templates/profile.jinja2:33
 msgid "page.details.moving_time"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:165 fietsboek/templates/details.jinja2:121
+#: fietsboek/templates/browse.jinja2:181 fietsboek/templates/details.jinja2:134
 #: fietsboek/templates/profile.jinja2:35
 msgid "page.details.stopped_time"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:169 fietsboek/templates/details.jinja2:125
+#: fietsboek/templates/browse.jinja2:185 fietsboek/templates/details.jinja2:138
 #: fietsboek/templates/profile.jinja2:39
 msgid "page.details.max_speed"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:171 fietsboek/templates/details.jinja2:129
+#: fietsboek/templates/browse.jinja2:187 fietsboek/templates/details.jinja2:142
 #: fietsboek/templates/profile.jinja2:41
 msgid "page.details.avg_speed"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:189
+#: fietsboek/templates/browse.jinja2:205
 msgid "page.browse.download_multiple"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:191
+#: fietsboek/templates/browse.jinja2:207
 msgid "page.browse.no_results"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:193
+#: fietsboek/templates/browse.jinja2:209
 msgid "page.browse.no_tracks"
 msgstr ""
 
 #: fietsboek/templates/create_account.jinja2:5
 msgid "page.create_account.title"
 msgstr ""
 
@@ -271,96 +287,96 @@
 msgid "page.create_account.repeat_password"
 msgstr ""
 
 #: fietsboek/templates/create_account.jinja2:54
 msgid "page.create_account.create"
 msgstr ""
 
-#: fietsboek/templates/details.jinja2:6
+#: fietsboek/templates/details.jinja2:7
 msgid "page.details.title"
 msgstr ""
 
-#: fietsboek/templates/details.jinja2:9
+#: fietsboek/templates/details.jinja2:20
 msgid "page.details.edit"
 msgstr ""
 
-#: fietsboek/templates/details.jinja2:10
+#: fietsboek/templates/details.jinja2:21
 msgid "page.details.share"
 msgstr ""
 
-#: fietsboek/templates/details.jinja2:11
+#: fietsboek/templates/details.jinja2:22
 msgid "page.details.delete"
 msgstr ""
 
-#: fietsboek/templates/details.jinja2:17
+#: fietsboek/templates/details.jinja2:28
 msgid "page.details.sharelink.title"
 msgstr ""
 
-#: fietsboek/templates/details.jinja2:21
+#: fietsboek/templates/details.jinja2:32
 msgid "page.details.sharelink.info"
 msgstr ""
 
-#: fietsboek/templates/details.jinja2:28
+#: fietsboek/templates/details.jinja2:39
 msgid "page.details.sharelink.invalidate"
 msgstr ""
 
-#: fietsboek/templates/details.jinja2:30
+#: fietsboek/templates/details.jinja2:41
 msgid "page.details.sharelink.close"
 msgstr ""
 
-#: fietsboek/templates/details.jinja2:40
+#: fietsboek/templates/details.jinja2:51
 msgid "page.details.delete.title"
 msgstr ""
 
-#: fietsboek/templates/details.jinja2:44
+#: fietsboek/templates/details.jinja2:55
 msgid "page.details.delete.info"
 msgstr ""
 
-#: fietsboek/templates/details.jinja2:49
+#: fietsboek/templates/details.jinja2:60
 msgid "page.details.delete.delete"
 msgstr ""
 
-#: fietsboek/templates/details.jinja2:51
+#: fietsboek/templates/details.jinja2:62
 msgid "page.details.delete.close"
 msgstr ""
 
-#: fietsboek/templates/details.jinja2:70
+#: fietsboek/templates/details.jinja2:81
 msgid "page.details.tags"
 msgstr ""
 
-#: fietsboek/templates/details.jinja2:80 fietsboek/templates/edit.jinja2:10
+#: fietsboek/templates/details.jinja2:91 fietsboek/templates/edit.jinja2:10
 #: fietsboek/templates/finish_upload.jinja2:10
 msgid "page.noscript"
 msgstr ""
 
-#: fietsboek/templates/details.jinja2:85
+#: fietsboek/templates/details.jinja2:97
 msgid "page.details.download"
 msgstr ""
 
-#: fietsboek/templates/details.jinja2:174
+#: fietsboek/templates/details.jinja2:187
 msgid "page.details.comments"
 msgstr ""
 
-#: fietsboek/templates/details.jinja2:178
+#: fietsboek/templates/details.jinja2:191
 msgid "page.details.comments.author"
 msgstr ""
 
-#: fietsboek/templates/details.jinja2:195
+#: fietsboek/templates/details.jinja2:208
 msgid "page.details.comments.new.title"
 msgstr ""
 
-#: fietsboek/templates/details.jinja2:198
+#: fietsboek/templates/details.jinja2:211
 msgid "page.details.comments.new.input_title"
 msgstr ""
 
-#: fietsboek/templates/details.jinja2:199
+#: fietsboek/templates/details.jinja2:212
 msgid "page.details.comments.new.input_comment"
 msgstr ""
 
-#: fietsboek/templates/details.jinja2:202
+#: fietsboek/templates/details.jinja2:215
 msgid "page.details.comments.new.submit"
 msgstr ""
 
 #: fietsboek/templates/edit.jinja2:8
 msgid "page.edit.title"
 msgstr ""
 
@@ -432,40 +448,44 @@
 msgid "page.track.form.tagged_people"
 msgstr ""
 
 #: fietsboek/templates/edit_form.jinja2:70
 msgid "page.track.form.add_friend"
 msgstr ""
 
-#: fietsboek/templates/edit_form.jinja2:90
+#: fietsboek/templates/edit_form.jinja2:92
 msgid "page.track.form.badges"
 msgstr ""
 
-#: fietsboek/templates/edit_form.jinja2:101
+#: fietsboek/templates/edit_form.jinja2:103
 msgid "page.track.form.description"
 msgstr ""
 
-#: fietsboek/templates/edit_form.jinja2:108
-#: fietsboek/templates/edit_form.jinja2:122
+#: fietsboek/templates/edit_form.jinja2:110
+#: fietsboek/templates/edit_form.jinja2:131
 msgid "page.track.form.remove_image"
 msgstr ""
 
-#: fietsboek/templates/edit_form.jinja2:117
+#: fietsboek/templates/edit_form.jinja2:120
 msgid "page.track.form.select_images"
 msgstr ""
 
-#: fietsboek/templates/edit_form.jinja2:133
+#: fietsboek/templates/edit_form.jinja2:124
+msgid "page.track.form.image_uploads_disabled"
+msgstr ""
+
+#: fietsboek/templates/edit_form.jinja2:142
 msgid "page.track.form.image_description_modal"
 msgstr ""
 
-#: fietsboek/templates/edit_form.jinja2:140
+#: fietsboek/templates/edit_form.jinja2:149
 msgid "page.track.form.image_description_modal.save"
 msgstr ""
 
-#: fietsboek/templates/edit_form.jinja2:166
+#: fietsboek/templates/edit_form.jinja2:175
 msgid "page.track.form.transformer.enable"
 msgstr ""
 
 #: fietsboek/templates/finish_upload.jinja2:8
 #: fietsboek/templates/upload.jinja2:6
 msgid "page.upload.title"
 msgstr ""
@@ -484,21 +504,21 @@
 msgstr ""
 
 #: fietsboek/templates/home.jinja2:17
 msgid "page.home.unfinished_uploads"
 msgstr ""
 
 #: fietsboek/templates/home.jinja2:31 fietsboek/templates/home.jinja2:38
-#: fietsboek/templates/home.jinja2:56
+#: fietsboek/templates/home.jinja2:66
 msgid "page.home.summary.track"
 msgid_plural "page.home.summary.tracks"
 msgstr[0] ""
 msgstr[1] ""
 
-#: fietsboek/templates/home.jinja2:56
+#: fietsboek/templates/home.jinja2:66
 msgid "page.home.total"
 msgstr ""
 
 #: fietsboek/templates/layout.jinja2:43
 msgid "page.navbar.toggle"
 msgstr ""
 
@@ -594,67 +614,87 @@
 msgid "page.password_reset.password_mismatch"
 msgstr ""
 
 #: fietsboek/templates/password_reset.jinja2:30
 msgid "page.password_reset.reset"
 msgstr ""
 
-#: fietsboek/templates/profile.jinja2:66
+#: fietsboek/templates/profile.jinja2:64
+msgid "page.profile.tabbar.overview"
+msgstr ""
+
+#: fietsboek/templates/profile.jinja2:69
+msgid "page.profile.tabbar.graphs"
+msgstr ""
+
+#: fietsboek/templates/profile.jinja2:83
 msgid "page.profile.length"
 msgstr ""
 
-#: fietsboek/templates/profile.jinja2:70
+#: fietsboek/templates/profile.jinja2:87
+msgid "page.profile.avg_length"
+msgstr ""
+
+#: fietsboek/templates/profile.jinja2:91
 msgid "page.profile.uphill"
 msgstr ""
 
-#: fietsboek/templates/profile.jinja2:74
+#: fietsboek/templates/profile.jinja2:95
 msgid "page.profile.downhill"
 msgstr ""
 
-#: fietsboek/templates/profile.jinja2:78
+#: fietsboek/templates/profile.jinja2:99
 msgid "page.profile.moving_time"
 msgstr ""
 
-#: fietsboek/templates/profile.jinja2:82
+#: fietsboek/templates/profile.jinja2:103
 msgid "page.profile.stopped_time"
 msgstr ""
 
-#: fietsboek/templates/profile.jinja2:86
+#: fietsboek/templates/profile.jinja2:107
+msgid "page.profile.avg_duration"
+msgstr ""
+
+#: fietsboek/templates/profile.jinja2:111
 msgid "page.profile.max_speed"
 msgstr ""
 
-#: fietsboek/templates/profile.jinja2:90
+#: fietsboek/templates/profile.jinja2:115
 msgid "page.profile.avg_speed"
 msgstr ""
 
-#: fietsboek/templates/profile.jinja2:94
+#: fietsboek/templates/profile.jinja2:119
 msgid "page.profile.number_of_tracks"
 msgstr ""
 
-#: fietsboek/templates/profile.jinja2:100
+#: fietsboek/templates/profile.jinja2:125
 msgid "page.profile.longest_distance_track"
 msgstr ""
 
-#: fietsboek/templates/profile.jinja2:105
+#: fietsboek/templates/profile.jinja2:130
 msgid "page.profile.shortest_distance_track"
 msgstr ""
 
-#: fietsboek/templates/profile.jinja2:110
+#: fietsboek/templates/profile.jinja2:135
 msgid "page.profile.longest_duration_track"
 msgstr ""
 
-#: fietsboek/templates/profile.jinja2:115
+#: fietsboek/templates/profile.jinja2:140
 msgid "page.profile.shortest_duration_track"
 msgstr ""
 
-#: fietsboek/templates/profile.jinja2:135
+#: fietsboek/templates/profile.jinja2:147
+msgid "page.profile.graph.km_per_month"
+msgstr ""
+
+#: fietsboek/templates/profile.jinja2:171
 msgid "page.profile.heatmap"
 msgstr ""
 
-#: fietsboek/templates/profile.jinja2:140
+#: fietsboek/templates/profile.jinja2:176
 msgid "page.profile.tilehunt"
 msgstr ""
 
 #: fietsboek/templates/request_password.jinja2:5
 msgid "page.request_password.title"
 msgstr ""
 
@@ -719,166 +759,182 @@
 msgstr ""
 
 #: fietsboek/templates/user_data.jinja2:33
 msgid "page.my_profile.personal_data.save"
 msgstr ""
 
 #: fietsboek/templates/user_data.jinja2:38
+msgid "page.my_profile.session_logout.title"
+msgstr ""
+
+#: fietsboek/templates/user_data.jinja2:40
+msgid "page.my_profile.session_logout.explanation"
+msgstr ""
+
+#: fietsboek/templates/user_data.jinja2:44
+msgid "page.my_profile.session_logout.button"
+msgstr ""
+
+#: fietsboek/templates/user_data.jinja2:49
 msgid "page.my_profile.friends"
 msgstr ""
 
-#: fietsboek/templates/user_data.jinja2:46
+#: fietsboek/templates/user_data.jinja2:57
 msgid "page.my_profile.unfriend"
 msgstr ""
 
-#: fietsboek/templates/user_data.jinja2:56
+#: fietsboek/templates/user_data.jinja2:67
 msgid "page.my_profile.accept_friend"
 msgstr ""
 
-#: fietsboek/templates/user_data.jinja2:73
+#: fietsboek/templates/user_data.jinja2:84
 msgid "page.my_profile.friend_request_email"
 msgstr ""
 
-#: fietsboek/templates/user_data.jinja2:77
+#: fietsboek/templates/user_data.jinja2:88
 msgid "page.my_profile.send_friend_request"
 msgstr ""
 
-#: fietsboek/transformers/breaks.py:31
+#: fietsboek/transformers/breaks.py:32
 msgid "transformers.remove-breaks.title"
 msgstr ""
 
-#: fietsboek/transformers/breaks.py:35
+#: fietsboek/transformers/breaks.py:36
 msgid "transformers.remove-breaks.description"
 msgstr ""
 
-#: fietsboek/transformers/elevation.py:42
+#: fietsboek/transformers/elevation.py:43
 msgid "transformers.fix-null-elevation.title"
 msgstr ""
 
-#: fietsboek/transformers/elevation.py:46
+#: fietsboek/transformers/elevation.py:47
 msgid "transformers.fix-null-elevation.description"
 msgstr ""
 
-#: fietsboek/transformers/elevation.py:115
+#: fietsboek/transformers/elevation.py:116
 msgid "transformers.fix-elevation-jumps"
 msgstr ""
 
-#: fietsboek/transformers/elevation.py:119
+#: fietsboek/transformers/elevation.py:120
 msgid "transformers.fix-elevation-jumps.description"
 msgstr ""
 
-#: fietsboek/views/account.py:53
+#: fietsboek/views/account.py:54
 msgid "flash.invalid_name"
 msgstr ""
 
-#: fietsboek/views/account.py:58
+#: fietsboek/views/account.py:59
 msgid "flash.invalid_email"
 msgstr ""
 
-#: fietsboek/views/account.py:67
+#: fietsboek/views/account.py:69
 msgid "flash.a_confirmation_link_has_been_sent"
 msgstr ""
 
-#: fietsboek/views/admin.py:48
+#: fietsboek/views/admin.py:49
 msgid "flash.badge_added"
 msgstr ""
 
-#: fietsboek/views/admin.py:72
+#: fietsboek/views/admin.py:73
 msgid "flash.badge_modified"
 msgstr ""
 
-#: fietsboek/views/admin.py:92
+#: fietsboek/views/admin.py:93
 msgid "flash.badge_deleted"
 msgstr ""
 
-#: fietsboek/views/default.py:115
+#: fietsboek/views/default.py:116
 msgid "flash.invalid_credentials"
 msgstr ""
 
-#: fietsboek/views/default.py:119
+#: fietsboek/views/default.py:120
 msgid "flash.account_not_verified"
 msgstr ""
 
-#: fietsboek/views/default.py:122
+#: fietsboek/views/default.py:123
 msgid "flash.logged_in"
 msgstr ""
 
-#: fietsboek/views/default.py:142
+#: fietsboek/views/default.py:144
 msgid "flash.logged_out"
 msgstr ""
 
-#: fietsboek/views/default.py:172
+#: fietsboek/views/default.py:174
 msgid "flash.reset_invalid_email"
 msgstr ""
 
-#: fietsboek/views/default.py:177
+#: fietsboek/views/default.py:179
 msgid "flash.password_token_generated"
 msgstr ""
 
-#: fietsboek/views/default.py:182
+#: fietsboek/views/default.py:184
 msgid "page.password_reset.email.subject"
 msgstr ""
 
-#: fietsboek/views/default.py:185
+#: fietsboek/views/default.py:187
 msgid "page.password_reset.email.body"
 msgstr ""
 
-#: fietsboek/views/default.py:224
+#: fietsboek/views/default.py:226
 msgid "flash.resend_verification_email_fail"
 msgstr ""
 
-#: fietsboek/views/default.py:229
+#: fietsboek/views/default.py:231
 msgid "flash.verification_token_generated"
 msgstr ""
 
-#: fietsboek/views/default.py:249
+#: fietsboek/views/default.py:251
 msgid "flash.token_expired"
 msgstr ""
 
-#: fietsboek/views/default.py:255
+#: fietsboek/views/default.py:257
 msgid "flash.email_verified"
 msgstr ""
 
-#: fietsboek/views/default.py:269
+#: fietsboek/views/default.py:271
 msgid "flash.password_updated"
 msgstr ""
 
-#: fietsboek/views/detail.py:155
+#: fietsboek/views/detail.py:162
 msgid "flash.track_deleted"
 msgstr ""
 
-#: fietsboek/views/upload.py:52
+#: fietsboek/views/upload.py:53
 msgid "flash.no_file_selected"
 msgstr ""
 
-#: fietsboek/views/upload.py:62
+#: fietsboek/views/upload.py:66
 msgid "flash.invalid_file"
 msgstr ""
 
-#: fietsboek/views/upload.py:188
+#: fietsboek/views/upload.py:192
 msgid "flash.upload_success"
 msgstr ""
 
-#: fietsboek/views/upload.py:207
+#: fietsboek/views/upload.py:211
 msgid "flash.upload_cancelled"
 msgstr ""
 
-#: fietsboek/views/user_data.py:60
+#: fietsboek/views/user_data.py:67
 msgid "flash.personal_data_updated"
 msgstr ""
 
-#: fietsboek/views/user_data.py:78
+#: fietsboek/views/user_data.py:86
 msgid "flash.friend_not_found"
 msgstr ""
 
-#: fietsboek/views/user_data.py:84
+#: fietsboek/views/user_data.py:92
 msgid "flash.friend_already_exists"
 msgstr ""
 
-#: fietsboek/views/user_data.py:92
+#: fietsboek/views/user_data.py:100
 msgid "flash.friend_added"
 msgstr ""
 
-#: fietsboek/views/user_data.py:102
+#: fietsboek/views/user_data.py:110
 msgid "flash.friend_request_sent"
 msgstr ""
 
+#: fietsboek/views/user_data.py:196
+msgid "flash.sessions_logged_out"
+msgstr ""
+
```

### Comparing `fietsboek-0.8.0/fietsboek/models/__init__.py` & `fietsboek-0.9.0/fietsboek/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Main module for the fietsboek models.
 
 Note that all SQLAlchemy models are re-imported here. You should only need to
 access the submodules if you need some of the auxiliary definitions.
 """
+
 import zope.sqlalchemy
 from sqlalchemy import engine_from_config
 from sqlalchemy.orm import configure_mappers, sessionmaker
 
 from .badge import Badge  # flake8: noqa
 from .comment import Comment  # flake8: noqa
 from .image import ImageMetadata  # flake8: noqa
```

### Comparing `fietsboek-0.8.0/fietsboek/models/badge.py` & `fietsboek-0.9.0/fietsboek/models/badge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The Badge model."""
+
 from typing import TYPE_CHECKING
 
 from pyramid.httpexceptions import HTTPNotFound
 from sqlalchemy import Column, Integer, LargeBinary, Text, select
 from sqlalchemy.orm import Mapped, relationship
 
 from .meta import Base
```

### Comparing `fietsboek-0.8.0/fietsboek/models/comment.py` & `fietsboek-0.9.0/fietsboek/models/comment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Comment model."""
+
 from typing import TYPE_CHECKING
 
 from sqlalchemy import Column, DateTime, ForeignKey, Integer, Text
 from sqlalchemy.orm import Mapped, relationship
 
 from .meta import Base
```

### Comparing `fietsboek-0.8.0/fietsboek/models/image.py` & `fietsboek-0.9.0/fietsboek/models/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Image metadata.
 
 The actual image data is saved on disk, we only store the metadata such as an
 image description here.
 """
+
 from typing import TYPE_CHECKING
 
 from sqlalchemy import Column, ForeignKey, Integer, Text, UniqueConstraint, select
 from sqlalchemy.orm import Mapped, relationship
 
 from .meta import Base
```

### Comparing `fietsboek-0.8.0/fietsboek/models/meta.py` & `fietsboek-0.9.0/fietsboek/models/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base metadata definition for the SQLAlchemy models."""
+
 from sqlalchemy.orm import declarative_base
 from sqlalchemy.schema import MetaData
 
 # Recommended naming convention used by Alembic, as various different database
 # providers will autogenerate vastly different names making migrations more
 # difficult. See: https://alembic.sqlalchemy.org/en/latest/naming.html
 NAMING_CONVENTION = {
```

### Comparing `fietsboek-0.8.0/fietsboek/models/track.py` & `fietsboek-0.9.0/fietsboek/models/track.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 Once the user has finished the upload, the track is saved as a :class:`Track`.
 Each track can have an associated cache that caches the computed values. This
 keeps the user's metadata and the computed information separate, and allows for
 example all cached data to be re-computed without interfering with the other
 meta information.
 """
+
 import datetime
 import enum
 import gzip
 import logging
 from itertools import chain
 from typing import TYPE_CHECKING, List, Optional, Set, Union
 
@@ -119,14 +120,22 @@
 track_badge_assoc = Table(
     "track_badge_assoc",
     Base.metadata,
     Column("track_id", ForeignKey("tracks.id"), primary_key=True),
     Column("badge_id", ForeignKey("badges.id"), primary_key=True),
 )
 
+
+track_favourite_assoc = Table(
+    "track_favourite_assoc",
+    Base.metadata,
+    Column("track_id", ForeignKey("tracks.id"), primary_key=True),
+    Column("user_id", ForeignKey("users.id"), primary_key=True),
+)
+
 # Some words about timezone handling in saved tracks:
 # https://www.youtube.com/watch?v=-5wpm-gesOY
 #
 # We usually want to store the times and dates in UTC, and then convert them
 # later to the user's display timezone. However, this is not quite right for
 # tracks, as the time of tracks is what JSR-310 would call a "LocalDateTime" -
 # that is, a date and time in the calendar without timezone information. This
@@ -186,14 +195,16 @@
     :vartype tagged_people: list[fietsboek.models.user.User]
     :ivar badges: Badges associated with this track.
     :vartype badges: list[fietsboek.models.badge.Badge]
     :ivar comments: Comments left on this track.
     :vartype comments: list[fietsboek.models.comment.Comment]
     :ivar images: Metadata of the images saved for this track.
     :vartype images: list[fietsboek.models.image.ImageMetadata]
+    :ivar favourees: List of users that have this track as a favourite.
+    :vartype favourees: list[fietsboek.models.user.User]
     """
 
     __tablename__ = "tracks"
     id = Column(Integer, primary_key=True)
     owner_id = Column(Integer, ForeignKey("users.id"))
     title = Column(Text)
     description = Column(Text)
@@ -219,14 +230,17 @@
     )
     comments: Mapped[list["models.Comment"]] = relationship(
         "Comment", back_populates="track", cascade="all, delete-orphan"
     )
     images: Mapped[list["models.ImageMetadata"]] = relationship(
         "ImageMetadata", back_populates="track", cascade="all, delete-orphan"
     )
+    favourees: Mapped[list["models.User"]] = relationship(
+        "User", secondary=track_favourite_assoc, back_populates="favourite_tracks"
+    )
 
     @classmethod
     def factory(cls, request):
         """Factory method to pass to a route definition.
 
         This factory retrieves the track based on the ``track_id`` matched
         route parameter, and returns the track. If the track is not found,
@@ -583,14 +597,15 @@
         """
 
         def number(num):
             return format_decimal(num, locale=localizer.locale_name)
 
         rows = [
             (_("tooltip.table.length"), f"{number(round(self.length / 1000, 2))} km"),
+            (_("tooltip.table.people"), str(len(self.track.tagged_people) + 1)),
             (_("tooltip.table.uphill"), f"{number(round(self.uphill, 2))} m"),
             (_("tooltip.table.downhill"), f"{number(round(self.downhill, 2))} m"),
             (_("tooltip.table.moving_time"), f"{self.moving_time}"),
             (_("tooltip.table.stopped_time"), f"{self.stopped_time}"),
             (
                 _("tooltip.table.max_speed"),
                 f"{number(round(util.mps_to_kph(self.max_speed), 2))} km/h",
@@ -602,14 +617,24 @@
         ]
         rows = [
             f"<tr><td>{localizer.translate(name)}</td><td>{value}</td></tr>"
             for (name, value) in rows
         ]
         return Markup(f'<table>{"".join(rows)}</table>')
 
+    def html_tooltip_tagged_people(self) -> Markup:
+        """Returns the tagged people as HTML, ready to be shown as a tooltip.
+
+        :return: The generated HTML.
+        """
+        people = [self.owner] + list(self.tagged_people)
+        people.sort(key=lambda p: p.name or "")
+        html_list = "".join(Markup("<li>{}</li>").format(person.name) for person in people)
+        return Markup("<ul class=&quot;mb-0&quot;>{}</ul>").format(html_list)
+
     # Proxied properties
     @property
     def id(self) -> Optional[int]:
         """ID of the underlying track."""
         return self.track.id
 
     @property
@@ -668,14 +693,19 @@
         return self.track.comments[:]
 
     @property
     def images(self) -> List["models.ImageMetadata"]:
         """Images of the underlying track."""
         return self.track.images[:]
 
+    @property
+    def favourees(self) -> List["models.User"]:
+        """People who have favoured this track."""
+        return self.track.favourees[:]
+
     def text_tags(self) -> Set[str]:
         """Returns a set of textual tags.
 
         :return: The tags of the track, as a set of strings.
         """
         return self.track.text_tags()
```

### Comparing `fietsboek-0.8.0/fietsboek/models/user.py` & `fietsboek-0.9.0/fietsboek/models/user.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """User models for fietsboek."""
+
 import datetime
 import enum
+import hashlib
 import secrets
 import uuid
 from functools import reduce
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
 from cryptography.exceptions import InvalidKey
 from cryptography.hazmat.primitives.kdf.scrypt import Scrypt
 from pyramid.authorization import ALL_PERMISSIONS, Allow
 from pyramid.httpexceptions import HTTPNotFound
 from pyramid.request import Request
 from sqlalchemy import (
@@ -24,15 +26,16 @@
     Text,
     UniqueConstraint,
     delete,
     func,
     select,
     union,
 )
-from sqlalchemy.orm import Mapped, relationship, with_parent
+from sqlalchemy.exc import NoResultFound
+from sqlalchemy.orm import Mapped, Session, relationship, with_parent
 from sqlalchemy.orm.attributes import flag_dirty
 from sqlalchemy.orm.session import object_session
 
 from .meta import Base
 
 if TYPE_CHECKING:
     from .comment import Comment
@@ -53,18 +56,23 @@
 SCRYPT_PARAMETERS = {
     "length": 32,
     "n": 2**14,
     "r": 8,
     "p": 1,
 }
 SALT_LENGTH = 32
+SESSION_SECRET_LENGTH = 32
+"""Length of the secret bytes for the user's session."""
 
 TOKEN_LIFETIME = datetime.timedelta(hours=24)
 """Maximum validity time of a token."""
 
+FINGERPRINT_SHAKE_BYTES = 10
+"""Number of bytes to include in the SHAKE digest of the fingerprint."""
+
 
 friends_assoc = Table(
     "friends_assoc",
     Base.metadata,
     Column("user_1_id", ForeignKey("users.id"), primary_key=True),
     Column("user_2_id", ForeignKey("users.id"), primary_key=True),
 )
@@ -81,45 +89,51 @@
         :meth:`set_password` and :meth:`check_password` to interface with the
         password instead of accessing this field directly.
     :vartype password: bytes
     :ivar salt: Password salt.
     :vartype salt: bytes
     :ivar email: Email address of the user.
     :vartype email: str
+    :ivar session_secret: Secret bytes for the session fingerprint.
+    :vartype session_secret: bytes
     :ivar is_admin: Flag determining whether this user has admin access.
     :vartype is_admin: bool
     :ivar is_verified: Flag determining whether this user has been verified.
     :vartype is_verified: bool
     :ivar tracks: Tracks owned by this user.
     :vartype tracks: list[fietsboek.models.track.Track]
     :ivar tagged_tracks: Tracks in which this user is tagged.
-    :vartype tracks: list[fietsboek.models.track.Track]
+    :vartype tagged_tracks: list[fietsboek.models.track.Track]
     :ivar uploads: Currently ongoing uploads by this user.
     :vartype uploads: list[fietsboek.models.track.Upload]
     :ivar tokens: List of tokens that this user can use.
     :vartype tokens: list[fietsboek.models.user.Token]
     :ivar comments: List of comments left by this user.
     :vartype comments: list[fietsboek.model.comment.Comment]
     """
 
     __tablename__ = "users"
     id = Column(Integer, primary_key=True)
     name = Column(Text)
     password = Column(LargeBinary)
     salt = Column(LargeBinary)
     email = Column(Text)
+    session_secret = Column(LargeBinary(SESSION_SECRET_LENGTH))
     is_admin = Column(Boolean, default=False)
     is_verified = Column(Boolean, default=False)
 
     tracks: Mapped[list["Track"]] = relationship(
         "Track", back_populates="owner", cascade="all, delete-orphan"
     )
     tagged_tracks: Mapped[list["Track"]] = relationship(
         "Track", secondary="track_people_assoc", back_populates="tagged_people"
     )
+    favourite_tracks: Mapped[list["Track"]] = relationship(
+        "Track", secondary="track_favourite_assoc", back_populates="favourees"
+    )
     uploads: Mapped[list["Upload"]] = relationship(
         "Upload", back_populates="owner", cascade="all, delete-orphan"
     )
     tokens: Mapped[list["Token"]] = relationship(
         "Token", back_populates="user", cascade="all, delete-orphan"
     )
     comments: Mapped[list["Comment"]] = relationship(
@@ -175,14 +189,67 @@
     def __acl__(self):
         acl = [
             (Allow, "group:admins", ALL_PERMISSIONS),
             (Allow, f"user:{self.id}", ALL_PERMISSIONS),
         ]
         return acl
 
+    def _fingerprint(self) -> str:
+        # We're not interested in hiding the data by all means, we just want a
+        # good check to see whether the email of the represented user actually
+        # matches with the database entry. Therefore, we use a short SHAKE hash.
+        email = self.email or ""
+        shaker = hashlib.shake_128()
+        shaker.update(email.encode("utf-8"))
+        shaker.update(self.password or b"")
+        shaker.update(self.session_secret or b"")
+        return shaker.hexdigest(FINGERPRINT_SHAKE_BYTES)
+
+    def authenticated_user_id(self) -> str:
+        """Returns a string suitable to re-identify this user, e.g. in a cookie
+        or session.
+
+        The returned ID contains a "fingerprint" to ensure that the
+        re-identified user matches.
+
+        :return: The string used to re-identify this user.
+        """
+        fingerprint = self._fingerprint()
+        return f"{self.id}-{fingerprint}"
+
+    @classmethod
+    def get_by_authenticated_user_id(cls, session: Session, user_id: str) -> Optional["User"]:
+        """Retrieves a user by their authenticated user ID (as returned by
+        :meth:`authenticated_user_id`).
+
+        This method returns ``None`` on any of the following conditions:
+
+        * The user ID is malformed.
+        * The user with the given ID was not found.
+        * The fingerprint of the ``user_id`` and the database user do not match.
+
+        :param session: The database session which to retrieve the user from.
+        :param user_id: The user ID.
+        :return: The user, if found.
+        """
+        try:
+            numeric_id, fingerprint = user_id.split("-")
+        except ValueError:
+            # Malformed ID
+            return None
+        query = select(cls).filter_by(id=numeric_id)
+        try:
+            user = session.execute(query).scalar_one()
+        except NoResultFound:
+            return None
+        # pylint: disable=protected-access
+        if user._fingerprint() != fingerprint:
+            return None
+        return user
+
     def set_password(self, new_password):
         """Sets a new password for the user.
 
         This function automatically generates a new random salt and updates the
         stored password hash and salt value.
 
         :param new_password: The new password of the user.
@@ -208,14 +275,22 @@
         password = password.encode("utf-8")
         scrypt = Scrypt(salt=self.salt or b"", **SCRYPT_PARAMETERS)
         try:
             scrypt.verify(password, self.password or b"")
         except InvalidKey:
             raise PasswordMismatch from None
 
+    def roll_session_secret(self):
+        """Rolls a new session secret for the user.
+
+        This function automatically generates the right amount of random bytes
+        from a secure source.
+        """
+        self.session_secret = secrets.token_bytes(SESSION_SECRET_LENGTH)
+
     def principals(self):
         """Returns all principals that this user fulfills.
 
         This does not include the ``Everyone`` and ``Authenticated``
         principals, as those have to be checked before accessing the user.
 
         :return: The seceurity principals that this user fulfills.
@@ -365,14 +440,24 @@
         assert session
         if self.id > friend.id:
             friend.add_friend(self)
             return
         stmt = friends_assoc.insert().values(user_1_id=self.id, user_2_id=friend.id)
         session.execute(stmt)
 
+    def toggle_favourite(self, track: "Track"):
+        """Toggles the favourite status for the given track.
+
+        :param track: The track to (un)favour.
+        """
+        if track in self.favourite_tracks:
+            self.favourite_tracks.remove(track)
+        else:
+            self.favourite_tracks.append(track)
+
     def autocomplete_tags(self):
         """Returns all tags the user has ever used, suitable for autocompletion
         lists.
 
         :return: All tags of the user.
         :rtype: ~collections.abc.Iterator[str]
         """
```

### Comparing `fietsboek-0.8.0/fietsboek/pages.py` & `fietsboek-0.9.0/fietsboek/pages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module containing logic to support "static" pages."""
+
 import enum
 import re
 from pathlib import Path
 from typing import List, Optional
 
 import markdown
 from pyramid.request import Request
```

### Comparing `fietsboek-0.8.0/fietsboek/routes.py` & `fietsboek-0.9.0/fietsboek/routes.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,26 +16,26 @@
     config.add_route("password-reset", "/password-reset")
     config.add_route("resend-verification", "/resend-verification")
     config.add_route("use-token", "/token/{uuid}")
     config.add_route("create-account", "/create-account")
 
     config.add_route("upload", "/upload")
     config.add_route(
-        "preview", "/preview/{upload_id}.gpx", factory="fietsboek.models.Upload.factory"
+        "preview", "/upload/{upload_id}/preview.gpx", factory="fietsboek.models.Upload.factory"
     )
     config.add_route(
         "finish-upload", "/upload/{upload_id}", factory="fietsboek.models.Upload.factory"
     )
     config.add_route(
-        "cancel-upload", "/cancel/{upload_id}", factory="fietsboek.models.Upload.factory"
+        "cancel-upload", "/upload/{upload_id}/cancel", factory="fietsboek.models.Upload.factory"
     )
 
     config.add_route("details", "/track/{track_id}", factory="fietsboek.models.Track.factory")
     config.add_route("edit", "/track/{track_id}/edit", factory="fietsboek.models.Track.factory")
-    config.add_route("gpx", "/gpx/{track_id}.gpx", factory="fietsboek.models.Track.factory")
+    config.add_route("gpx", "/track/{track_id}/gpx", factory="fietsboek.models.Track.factory")
     config.add_route(
         "invalidate-share",
         "/track/{track_id}/invalidate-link",
         factory="fietsboek.models.Track.factory",
     )
     config.add_route(
         "delete-track", "/track/{track_id}/delete", factory="fietsboek.models.Track.factory"
@@ -55,14 +55,17 @@
     config.add_route("admin-badge-delete", "/admin/delete-badge")
 
     config.add_route("user-data", "/me")
     config.add_route("add-friend", "/me/send-friend-request")
     config.add_route("delete-friend", "/me/delete-friend")
     config.add_route("accept-friend", "/me/accept-friend")
     config.add_route("json-friends", "/me/friends.json")
+    config.add_route("json-summary", "/me/summary.json")
+    config.add_route("toggle-favourite", "/me/toggle-favourite")
+    config.add_route("force-logout", "/me/force-logout")
 
     config.add_route("profile", "/user/{user_id}", factory="fietsboek.models.User.factory")
     config.add_route(
         "user-tile",
         "/user/{user_id}/tile/{map}/{z:\\d+}/{x:\\d+}/{y:\\d+}",
         factory="fietsboek.models.User.factory",
     )
```

### Comparing `fietsboek-0.8.0/fietsboek/scripts/__init__.py` & `fietsboek-0.9.0/fietsboek/scripts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Various command line scripts to interact with the fietsboek installation."""
+
 from typing import Any, Optional
 
 import click
 from click.core import ParameterSource
 
 
 class ConfigOption(click.Path):
```

### Comparing `fietsboek-0.8.0/fietsboek/scripts/fietscron.py` & `fietsboek-0.9.0/fietsboek/scripts/fietscron.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Script to do maintenance actions for fietsboek."""
+
 import datetime
 import logging
 import logging.config
 from pathlib import Path
 
 import click
 import pyramid.paster
```

### Comparing `fietsboek-0.8.0/fietsboek/scripts/fietsctl.py` & `fietsboek-0.9.0/fietsboek/scripts/fietsctl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Script to do maintenance work on a Fietsboek instance."""
+
 # pylint: disable=too-many-arguments
 import logging
 from typing import Optional
 
 import click
 from click_option_group import RequiredMutuallyExclusiveOptionGroup, optgroup
 from pyramid.paster import bootstrap, setup_logging
 from pyramid.scripting import AppEnvironment
 from sqlalchemy import select
+from sqlalchemy.exc import NoResultFound
 
 from .. import __VERSION__, hittekaart, models, util
 from ..data import DataManager
 from . import config_option
 
 LOGGER = logging.getLogger("fietsctl")
 
@@ -106,14 +108,15 @@
         result = env["request"].dbsession.execute(query).scalar_one_or_none()
         if result is not None:
             click.echo("Error: The given email already exists!", err=True)
             ctx.exit(EXIT_FAILURE)
 
     user = models.User(name=name, email=email, is_verified=True, is_admin=admin)
     user.set_password(password)
+    user.roll_session_secret()
 
     with env["request"].tm:
         dbsession = env["request"].dbsession
         dbsession.add(user)
         dbsession.flush()
         user_id = user.id
 
@@ -225,25 +228,27 @@
         click.echo(f"Changed password of {user_name} ({user_email})")
 
 
 @cmd_user.command("modify")
 @config_option
 @click.option("--admin/--no-admin", help="Make the user an admin.", default=None)
 @click.option("--verified/--no-verified", help="Set the user verification status.", default=None)
+@click.option("--set-email", help="Set the user's email address")
 @optgroup.group("User selection", cls=RequiredMutuallyExclusiveOptionGroup)
 @optgroup.option("--id", "-i", "id_", help="Database ID of the user.", type=int)
 @optgroup.option("--email", "-e", help="Email address of the user.")
 @click.pass_context
 def cms_user_modify(
     ctx: click.Context,
     config: str,
     admin: Optional[bool],
     verified: Optional[bool],
     id_: Optional[int],
     email: Optional[str],
+    set_email: Optional[str],
 ):
     """Modify a user."""
     env = setup(config)
     if id_ is not None:
         query = select(models.User).filter_by(id=id_)
     else:
         query = models.User.query_by_email(email)
@@ -254,14 +259,24 @@
             click.echo("Error: No such user found.", err=True)
             ctx.exit(EXIT_FAILURE)
 
         if admin is not None:
             user.is_admin = admin
         if verified is not None:
             user.is_verified = verified
+        if set_email is not None:
+            # Try to ensure that the email is unique. We do have the constraint
+            # for that, but capitalization might screw us here.
+            try:
+                dbsession.execute(models.User.query_by_email(set_email)).scalar_one()
+            except NoResultFound:
+                user.email = set_email
+            else:
+                click.echo("Error: E-Mail already exists", err=True)
+                ctx.exit(EXIT_FAILURE)
 
         user_name = click.style(user.name, fg=FG_USER_NAME)
         user_email = click.style(user.email, fg=FG_USER_EMAIL)
         click.echo(f"{user_name} - {user_email}")
         click.echo(f"Is admin: {human_bool(user.is_admin)}")
         click.echo(f"Is verified: {human_bool(user.is_verified)}")
```

### Comparing `fietsboek-0.8.0/fietsboek/security.py` & `fietsboek-0.9.0/fietsboek/security.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module implementing the user authentication."""
+
 from pyramid.authentication import AuthTktCookieHelper, SessionAuthenticationHelper
 from pyramid.authorization import ACLHelper, Authenticated, Everyone
 from pyramid.interfaces import ISecurityPolicy
 from pyramid.security import Allowed, Denied
 from pyramid.traversal import DefaultRootFactory
-from sqlalchemy import select
 from zope.interface import implementer
 
 from . import models
 
 ADMIN_PERMISSIONS = {"admin"}
 
 
@@ -32,23 +32,22 @@
             auth_info = self.cookie_helper.identify(request) or {}
             userid = auth_info.get("userid")
 
         # Still no identity found
         if userid is None:
             return None
 
-        query = select(models.User).filter_by(id=int(userid))
-        return request.dbsession.execute(query).scalar_one_or_none()
+        return models.User.get_by_authenticated_user_id(request.dbsession, userid)
 
     def authenticated_userid(self, request):
         """See :meth:`pyramid.interfaces.ISecurityPolicy.authenticated_userid`"""
         identity = self.identity(request)
         if identity is None:
             return None
-        return str(identity.id)
+        return identity.authenticated_user_id()
 
     def permits(self, request, context, permission):
         """See :meth:`pyramid.interfaces.ISecurityPolicy.permits`"""
         identity = self.identity(request)
         # If the context is not there, we are on a static site that does not use ACL
         if isinstance(context, DefaultRootFactory):
             if identity is None:
```

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/GPX2GM.css` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/GPX2GM.css`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/GPX2GM.js` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/GPX2GM.js`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/GPX2GM_Defs.js` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/GPX2GM_Defs.js`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/Loading_icon.gif` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/Loading_icon.gif`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/Loading_icon_V1.gif` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/Loading_icon_V1.gif`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/Loading_icon_V2.gif` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/Loading_icon_V2.gif`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/airport.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/airport.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/bar.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/bar.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/boat.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/boat.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/bridge.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/bridge.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/castle.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/castle.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/church2.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/church2.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/cluster.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/cluster.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/cluster.svg` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/cluster.svg`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/current_location - Kopie.svg` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/current_location - Kopie.svg`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/current_location.svg` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/current_location.svg`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/cycling.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/cycling.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/finish.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/finish.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/harbor.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/harbor.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/hiking.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/hiking.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/hotel2.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/hotel2.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/kreis.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/kreis.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/library.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/library.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/marker-icon_bw.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/marker-icon_bw.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/marker.svg` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/marker.svg`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/museum.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/museum.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/panorama.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/panorama.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/park.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/park.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/peak.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/peak.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/photo.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/photo.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/pin_red.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/pin_red.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/pin_red_shadow.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/pin_red_shadow.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/restaurant.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/restaurant.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/shadow.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/shadow.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/shadow50.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/shadow50.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/shoppingmall.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/shoppingmall.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/streckenmarker - Kopie.svg` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/streckenmarker - Kopie.svg`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/streckenmarker.svg` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/streckenmarker.svg`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/subway.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/subway.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/tent.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/tent.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/train.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/train.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/video.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/video.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/villa.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/villa.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/whereami.svg` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/whereami.svg`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/whereami_V1.svg` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/Icons/whereami_V1.svg`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/gmutils.js` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/gmutils.js`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/gra_canvas.js` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/gra_canvas.js`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/gra_svg.js` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/gra_svg.js`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/images/layers-2x.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/leaflet/images/layers-2x.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/images/layers.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/leaflet/images/layers.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/images/marker-icon-2x.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/leaflet/images/marker-icon-2x.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/images/marker-icon.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/leaflet/images/marker-icon.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/images/marker-shadow.png` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/leaflet/images/marker-shadow.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/leaflet.css` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/leaflet/leaflet.css`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/leaflet.js` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/leaflet/leaflet.js`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/leaflet.js.map` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/leaflet/leaflet.js.map`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/osmutils.js` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/osmutils.js`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/plot.js` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/plot.js`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/GM_Utils/shimg.js` & `fietsboek-0.9.0/fietsboek/static/GM_Utils/shimg.js`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/bootstrap-icons.css` & `fietsboek-0.9.0/fietsboek/static/bootstrap-icons.css`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*!
- * Bootstrap Icons (https://icons.getbootstrap.com/)
+ * Bootstrap Icons v1.10.5 (https://icons.getbootstrap.com/)
  * Copyright 2019-2023 The Bootstrap Authors
- * Licensed under MIT (https://github.com/twbs/icons/blob/main/LICENSE.md)
+ * Licensed under MIT (https://github.com/twbs/icons/blob/main/LICENSE)
  */
 
 @font-face {
   font-display: block;
   font-family: "bootstrap-icons";
   src: url("./fonts/bootstrap-icons.woff2?1fa40e8900654d2863d011707b9fb6f2") format("woff2"),
 url("./fonts/bootstrap-icons.woff?1fa40e8900654d2863d011707b9fb6f2") format("woff");
```

### Comparing `fietsboek-0.8.0/fietsboek/static/bootstrap.bundle.min.js` & `fietsboek-0.9.0/fietsboek/static/bootstrap.bundle.min.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,39 +1,37 @@
 /*!
- * Bootstrap v5.2.3 (https://getbootstrap.com/)
- * Copyright 2011-2022 The Bootstrap Authors (https://github.com/twbs/bootstrap/graphs/contributors)
+ * Bootstrap v5.3.1 (https://getbootstrap.com/)
+ * Copyright 2011-2023 The Bootstrap Authors (https://github.com/twbs/bootstrap/graphs/contributors)
  * Licensed under MIT (https://github.com/twbs/bootstrap/blob/main/LICENSE)
  */
 ! function(t, e) {
     "object" == typeof exports && "undefined" != typeof module ? module.exports = e() : "function" == typeof define && define.amd ? define(e) : (t = "undefined" != typeof globalThis ? globalThis : t || self).bootstrap = e()
 }(this, (function() {
     "use strict";
-    const t = "transitionend",
-        e = t => {
-            let e = t.getAttribute("data-bs-target");
-            if (!e || "#" === e) {
-                let i = t.getAttribute("href");
-                if (!i || !i.includes("#") && !i.startsWith(".")) return null;
-                i.includes("#") && !i.startsWith("#") && (i = `#${i.split("#")[1]}`), e = i && "#" !== i ? i.trim() : null
+    const t = new Map,
+        e = {
+            set(e, i, n) {
+                t.has(e) || t.set(e, new Map);
+                const s = t.get(e);
+                s.has(i) || 0 === s.size ? s.set(i, n) : console.error(`Bootstrap doesn't allow more than one instance per element. Bound instance: ${Array.from(s.keys())[0]}.`)
+            },
+            get: (e, i) => t.has(e) && t.get(e).get(i) || null,
+            remove(e, i) {
+                if (!t.has(e)) return;
+                const n = t.get(e);
+                n.delete(i), 0 === n.size && t.delete(e)
             }
-            return e
         },
-        i = t => {
-            const i = e(t);
-            return i && document.querySelector(i) ? i : null
-        },
-        n = t => {
-            const i = e(t);
-            return i ? document.querySelector(i) : null
-        },
-        s = e => {
-            e.dispatchEvent(new Event(t))
+        i = "transitionend",
+        n = t => (t && window.CSS && window.CSS.escape && (t = t.replace(/#([^\s"#']+)/g, ((t, e) => `#${CSS.escape(e)}`))), t),
+        s = t => {
+            t.dispatchEvent(new Event(i))
         },
         o = t => !(!t || "object" != typeof t) && (void 0 !== t.jquery && (t = t[0]), void 0 !== t.nodeType),
-        r = t => o(t) ? t.jquery ? t[0] : t : "string" == typeof t && t.length > 0 ? document.querySelector(t) : null,
+        r = t => o(t) ? t.jquery ? t[0] : t : "string" == typeof t && t.length > 0 ? document.querySelector(n(t)) : null,
         a = t => {
             if (!o(t) || 0 === t.getClientRects().length) return !1;
             const e = "visible" === getComputedStyle(t).getPropertyValue("visibility"),
                 i = t.closest("details:not([open])");
             if (!i) return e;
             if (i !== t) {
                 const e = t.closest("summary");
@@ -54,50 +52,48 @@
         h = () => {},
         d = t => {
             t.offsetHeight
         },
         u = () => window.jQuery && !document.body.hasAttribute("data-bs-no-jquery") ? window.jQuery : null,
         f = [],
         p = () => "rtl" === document.documentElement.dir,
-        g = t => {
+        m = t => {
             var e;
             e = () => {
                 const e = u();
                 if (e) {
                     const i = t.NAME,
                         n = e.fn[i];
                     e.fn[i] = t.jQueryInterface, e.fn[i].Constructor = t, e.fn[i].noConflict = () => (e.fn[i] = n, t.jQueryInterface)
                 }
             }, "loading" === document.readyState ? (f.length || document.addEventListener("DOMContentLoaded", (() => {
                 for (const t of f) t()
             })), f.push(e)) : e()
         },
-        m = t => {
-            "function" == typeof t && t()
-        },
-        _ = (e, i, n = !0) => {
-            if (!n) return void m(e);
+        g = (t, e = [], i = t) => "function" == typeof t ? t(...e) : i,
+        _ = (t, e, n = !0) => {
+            if (!n) return void g(t);
             const o = (t => {
                 if (!t) return 0;
                 let {
                     transitionDuration: e,
                     transitionDelay: i
                 } = window.getComputedStyle(t);
                 const n = Number.parseFloat(e),
                     s = Number.parseFloat(i);
                 return n || s ? (e = e.split(",")[0], i = i.split(",")[0], 1e3 * (Number.parseFloat(e) + Number.parseFloat(i))) : 0
-            })(i) + 5;
+            })(e) + 5;
             let r = !1;
             const a = ({
                 target: n
             }) => {
-                n === i && (r = !0, i.removeEventListener(t, a), m(e))
+                n === e && (r = !0, e.removeEventListener(i, a), g(t))
             };
-            i.addEventListener(t, a), setTimeout((() => {
-                r || s(i)
+            e.addEventListener(i, a), setTimeout((() => {
+                r || s(e)
             }), o)
         },
         b = (t, e, i, n) => {
             const s = t.length;
             let o = t.indexOf(e);
             return -1 === o ? !i && n ? t[s - 1] : t[0] : (o += i ? 1 : -1, n && (o = (o + s) % s), t[Math.max(0, Math.min(o, s - 1))])
         },
@@ -124,19 +120,19 @@
     function k(t, e, i = null) {
         return Object.values(t).find((t => t.callable === e && t.delegationSelector === i))
     }
 
     function L(t, e, i) {
         const n = "string" == typeof e,
             s = n ? i : e || i;
-        let o = N(t);
+        let o = I(t);
         return C.has(o) || (o = t), [n, s, o]
     }
 
-    function D(t, e, i, n, s) {
+    function S(t, e, i, n, s) {
         if ("string" != typeof e || !t) return;
         let [o, r, a] = L(e, i, n);
         if (e in T) {
             const t = t => function(e) {
                 if (!e.relatedTarget || e.relatedTarget !== e.delegateTarget && !e.delegateTarget.contains(e.relatedTarget)) return t.call(this, e)
             };
             r = t(r)
@@ -149,148 +145,127 @@
             u = o ? function(t, e, i) {
                 return function n(s) {
                     const o = t.querySelectorAll(e);
                     for (let {
                             target: r
                         } = s; r && r !== this; r = r.parentNode)
                         for (const a of o)
-                            if (a === r) return j(s, {
+                            if (a === r) return P(s, {
                                 delegateTarget: r
-                            }), n.oneOff && P.off(t, s.type, e, i), i.apply(r, [s])
+                            }), n.oneOff && N.off(t, s.type, e, i), i.apply(r, [s])
                 }
             }(t, i, r) : function(t, e) {
                 return function i(n) {
-                    return j(n, {
+                    return P(n, {
                         delegateTarget: t
-                    }), i.oneOff && P.off(t, n.type, e), e.apply(t, [n])
+                    }), i.oneOff && N.off(t, n.type, e), e.apply(t, [n])
                 }
             }(t, r);
         u.delegationSelector = o ? i : null, u.callable = r, u.oneOff = s, u.uidEvent = d, c[d] = u, t.addEventListener(a, u, o)
     }
 
-    function S(t, e, i, n, s) {
+    function D(t, e, i, n, s) {
         const o = k(e[i], n, s);
         o && (t.removeEventListener(i, o, Boolean(s)), delete e[i][o.uidEvent])
     }
 
-    function I(t, e, i, n) {
+    function $(t, e, i, n) {
         const s = e[i] || {};
-        for (const o of Object.keys(s))
-            if (o.includes(n)) {
-                const n = s[o];
-                S(t, e, i, n.callable, n.delegationSelector)
-            }
+        for (const [o, r] of Object.entries(s)) o.includes(n) && D(t, e, i, r.callable, r.delegationSelector)
     }
 
-    function N(t) {
+    function I(t) {
         return t = t.replace(y, ""), T[t] || t
     }
-    const P = {
+    const N = {
         on(t, e, i, n) {
-            D(t, e, i, n, !1)
+            S(t, e, i, n, !1)
         },
         one(t, e, i, n) {
-            D(t, e, i, n, !0)
+            S(t, e, i, n, !0)
         },
         off(t, e, i, n) {
             if ("string" != typeof e || !t) return;
             const [s, o, r] = L(e, i, n), a = r !== e, l = x(t), c = l[r] || {}, h = e.startsWith(".");
             if (void 0 === o) {
                 if (h)
-                    for (const i of Object.keys(l)) I(t, l, i, e.slice(1));
-                for (const i of Object.keys(c)) {
-                    const n = i.replace(w, "");
-                    if (!a || e.includes(n)) {
-                        const e = c[i];
-                        S(t, l, r, e.callable, e.delegationSelector)
-                    }
+                    for (const i of Object.keys(l)) $(t, l, i, e.slice(1));
+                for (const [i, n] of Object.entries(c)) {
+                    const s = i.replace(w, "");
+                    a && !e.includes(s) || D(t, l, r, n.callable, n.delegationSelector)
                 }
             } else {
                 if (!Object.keys(c).length) return;
-                S(t, l, r, o, s ? i : null)
+                D(t, l, r, o, s ? i : null)
             }
         },
         trigger(t, e, i) {
             if ("string" != typeof e || !t) return null;
             const n = u();
             let s = null,
                 o = !0,
                 r = !0,
                 a = !1;
-            e !== N(e) && n && (s = n.Event(e, i), n(t).trigger(s), o = !s.isPropagationStopped(), r = !s.isImmediatePropagationStopped(), a = s.isDefaultPrevented());
-            let l = new Event(e, {
+            e !== I(e) && n && (s = n.Event(e, i), n(t).trigger(s), o = !s.isPropagationStopped(), r = !s.isImmediatePropagationStopped(), a = s.isDefaultPrevented());
+            const l = P(new Event(e, {
                 bubbles: o,
                 cancelable: !0
-            });
-            return l = j(l, i), a && l.preventDefault(), r && t.dispatchEvent(l), l.defaultPrevented && s && s.preventDefault(), l
+            }), i);
+            return a && l.preventDefault(), r && t.dispatchEvent(l), l.defaultPrevented && s && s.preventDefault(), l
         }
     };
 
-    function j(t, e) {
-        for (const [i, n] of Object.entries(e || {})) try {
+    function P(t, e = {}) {
+        for (const [i, n] of Object.entries(e)) try {
             t[i] = n
         } catch (e) {
             Object.defineProperty(t, i, {
                 configurable: !0,
                 get: () => n
             })
         }
         return t
     }
-    const M = new Map,
-        H = {
-            set(t, e, i) {
-                M.has(t) || M.set(t, new Map);
-                const n = M.get(t);
-                n.has(e) || 0 === n.size ? n.set(e, i) : console.error(`Bootstrap doesn't allow more than one instance per element. Bound instance: ${Array.from(n.keys())[0]}.`)
-            },
-            get: (t, e) => M.has(t) && M.get(t).get(e) || null,
-            remove(t, e) {
-                if (!M.has(t)) return;
-                const i = M.get(t);
-                i.delete(e), 0 === i.size && M.delete(t)
-            }
-        };
 
-    function $(t) {
+    function M(t) {
         if ("true" === t) return !0;
         if ("false" === t) return !1;
         if (t === Number(t).toString()) return Number(t);
         if ("" === t || "null" === t) return null;
         if ("string" != typeof t) return t;
         try {
             return JSON.parse(decodeURIComponent(t))
         } catch (e) {
             return t
         }
     }
 
-    function W(t) {
+    function j(t) {
         return t.replace(/[A-Z]/g, (t => `-${t.toLowerCase()}`))
     }
-    const B = {
+    const F = {
         setDataAttribute(t, e, i) {
-            t.setAttribute(`data-bs-${W(e)}`, i)
+            t.setAttribute(`data-bs-${j(e)}`, i)
         },
         removeDataAttribute(t, e) {
-            t.removeAttribute(`data-bs-${W(e)}`)
+            t.removeAttribute(`data-bs-${j(e)}`)
         },
         getDataAttributes(t) {
             if (!t) return {};
             const e = {},
                 i = Object.keys(t.dataset).filter((t => t.startsWith("bs") && !t.startsWith("bsConfig")));
             for (const n of i) {
                 let i = n.replace(/^bs/, "");
-                i = i.charAt(0).toLowerCase() + i.slice(1, i.length), e[i] = $(t.dataset[n])
+                i = i.charAt(0).toLowerCase() + i.slice(1, i.length), e[i] = M(t.dataset[n])
             }
             return e
         },
-        getDataAttribute: (t, e) => $(t.getAttribute(`data-bs-${W(e)}`))
+        getDataAttribute: (t, e) => M(t.getAttribute(`data-bs-${j(e)}`))
     };
-    class F {
+    class H {
         static get Default() {
             return {}
         }
         static get DefaultType() {
             return {}
         }
         static get NAME() {
@@ -299,543 +274,589 @@
         _getConfig(t) {
             return t = this._mergeConfigObj(t), t = this._configAfterMerge(t), this._typeCheckConfig(t), t
         }
         _configAfterMerge(t) {
             return t
         }
         _mergeConfigObj(t, e) {
-            const i = o(e) ? B.getDataAttribute(e, "config") : {};
+            const i = o(e) ? F.getDataAttribute(e, "config") : {};
             return {
                 ...this.constructor.Default,
                 ..."object" == typeof i ? i : {},
-                ...o(e) ? B.getDataAttributes(e) : {},
+                ...o(e) ? F.getDataAttributes(e) : {},
                 ..."object" == typeof t ? t : {}
             }
         }
         _typeCheckConfig(t, e = this.constructor.DefaultType) {
-            for (const n of Object.keys(e)) {
-                const s = e[n],
-                    r = t[n],
-                    a = o(r) ? "element" : null == (i = r) ? `${i}` : Object.prototype.toString.call(i).match(/\s([a-z]+)/i)[1].toLowerCase();
-                if (!new RegExp(s).test(a)) throw new TypeError(`${this.constructor.NAME.toUpperCase()}: Option "${n}" provided type "${a}" but expected type "${s}".`)
+            for (const [n, s] of Object.entries(e)) {
+                const e = t[n],
+                    r = o(e) ? "element" : null == (i = e) ? `${i}` : Object.prototype.toString.call(i).match(/\s([a-z]+)/i)[1].toLowerCase();
+                if (!new RegExp(s).test(r)) throw new TypeError(`${this.constructor.NAME.toUpperCase()}: Option "${n}" provided type "${r}" but expected type "${s}".`)
             }
             var i
         }
     }
-    class z extends F {
-        constructor(t, e) {
-            super(), (t = r(t)) && (this._element = t, this._config = this._getConfig(e), H.set(this._element, this.constructor.DATA_KEY, this))
+    class W extends H {
+        constructor(t, i) {
+            super(), (t = r(t)) && (this._element = t, this._config = this._getConfig(i), e.set(this._element, this.constructor.DATA_KEY, this))
         }
         dispose() {
-            H.remove(this._element, this.constructor.DATA_KEY), P.off(this._element, this.constructor.EVENT_KEY);
+            e.remove(this._element, this.constructor.DATA_KEY), N.off(this._element, this.constructor.EVENT_KEY);
             for (const t of Object.getOwnPropertyNames(this)) this[t] = null
         }
         _queueCallback(t, e, i = !0) {
             _(t, e, i)
         }
         _getConfig(t) {
             return t = this._mergeConfigObj(t, this._element), t = this._configAfterMerge(t), this._typeCheckConfig(t), t
         }
         static getInstance(t) {
-            return H.get(r(t), this.DATA_KEY)
+            return e.get(r(t), this.DATA_KEY)
         }
         static getOrCreateInstance(t, e = {}) {
             return this.getInstance(t) || new this(t, "object" == typeof e ? e : null)
         }
         static get VERSION() {
-            return "5.2.3"
+            return "5.3.1"
         }
         static get DATA_KEY() {
             return `bs.${this.NAME}`
         }
         static get EVENT_KEY() {
             return `.${this.DATA_KEY}`
         }
         static eventName(t) {
             return `${t}${this.EVENT_KEY}`
         }
     }
-    const q = (t, e = "hide") => {
-        const i = `click.dismiss${t.EVENT_KEY}`,
-            s = t.NAME;
-        P.on(document, i, `[data-bs-dismiss="${s}"]`, (function(i) {
-            if (["A", "AREA"].includes(this.tagName) && i.preventDefault(), l(this)) return;
-            const o = n(this) || this.closest(`.${s}`);
-            t.getOrCreateInstance(o)[e]()
-        }))
-    };
-    class R extends z {
+    const B = t => {
+            let e = t.getAttribute("data-bs-target");
+            if (!e || "#" === e) {
+                let i = t.getAttribute("href");
+                if (!i || !i.includes("#") && !i.startsWith(".")) return null;
+                i.includes("#") && !i.startsWith("#") && (i = `#${i.split("#")[1]}`), e = i && "#" !== i ? i.trim() : null
+            }
+            return n(e)
+        },
+        z = {
+            find: (t, e = document.documentElement) => [].concat(...Element.prototype.querySelectorAll.call(e, t)),
+            findOne: (t, e = document.documentElement) => Element.prototype.querySelector.call(e, t),
+            children: (t, e) => [].concat(...t.children).filter((t => t.matches(e))),
+            parents(t, e) {
+                const i = [];
+                let n = t.parentNode.closest(e);
+                for (; n;) i.push(n), n = n.parentNode.closest(e);
+                return i
+            },
+            prev(t, e) {
+                let i = t.previousElementSibling;
+                for (; i;) {
+                    if (i.matches(e)) return [i];
+                    i = i.previousElementSibling
+                }
+                return []
+            },
+            next(t, e) {
+                let i = t.nextElementSibling;
+                for (; i;) {
+                    if (i.matches(e)) return [i];
+                    i = i.nextElementSibling
+                }
+                return []
+            },
+            focusableChildren(t) {
+                const e = ["a", "button", "input", "textarea", "select", "details", "[tabindex]", '[contenteditable="true"]'].map((t => `${t}:not([tabindex^="-"])`)).join(",");
+                return this.find(e, t).filter((t => !l(t) && a(t)))
+            },
+            getSelectorFromElement(t) {
+                const e = B(t);
+                return e && z.findOne(e) ? e : null
+            },
+            getElementFromSelector(t) {
+                const e = B(t);
+                return e ? z.findOne(e) : null
+            },
+            getMultipleElementsFromSelector(t) {
+                const e = B(t);
+                return e ? z.find(e) : []
+            }
+        },
+        R = (t, e = "hide") => {
+            const i = `click.dismiss${t.EVENT_KEY}`,
+                n = t.NAME;
+            N.on(document, i, `[data-bs-dismiss="${n}"]`, (function(i) {
+                if (["A", "AREA"].includes(this.tagName) && i.preventDefault(), l(this)) return;
+                const s = z.getElementFromSelector(this) || this.closest(`.${n}`);
+                t.getOrCreateInstance(s)[e]()
+            }))
+        },
+        q = ".bs.alert",
+        V = `close${q}`,
+        K = `closed${q}`;
+    class Q extends W {
         static get NAME() {
             return "alert"
         }
         close() {
-            if (P.trigger(this._element, "close.bs.alert").defaultPrevented) return;
+            if (N.trigger(this._element, V).defaultPrevented) return;
             this._element.classList.remove("show");
             const t = this._element.classList.contains("fade");
             this._queueCallback((() => this._destroyElement()), this._element, t)
         }
         _destroyElement() {
-            this._element.remove(), P.trigger(this._element, "closed.bs.alert"), this.dispose()
+            this._element.remove(), N.trigger(this._element, K), this.dispose()
         }
         static jQueryInterface(t) {
             return this.each((function() {
-                const e = R.getOrCreateInstance(this);
+                const e = Q.getOrCreateInstance(this);
                 if ("string" == typeof t) {
                     if (void 0 === e[t] || t.startsWith("_") || "constructor" === t) throw new TypeError(`No method named "${t}"`);
                     e[t](this)
                 }
             }))
         }
     }
-    q(R, "close"), g(R);
-    const V = '[data-bs-toggle="button"]';
-    class K extends z {
+    R(Q, "close"), m(Q);
+    const X = '[data-bs-toggle="button"]';
+    class Y extends W {
         static get NAME() {
             return "button"
         }
         toggle() {
             this._element.setAttribute("aria-pressed", this._element.classList.toggle("active"))
         }
         static jQueryInterface(t) {
             return this.each((function() {
-                const e = K.getOrCreateInstance(this);
+                const e = Y.getOrCreateInstance(this);
                 "toggle" === t && e[t]()
             }))
         }
     }
-    P.on(document, "click.bs.button.data-api", V, (t => {
+    N.on(document, "click.bs.button.data-api", X, (t => {
         t.preventDefault();
-        const e = t.target.closest(V);
-        K.getOrCreateInstance(e).toggle()
-    })), g(K);
-    const Q = {
-            find: (t, e = document.documentElement) => [].concat(...Element.prototype.querySelectorAll.call(e, t)),
-            findOne: (t, e = document.documentElement) => Element.prototype.querySelector.call(e, t),
-            children: (t, e) => [].concat(...t.children).filter((t => t.matches(e))),
-            parents(t, e) {
-                const i = [];
-                let n = t.parentNode.closest(e);
-                for (; n;) i.push(n), n = n.parentNode.closest(e);
-                return i
-            },
-            prev(t, e) {
-                let i = t.previousElementSibling;
-                for (; i;) {
-                    if (i.matches(e)) return [i];
-                    i = i.previousElementSibling
-                }
-                return []
-            },
-            next(t, e) {
-                let i = t.nextElementSibling;
-                for (; i;) {
-                    if (i.matches(e)) return [i];
-                    i = i.nextElementSibling
-                }
-                return []
-            },
-            focusableChildren(t) {
-                const e = ["a", "button", "input", "textarea", "select", "details", "[tabindex]", '[contenteditable="true"]'].map((t => `${t}:not([tabindex^="-"])`)).join(",");
-                return this.find(e, t).filter((t => !l(t) && a(t)))
-            }
-        },
-        X = {
+        const e = t.target.closest(X);
+        Y.getOrCreateInstance(e).toggle()
+    })), m(Y);
+    const U = ".bs.swipe",
+        G = `touchstart${U}`,
+        J = `touchmove${U}`,
+        Z = `touchend${U}`,
+        tt = `pointerdown${U}`,
+        et = `pointerup${U}`,
+        it = {
             endCallback: null,
             leftCallback: null,
             rightCallback: null
         },
-        Y = {
+        nt = {
             endCallback: "(function|null)",
             leftCallback: "(function|null)",
             rightCallback: "(function|null)"
         };
-    class U extends F {
+    class st extends H {
         constructor(t, e) {
-            super(), this._element = t, t && U.isSupported() && (this._config = this._getConfig(e), this._deltaX = 0, this._supportPointerEvents = Boolean(window.PointerEvent), this._initEvents())
+            super(), this._element = t, t && st.isSupported() && (this._config = this._getConfig(e), this._deltaX = 0, this._supportPointerEvents = Boolean(window.PointerEvent), this._initEvents())
         }
         static get Default() {
-            return X
+            return it
         }
         static get DefaultType() {
-            return Y
+            return nt
         }
         static get NAME() {
             return "swipe"
         }
         dispose() {
-            P.off(this._element, ".bs.swipe")
+            N.off(this._element, U)
         }
         _start(t) {
             this._supportPointerEvents ? this._eventIsPointerPenTouch(t) && (this._deltaX = t.clientX) : this._deltaX = t.touches[0].clientX
         }
         _end(t) {
-            this._eventIsPointerPenTouch(t) && (this._deltaX = t.clientX - this._deltaX), this._handleSwipe(), m(this._config.endCallback)
+            this._eventIsPointerPenTouch(t) && (this._deltaX = t.clientX - this._deltaX), this._handleSwipe(), g(this._config.endCallback)
         }
         _move(t) {
             this._deltaX = t.touches && t.touches.length > 1 ? 0 : t.touches[0].clientX - this._deltaX
         }
         _handleSwipe() {
             const t = Math.abs(this._deltaX);
             if (t <= 40) return;
             const e = t / this._deltaX;
-            this._deltaX = 0, e && m(e > 0 ? this._config.rightCallback : this._config.leftCallback)
+            this._deltaX = 0, e && g(e > 0 ? this._config.rightCallback : this._config.leftCallback)
         }
         _initEvents() {
-            this._supportPointerEvents ? (P.on(this._element, "pointerdown.bs.swipe", (t => this._start(t))), P.on(this._element, "pointerup.bs.swipe", (t => this._end(t))), this._element.classList.add("pointer-event")) : (P.on(this._element, "touchstart.bs.swipe", (t => this._start(t))), P.on(this._element, "touchmove.bs.swipe", (t => this._move(t))), P.on(this._element, "touchend.bs.swipe", (t => this._end(t))))
+            this._supportPointerEvents ? (N.on(this._element, tt, (t => this._start(t))), N.on(this._element, et, (t => this._end(t))), this._element.classList.add("pointer-event")) : (N.on(this._element, G, (t => this._start(t))), N.on(this._element, J, (t => this._move(t))), N.on(this._element, Z, (t => this._end(t))))
         }
         _eventIsPointerPenTouch(t) {
             return this._supportPointerEvents && ("pen" === t.pointerType || "touch" === t.pointerType)
         }
         static isSupported() {
             return "ontouchstart" in document.documentElement || navigator.maxTouchPoints > 0
         }
     }
-    const G = "next",
-        J = "prev",
-        Z = "left",
-        tt = "right",
-        et = "slid.bs.carousel",
-        it = "carousel",
-        nt = "active",
-        st = {
-            ArrowLeft: tt,
-            ArrowRight: Z
+    const ot = ".bs.carousel",
+        rt = ".data-api",
+        at = "next",
+        lt = "prev",
+        ct = "left",
+        ht = "right",
+        dt = `slide${ot}`,
+        ut = `slid${ot}`,
+        ft = `keydown${ot}`,
+        pt = `mouseenter${ot}`,
+        mt = `mouseleave${ot}`,
+        gt = `dragstart${ot}`,
+        _t = `load${ot}${rt}`,
+        bt = `click${ot}${rt}`,
+        vt = "carousel",
+        yt = "active",
+        wt = ".active",
+        At = ".carousel-item",
+        Et = wt + At,
+        Tt = {
+            ArrowLeft: ht,
+            ArrowRight: ct
         },
-        ot = {
+        Ct = {
             interval: 5e3,
             keyboard: !0,
             pause: "hover",
             ride: !1,
             touch: !0,
             wrap: !0
         },
-        rt = {
+        Ot = {
             interval: "(number|boolean)",
             keyboard: "boolean",
             pause: "(string|boolean)",
             ride: "(boolean|string)",
             touch: "boolean",
             wrap: "boolean"
         };
-    class at extends z {
+    class xt extends W {
         constructor(t, e) {
-            super(t, e), this._interval = null, this._activeElement = null, this._isSliding = !1, this.touchTimeout = null, this._swipeHelper = null, this._indicatorsElement = Q.findOne(".carousel-indicators", this._element), this._addEventListeners(), this._config.ride === it && this.cycle()
+            super(t, e), this._interval = null, this._activeElement = null, this._isSliding = !1, this.touchTimeout = null, this._swipeHelper = null, this._indicatorsElement = z.findOne(".carousel-indicators", this._element), this._addEventListeners(), this._config.ride === vt && this.cycle()
         }
         static get Default() {
-            return ot
+            return Ct
         }
         static get DefaultType() {
-            return rt
+            return Ot
         }
         static get NAME() {
             return "carousel"
         }
         next() {
-            this._slide(G)
+            this._slide(at)
         }
         nextWhenVisible() {
             !document.hidden && a(this._element) && this.next()
         }
         prev() {
-            this._slide(J)
+            this._slide(lt)
         }
         pause() {
             this._isSliding && s(this._element), this._clearInterval()
         }
         cycle() {
             this._clearInterval(), this._updateInterval(), this._interval = setInterval((() => this.nextWhenVisible()), this._config.interval)
         }
         _maybeEnableCycle() {
-            this._config.ride && (this._isSliding ? P.one(this._element, et, (() => this.cycle())) : this.cycle())
+            this._config.ride && (this._isSliding ? N.one(this._element, ut, (() => this.cycle())) : this.cycle())
         }
         to(t) {
             const e = this._getItems();
             if (t > e.length - 1 || t < 0) return;
-            if (this._isSliding) return void P.one(this._element, et, (() => this.to(t)));
+            if (this._isSliding) return void N.one(this._element, ut, (() => this.to(t)));
             const i = this._getItemIndex(this._getActive());
             if (i === t) return;
-            const n = t > i ? G : J;
+            const n = t > i ? at : lt;
             this._slide(n, e[t])
         }
         dispose() {
             this._swipeHelper && this._swipeHelper.dispose(), super.dispose()
         }
         _configAfterMerge(t) {
             return t.defaultInterval = t.interval, t
         }
         _addEventListeners() {
-            this._config.keyboard && P.on(this._element, "keydown.bs.carousel", (t => this._keydown(t))), "hover" === this._config.pause && (P.on(this._element, "mouseenter.bs.carousel", (() => this.pause())), P.on(this._element, "mouseleave.bs.carousel", (() => this._maybeEnableCycle()))), this._config.touch && U.isSupported() && this._addTouchEventListeners()
+            this._config.keyboard && N.on(this._element, ft, (t => this._keydown(t))), "hover" === this._config.pause && (N.on(this._element, pt, (() => this.pause())), N.on(this._element, mt, (() => this._maybeEnableCycle()))), this._config.touch && st.isSupported() && this._addTouchEventListeners()
         }
         _addTouchEventListeners() {
-            for (const t of Q.find(".carousel-item img", this._element)) P.on(t, "dragstart.bs.carousel", (t => t.preventDefault()));
+            for (const t of z.find(".carousel-item img", this._element)) N.on(t, gt, (t => t.preventDefault()));
             const t = {
-                leftCallback: () => this._slide(this._directionToOrder(Z)),
-                rightCallback: () => this._slide(this._directionToOrder(tt)),
+                leftCallback: () => this._slide(this._directionToOrder(ct)),
+                rightCallback: () => this._slide(this._directionToOrder(ht)),
                 endCallback: () => {
                     "hover" === this._config.pause && (this.pause(), this.touchTimeout && clearTimeout(this.touchTimeout), this.touchTimeout = setTimeout((() => this._maybeEnableCycle()), 500 + this._config.interval))
                 }
             };
-            this._swipeHelper = new U(this._element, t)
+            this._swipeHelper = new st(this._element, t)
         }
         _keydown(t) {
             if (/input|textarea/i.test(t.target.tagName)) return;
-            const e = st[t.key];
+            const e = Tt[t.key];
             e && (t.preventDefault(), this._slide(this._directionToOrder(e)))
         }
         _getItemIndex(t) {
             return this._getItems().indexOf(t)
         }
         _setActiveIndicatorElement(t) {
             if (!this._indicatorsElement) return;
-            const e = Q.findOne(".active", this._indicatorsElement);
-            e.classList.remove(nt), e.removeAttribute("aria-current");
-            const i = Q.findOne(`[data-bs-slide-to="${t}"]`, this._indicatorsElement);
-            i && (i.classList.add(nt), i.setAttribute("aria-current", "true"))
+            const e = z.findOne(wt, this._indicatorsElement);
+            e.classList.remove(yt), e.removeAttribute("aria-current");
+            const i = z.findOne(`[data-bs-slide-to="${t}"]`, this._indicatorsElement);
+            i && (i.classList.add(yt), i.setAttribute("aria-current", "true"))
         }
         _updateInterval() {
             const t = this._activeElement || this._getActive();
             if (!t) return;
             const e = Number.parseInt(t.getAttribute("data-bs-interval"), 10);
             this._config.interval = e || this._config.defaultInterval
         }
         _slide(t, e = null) {
             if (this._isSliding) return;
             const i = this._getActive(),
-                n = t === G,
+                n = t === at,
                 s = e || b(this._getItems(), i, n, this._config.wrap);
             if (s === i) return;
             const o = this._getItemIndex(s),
-                r = e => P.trigger(this._element, e, {
+                r = e => N.trigger(this._element, e, {
                     relatedTarget: s,
                     direction: this._orderToDirection(t),
                     from: this._getItemIndex(i),
                     to: o
                 });
-            if (r("slide.bs.carousel").defaultPrevented) return;
+            if (r(dt).defaultPrevented) return;
             if (!i || !s) return;
             const a = Boolean(this._interval);
             this.pause(), this._isSliding = !0, this._setActiveIndicatorElement(o), this._activeElement = s;
             const l = n ? "carousel-item-start" : "carousel-item-end",
                 c = n ? "carousel-item-next" : "carousel-item-prev";
             s.classList.add(c), d(s), i.classList.add(l), s.classList.add(l), this._queueCallback((() => {
-                s.classList.remove(l, c), s.classList.add(nt), i.classList.remove(nt, c, l), this._isSliding = !1, r(et)
+                s.classList.remove(l, c), s.classList.add(yt), i.classList.remove(yt, c, l), this._isSliding = !1, r(ut)
             }), i, this._isAnimated()), a && this.cycle()
         }
         _isAnimated() {
             return this._element.classList.contains("slide")
         }
         _getActive() {
-            return Q.findOne(".active.carousel-item", this._element)
+            return z.findOne(Et, this._element)
         }
         _getItems() {
-            return Q.find(".carousel-item", this._element)
+            return z.find(At, this._element)
         }
         _clearInterval() {
             this._interval && (clearInterval(this._interval), this._interval = null)
         }
         _directionToOrder(t) {
-            return p() ? t === Z ? J : G : t === Z ? G : J
+            return p() ? t === ct ? lt : at : t === ct ? at : lt
         }
         _orderToDirection(t) {
-            return p() ? t === J ? Z : tt : t === J ? tt : Z
+            return p() ? t === lt ? ct : ht : t === lt ? ht : ct
         }
         static jQueryInterface(t) {
             return this.each((function() {
-                const e = at.getOrCreateInstance(this, t);
+                const e = xt.getOrCreateInstance(this, t);
                 if ("number" != typeof t) {
                     if ("string" == typeof t) {
                         if (void 0 === e[t] || t.startsWith("_") || "constructor" === t) throw new TypeError(`No method named "${t}"`);
                         e[t]()
                     }
                 } else e.to(t)
             }))
         }
     }
-    P.on(document, "click.bs.carousel.data-api", "[data-bs-slide], [data-bs-slide-to]", (function(t) {
-        const e = n(this);
-        if (!e || !e.classList.contains(it)) return;
+    N.on(document, bt, "[data-bs-slide], [data-bs-slide-to]", (function(t) {
+        const e = z.getElementFromSelector(this);
+        if (!e || !e.classList.contains(vt)) return;
         t.preventDefault();
-        const i = at.getOrCreateInstance(e),
-            s = this.getAttribute("data-bs-slide-to");
-        return s ? (i.to(s), void i._maybeEnableCycle()) : "next" === B.getDataAttribute(this, "slide") ? (i.next(), void i._maybeEnableCycle()) : (i.prev(), void i._maybeEnableCycle())
-    })), P.on(window, "load.bs.carousel.data-api", (() => {
-        const t = Q.find('[data-bs-ride="carousel"]');
-        for (const e of t) at.getOrCreateInstance(e)
-    })), g(at);
-    const lt = "show",
-        ct = "collapse",
-        ht = "collapsing",
-        dt = '[data-bs-toggle="collapse"]',
-        ut = {
+        const i = xt.getOrCreateInstance(e),
+            n = this.getAttribute("data-bs-slide-to");
+        return n ? (i.to(n), void i._maybeEnableCycle()) : "next" === F.getDataAttribute(this, "slide") ? (i.next(), void i._maybeEnableCycle()) : (i.prev(), void i._maybeEnableCycle())
+    })), N.on(window, _t, (() => {
+        const t = z.find('[data-bs-ride="carousel"]');
+        for (const e of t) xt.getOrCreateInstance(e)
+    })), m(xt);
+    const kt = ".bs.collapse",
+        Lt = `show${kt}`,
+        St = `shown${kt}`,
+        Dt = `hide${kt}`,
+        $t = `hidden${kt}`,
+        It = `click${kt}.data-api`,
+        Nt = "show",
+        Pt = "collapse",
+        Mt = "collapsing",
+        jt = `:scope .${Pt} .${Pt}`,
+        Ft = '[data-bs-toggle="collapse"]',
+        Ht = {
             parent: null,
             toggle: !0
         },
-        ft = {
+        Wt = {
             parent: "(null|element)",
             toggle: "boolean"
         };
-    class pt extends z {
+    class Bt extends W {
         constructor(t, e) {
             super(t, e), this._isTransitioning = !1, this._triggerArray = [];
-            const n = Q.find(dt);
-            for (const t of n) {
-                const e = i(t),
-                    n = Q.find(e).filter((t => t === this._element));
-                null !== e && n.length && this._triggerArray.push(t)
+            const i = z.find(Ft);
+            for (const t of i) {
+                const e = z.getSelectorFromElement(t),
+                    i = z.find(e).filter((t => t === this._element));
+                null !== e && i.length && this._triggerArray.push(t)
             }
             this._initializeChildren(), this._config.parent || this._addAriaAndCollapsedClass(this._triggerArray, this._isShown()), this._config.toggle && this.toggle()
         }
         static get Default() {
-            return ut
+            return Ht
         }
         static get DefaultType() {
-            return ft
+            return Wt
         }
         static get NAME() {
             return "collapse"
         }
         toggle() {
             this._isShown() ? this.hide() : this.show()
         }
         show() {
             if (this._isTransitioning || this._isShown()) return;
             let t = [];
-            if (this._config.parent && (t = this._getFirstLevelChildren(".collapse.show, .collapse.collapsing").filter((t => t !== this._element)).map((t => pt.getOrCreateInstance(t, {
+            if (this._config.parent && (t = this._getFirstLevelChildren(".collapse.show, .collapse.collapsing").filter((t => t !== this._element)).map((t => Bt.getOrCreateInstance(t, {
                     toggle: !1
                 })))), t.length && t[0]._isTransitioning) return;
-            if (P.trigger(this._element, "show.bs.collapse").defaultPrevented) return;
+            if (N.trigger(this._element, Lt).defaultPrevented) return;
             for (const e of t) e.hide();
             const e = this._getDimension();
-            this._element.classList.remove(ct), this._element.classList.add(ht), this._element.style[e] = 0, this._addAriaAndCollapsedClass(this._triggerArray, !0), this._isTransitioning = !0;
+            this._element.classList.remove(Pt), this._element.classList.add(Mt), this._element.style[e] = 0, this._addAriaAndCollapsedClass(this._triggerArray, !0), this._isTransitioning = !0;
             const i = `scroll${e[0].toUpperCase()+e.slice(1)}`;
             this._queueCallback((() => {
-                this._isTransitioning = !1, this._element.classList.remove(ht), this._element.classList.add(ct, lt), this._element.style[e] = "", P.trigger(this._element, "shown.bs.collapse")
+                this._isTransitioning = !1, this._element.classList.remove(Mt), this._element.classList.add(Pt, Nt), this._element.style[e] = "", N.trigger(this._element, St)
             }), this._element, !0), this._element.style[e] = `${this._element[i]}px`
         }
         hide() {
             if (this._isTransitioning || !this._isShown()) return;
-            if (P.trigger(this._element, "hide.bs.collapse").defaultPrevented) return;
+            if (N.trigger(this._element, Dt).defaultPrevented) return;
             const t = this._getDimension();
-            this._element.style[t] = `${this._element.getBoundingClientRect()[t]}px`, d(this._element), this._element.classList.add(ht), this._element.classList.remove(ct, lt);
+            this._element.style[t] = `${this._element.getBoundingClientRect()[t]}px`, d(this._element), this._element.classList.add(Mt), this._element.classList.remove(Pt, Nt);
             for (const t of this._triggerArray) {
-                const e = n(t);
+                const e = z.getElementFromSelector(t);
                 e && !this._isShown(e) && this._addAriaAndCollapsedClass([t], !1)
             }
             this._isTransitioning = !0, this._element.style[t] = "", this._queueCallback((() => {
-                this._isTransitioning = !1, this._element.classList.remove(ht), this._element.classList.add(ct), P.trigger(this._element, "hidden.bs.collapse")
+                this._isTransitioning = !1, this._element.classList.remove(Mt), this._element.classList.add(Pt), N.trigger(this._element, $t)
             }), this._element, !0)
         }
         _isShown(t = this._element) {
-            return t.classList.contains(lt)
+            return t.classList.contains(Nt)
         }
         _configAfterMerge(t) {
             return t.toggle = Boolean(t.toggle), t.parent = r(t.parent), t
         }
         _getDimension() {
             return this._element.classList.contains("collapse-horizontal") ? "width" : "height"
         }
         _initializeChildren() {
             if (!this._config.parent) return;
-            const t = this._getFirstLevelChildren(dt);
+            const t = this._getFirstLevelChildren(Ft);
             for (const e of t) {
-                const t = n(e);
+                const t = z.getElementFromSelector(e);
                 t && this._addAriaAndCollapsedClass([e], this._isShown(t))
             }
         }
         _getFirstLevelChildren(t) {
-            const e = Q.find(":scope .collapse .collapse", this._config.parent);
-            return Q.find(t, this._config.parent).filter((t => !e.includes(t)))
+            const e = z.find(jt, this._config.parent);
+            return z.find(t, this._config.parent).filter((t => !e.includes(t)))
         }
         _addAriaAndCollapsedClass(t, e) {
             if (t.length)
                 for (const i of t) i.classList.toggle("collapsed", !e), i.setAttribute("aria-expanded", e)
         }
         static jQueryInterface(t) {
             const e = {};
             return "string" == typeof t && /show|hide/.test(t) && (e.toggle = !1), this.each((function() {
-                const i = pt.getOrCreateInstance(this, e);
+                const i = Bt.getOrCreateInstance(this, e);
                 if ("string" == typeof t) {
                     if (void 0 === i[t]) throw new TypeError(`No method named "${t}"`);
                     i[t]()
                 }
             }))
         }
     }
-    P.on(document, "click.bs.collapse.data-api", dt, (function(t) {
+    N.on(document, It, Ft, (function(t) {
         ("A" === t.target.tagName || t.delegateTarget && "A" === t.delegateTarget.tagName) && t.preventDefault();
-        const e = i(this),
-            n = Q.find(e);
-        for (const t of n) pt.getOrCreateInstance(t, {
+        for (const t of z.getMultipleElementsFromSelector(this)) Bt.getOrCreateInstance(t, {
             toggle: !1
         }).toggle()
-    })), g(pt);
-    var gt = "top",
-        mt = "bottom",
-        _t = "right",
-        bt = "left",
-        vt = "auto",
-        yt = [gt, mt, _t, bt],
-        wt = "start",
-        At = "end",
-        Et = "clippingParents",
-        Tt = "viewport",
-        Ct = "popper",
-        Ot = "reference",
-        xt = yt.reduce((function(t, e) {
-            return t.concat([e + "-" + wt, e + "-" + At])
+    })), m(Bt);
+    var zt = "top",
+        Rt = "bottom",
+        qt = "right",
+        Vt = "left",
+        Kt = "auto",
+        Qt = [zt, Rt, qt, Vt],
+        Xt = "start",
+        Yt = "end",
+        Ut = "clippingParents",
+        Gt = "viewport",
+        Jt = "popper",
+        Zt = "reference",
+        te = Qt.reduce((function(t, e) {
+            return t.concat([e + "-" + Xt, e + "-" + Yt])
         }), []),
-        kt = [].concat(yt, [vt]).reduce((function(t, e) {
-            return t.concat([e, e + "-" + wt, e + "-" + At])
+        ee = [].concat(Qt, [Kt]).reduce((function(t, e) {
+            return t.concat([e, e + "-" + Xt, e + "-" + Yt])
         }), []),
-        Lt = "beforeRead",
-        Dt = "read",
-        St = "afterRead",
-        It = "beforeMain",
-        Nt = "main",
-        Pt = "afterMain",
-        jt = "beforeWrite",
-        Mt = "write",
-        Ht = "afterWrite",
-        $t = [Lt, Dt, St, It, Nt, Pt, jt, Mt, Ht];
+        ie = "beforeRead",
+        ne = "read",
+        se = "afterRead",
+        oe = "beforeMain",
+        re = "main",
+        ae = "afterMain",
+        le = "beforeWrite",
+        ce = "write",
+        he = "afterWrite",
+        de = [ie, ne, se, oe, re, ae, le, ce, he];
 
-    function Wt(t) {
+    function ue(t) {
         return t ? (t.nodeName || "").toLowerCase() : null
     }
 
-    function Bt(t) {
+    function fe(t) {
         if (null == t) return window;
         if ("[object Window]" !== t.toString()) {
             var e = t.ownerDocument;
             return e && e.defaultView || window
         }
         return t
     }
 
-    function Ft(t) {
-        return t instanceof Bt(t).Element || t instanceof Element
+    function pe(t) {
+        return t instanceof fe(t).Element || t instanceof Element
     }
 
-    function zt(t) {
-        return t instanceof Bt(t).HTMLElement || t instanceof HTMLElement
+    function me(t) {
+        return t instanceof fe(t).HTMLElement || t instanceof HTMLElement
     }
 
-    function qt(t) {
-        return "undefined" != typeof ShadowRoot && (t instanceof Bt(t).ShadowRoot || t instanceof ShadowRoot)
+    function ge(t) {
+        return "undefined" != typeof ShadowRoot && (t instanceof fe(t).ShadowRoot || t instanceof ShadowRoot)
     }
-    const Rt = {
+    const _e = {
         name: "applyStyles",
         enabled: !0,
         phase: "write",
         fn: function(t) {
             var e = t.state;
             Object.keys(e.elements).forEach((function(t) {
                 var i = e.styles[t] || {},
                     n = e.attributes[t] || {},
                     s = e.elements[t];
-                zt(s) && Wt(s) && (Object.assign(s.style, i), Object.keys(n).forEach((function(t) {
+                me(s) && ue(s) && (Object.assign(s.style, i), Object.keys(n).forEach((function(t) {
                     var e = n[t];
                     !1 === e ? s.removeAttribute(t) : s.setAttribute(t, !0 === e ? "" : e)
                 })))
             }))
         },
         effect: function(t) {
             var e = t.state,
@@ -855,49 +876,49 @@
                 function() {
                     Object.keys(e.elements).forEach((function(t) {
                         var n = e.elements[t],
                             s = e.attributes[t] || {},
                             o = Object.keys(e.styles.hasOwnProperty(t) ? e.styles[t] : i[t]).reduce((function(t, e) {
                                 return t[e] = "", t
                             }), {});
-                        zt(n) && Wt(n) && (Object.assign(n.style, o), Object.keys(s).forEach((function(t) {
+                        me(n) && ue(n) && (Object.assign(n.style, o), Object.keys(s).forEach((function(t) {
                             n.removeAttribute(t)
                         })))
                     }))
                 }
         },
         requires: ["computeStyles"]
     };
 
-    function Vt(t) {
+    function be(t) {
         return t.split("-")[0]
     }
-    var Kt = Math.max,
-        Qt = Math.min,
-        Xt = Math.round;
+    var ve = Math.max,
+        ye = Math.min,
+        we = Math.round;
 
-    function Yt() {
+    function Ae() {
         var t = navigator.userAgentData;
-        return null != t && t.brands ? t.brands.map((function(t) {
+        return null != t && t.brands && Array.isArray(t.brands) ? t.brands.map((function(t) {
             return t.brand + "/" + t.version
         })).join(" ") : navigator.userAgent
     }
 
-    function Ut() {
-        return !/^((?!chrome|android).)*safari/i.test(Yt())
+    function Ee() {
+        return !/^((?!chrome|android).)*safari/i.test(Ae())
     }
 
-    function Gt(t, e, i) {
+    function Te(t, e, i) {
         void 0 === e && (e = !1), void 0 === i && (i = !1);
         var n = t.getBoundingClientRect(),
             s = 1,
             o = 1;
-        e && zt(t) && (s = t.offsetWidth > 0 && Xt(n.width) / t.offsetWidth || 1, o = t.offsetHeight > 0 && Xt(n.height) / t.offsetHeight || 1);
-        var r = (Ft(t) ? Bt(t) : window).visualViewport,
-            a = !Ut() && i,
+        e && me(t) && (s = t.offsetWidth > 0 && we(n.width) / t.offsetWidth || 1, o = t.offsetHeight > 0 && we(n.height) / t.offsetHeight || 1);
+        var r = (pe(t) ? fe(t) : window).visualViewport,
+            a = !Ee() && i,
             l = (n.left + (a && r ? r.offsetLeft : 0)) / s,
             c = (n.top + (a && r ? r.offsetTop : 0)) / o,
             h = n.width / s,
             d = n.height / o;
         return {
             width: h,
             height: d,
@@ -906,692 +927,692 @@
             bottom: c + d,
             left: l,
             x: l,
             y: c
         }
     }
 
-    function Jt(t) {
-        var e = Gt(t),
+    function Ce(t) {
+        var e = Te(t),
             i = t.offsetWidth,
             n = t.offsetHeight;
         return Math.abs(e.width - i) <= 1 && (i = e.width), Math.abs(e.height - n) <= 1 && (n = e.height), {
             x: t.offsetLeft,
             y: t.offsetTop,
             width: i,
             height: n
         }
     }
 
-    function Zt(t, e) {
+    function Oe(t, e) {
         var i = e.getRootNode && e.getRootNode();
         if (t.contains(e)) return !0;
-        if (i && qt(i)) {
+        if (i && ge(i)) {
             var n = e;
             do {
                 if (n && t.isSameNode(n)) return !0;
                 n = n.parentNode || n.host
             } while (n)
         }
         return !1
     }
 
-    function te(t) {
-        return Bt(t).getComputedStyle(t)
+    function xe(t) {
+        return fe(t).getComputedStyle(t)
     }
 
-    function ee(t) {
-        return ["table", "td", "th"].indexOf(Wt(t)) >= 0
+    function ke(t) {
+        return ["table", "td", "th"].indexOf(ue(t)) >= 0
     }
 
-    function ie(t) {
-        return ((Ft(t) ? t.ownerDocument : t.document) || window.document).documentElement
+    function Le(t) {
+        return ((pe(t) ? t.ownerDocument : t.document) || window.document).documentElement
     }
 
-    function ne(t) {
-        return "html" === Wt(t) ? t : t.assignedSlot || t.parentNode || (qt(t) ? t.host : null) || ie(t)
+    function Se(t) {
+        return "html" === ue(t) ? t : t.assignedSlot || t.parentNode || (ge(t) ? t.host : null) || Le(t)
     }
 
-    function se(t) {
-        return zt(t) && "fixed" !== te(t).position ? t.offsetParent : null
+    function De(t) {
+        return me(t) && "fixed" !== xe(t).position ? t.offsetParent : null
     }
 
-    function oe(t) {
-        for (var e = Bt(t), i = se(t); i && ee(i) && "static" === te(i).position;) i = se(i);
-        return i && ("html" === Wt(i) || "body" === Wt(i) && "static" === te(i).position) ? e : i || function(t) {
-            var e = /firefox/i.test(Yt());
-            if (/Trident/i.test(Yt()) && zt(t) && "fixed" === te(t).position) return null;
-            var i = ne(t);
-            for (qt(i) && (i = i.host); zt(i) && ["html", "body"].indexOf(Wt(i)) < 0;) {
-                var n = te(i);
+    function $e(t) {
+        for (var e = fe(t), i = De(t); i && ke(i) && "static" === xe(i).position;) i = De(i);
+        return i && ("html" === ue(i) || "body" === ue(i) && "static" === xe(i).position) ? e : i || function(t) {
+            var e = /firefox/i.test(Ae());
+            if (/Trident/i.test(Ae()) && me(t) && "fixed" === xe(t).position) return null;
+            var i = Se(t);
+            for (ge(i) && (i = i.host); me(i) && ["html", "body"].indexOf(ue(i)) < 0;) {
+                var n = xe(i);
                 if ("none" !== n.transform || "none" !== n.perspective || "paint" === n.contain || -1 !== ["transform", "perspective"].indexOf(n.willChange) || e && "filter" === n.willChange || e && n.filter && "none" !== n.filter) return i;
                 i = i.parentNode
             }
             return null
         }(t) || e
     }
 
-    function re(t) {
+    function Ie(t) {
         return ["top", "bottom"].indexOf(t) >= 0 ? "x" : "y"
     }
 
-    function ae(t, e, i) {
-        return Kt(t, Qt(e, i))
+    function Ne(t, e, i) {
+        return ve(t, ye(e, i))
     }
 
-    function le(t) {
+    function Pe(t) {
         return Object.assign({}, {
             top: 0,
             right: 0,
             bottom: 0,
             left: 0
         }, t)
     }
 
-    function ce(t, e) {
+    function Me(t, e) {
         return e.reduce((function(e, i) {
             return e[i] = t, e
         }), {})
     }
-    const he = {
+    const je = {
         name: "arrow",
         enabled: !0,
         phase: "main",
         fn: function(t) {
             var e, i = t.state,
                 n = t.name,
                 s = t.options,
                 o = i.elements.arrow,
                 r = i.modifiersData.popperOffsets,
-                a = Vt(i.placement),
-                l = re(a),
-                c = [bt, _t].indexOf(a) >= 0 ? "height" : "width";
+                a = be(i.placement),
+                l = Ie(a),
+                c = [Vt, qt].indexOf(a) >= 0 ? "height" : "width";
             if (o && r) {
                 var h = function(t, e) {
-                        return le("number" != typeof(t = "function" == typeof t ? t(Object.assign({}, e.rects, {
+                        return Pe("number" != typeof(t = "function" == typeof t ? t(Object.assign({}, e.rects, {
                             placement: e.placement
-                        })) : t) ? t : ce(t, yt))
+                        })) : t) ? t : Me(t, Qt))
                     }(s.padding, i),
-                    d = Jt(o),
-                    u = "y" === l ? gt : bt,
-                    f = "y" === l ? mt : _t,
+                    d = Ce(o),
+                    u = "y" === l ? zt : Vt,
+                    f = "y" === l ? Rt : qt,
                     p = i.rects.reference[c] + i.rects.reference[l] - r[l] - i.rects.popper[c],
-                    g = r[l] - i.rects.reference[l],
-                    m = oe(o),
-                    _ = m ? "y" === l ? m.clientHeight || 0 : m.clientWidth || 0 : 0,
-                    b = p / 2 - g / 2,
+                    m = r[l] - i.rects.reference[l],
+                    g = $e(o),
+                    _ = g ? "y" === l ? g.clientHeight || 0 : g.clientWidth || 0 : 0,
+                    b = p / 2 - m / 2,
                     v = h[u],
                     y = _ - d[c] - h[f],
                     w = _ / 2 - d[c] / 2 + b,
-                    A = ae(v, w, y),
+                    A = Ne(v, w, y),
                     E = l;
                 i.modifiersData[n] = ((e = {})[E] = A, e.centerOffset = A - w, e)
             }
         },
         effect: function(t) {
             var e = t.state,
                 i = t.options.element,
                 n = void 0 === i ? "[data-popper-arrow]" : i;
-            null != n && ("string" != typeof n || (n = e.elements.popper.querySelector(n))) && Zt(e.elements.popper, n) && (e.elements.arrow = n)
+            null != n && ("string" != typeof n || (n = e.elements.popper.querySelector(n))) && Oe(e.elements.popper, n) && (e.elements.arrow = n)
         },
         requires: ["popperOffsets"],
         requiresIfExists: ["preventOverflow"]
     };
 
-    function de(t) {
+    function Fe(t) {
         return t.split("-")[1]
     }
-    var ue = {
+    var He = {
         top: "auto",
         right: "auto",
         bottom: "auto",
         left: "auto"
     };
 
-    function fe(t) {
+    function We(t) {
         var e, i = t.popper,
             n = t.popperRect,
             s = t.placement,
             o = t.variation,
             r = t.offsets,
             a = t.position,
             l = t.gpuAcceleration,
             c = t.adaptive,
             h = t.roundOffsets,
             d = t.isFixed,
             u = r.x,
             f = void 0 === u ? 0 : u,
             p = r.y,
-            g = void 0 === p ? 0 : p,
-            m = "function" == typeof h ? h({
+            m = void 0 === p ? 0 : p,
+            g = "function" == typeof h ? h({
                 x: f,
-                y: g
+                y: m
             }) : {
                 x: f,
-                y: g
+                y: m
             };
-        f = m.x, g = m.y;
+        f = g.x, m = g.y;
         var _ = r.hasOwnProperty("x"),
             b = r.hasOwnProperty("y"),
-            v = bt,
-            y = gt,
+            v = Vt,
+            y = zt,
             w = window;
         if (c) {
-            var A = oe(i),
+            var A = $e(i),
                 E = "clientHeight",
                 T = "clientWidth";
-            A === Bt(i) && "static" !== te(A = ie(i)).position && "absolute" === a && (E = "scrollHeight", T = "scrollWidth"), (s === gt || (s === bt || s === _t) && o === At) && (y = mt, g -= (d && A === w && w.visualViewport ? w.visualViewport.height : A[E]) - n.height, g *= l ? 1 : -1), s !== bt && (s !== gt && s !== mt || o !== At) || (v = _t, f -= (d && A === w && w.visualViewport ? w.visualViewport.width : A[T]) - n.width, f *= l ? 1 : -1)
+            A === fe(i) && "static" !== xe(A = Le(i)).position && "absolute" === a && (E = "scrollHeight", T = "scrollWidth"), (s === zt || (s === Vt || s === qt) && o === Yt) && (y = Rt, m -= (d && A === w && w.visualViewport ? w.visualViewport.height : A[E]) - n.height, m *= l ? 1 : -1), s !== Vt && (s !== zt && s !== Rt || o !== Yt) || (v = qt, f -= (d && A === w && w.visualViewport ? w.visualViewport.width : A[T]) - n.width, f *= l ? 1 : -1)
         }
         var C, O = Object.assign({
                 position: a
-            }, c && ue),
-            x = !0 === h ? function(t) {
-                var e = t.x,
-                    i = t.y,
-                    n = window.devicePixelRatio || 1;
+            }, c && He),
+            x = !0 === h ? function(t, e) {
+                var i = t.x,
+                    n = t.y,
+                    s = e.devicePixelRatio || 1;
                 return {
-                    x: Xt(e * n) / n || 0,
-                    y: Xt(i * n) / n || 0
+                    x: we(i * s) / s || 0,
+                    y: we(n * s) / s || 0
                 }
             }({
                 x: f,
-                y: g
-            }) : {
+                y: m
+            }, fe(i)) : {
                 x: f,
-                y: g
+                y: m
             };
-        return f = x.x, g = x.y, l ? Object.assign({}, O, ((C = {})[y] = b ? "0" : "", C[v] = _ ? "0" : "", C.transform = (w.devicePixelRatio || 1) <= 1 ? "translate(" + f + "px, " + g + "px)" : "translate3d(" + f + "px, " + g + "px, 0)", C)) : Object.assign({}, O, ((e = {})[y] = b ? g + "px" : "", e[v] = _ ? f + "px" : "", e.transform = "", e))
+        return f = x.x, m = x.y, l ? Object.assign({}, O, ((C = {})[y] = b ? "0" : "", C[v] = _ ? "0" : "", C.transform = (w.devicePixelRatio || 1) <= 1 ? "translate(" + f + "px, " + m + "px)" : "translate3d(" + f + "px, " + m + "px, 0)", C)) : Object.assign({}, O, ((e = {})[y] = b ? m + "px" : "", e[v] = _ ? f + "px" : "", e.transform = "", e))
     }
-    const pe = {
+    const Be = {
         name: "computeStyles",
         enabled: !0,
         phase: "beforeWrite",
         fn: function(t) {
             var e = t.state,
                 i = t.options,
                 n = i.gpuAcceleration,
                 s = void 0 === n || n,
                 o = i.adaptive,
                 r = void 0 === o || o,
                 a = i.roundOffsets,
                 l = void 0 === a || a,
                 c = {
-                    placement: Vt(e.placement),
-                    variation: de(e.placement),
+                    placement: be(e.placement),
+                    variation: Fe(e.placement),
                     popper: e.elements.popper,
                     popperRect: e.rects.popper,
                     gpuAcceleration: s,
                     isFixed: "fixed" === e.options.strategy
                 };
-            null != e.modifiersData.popperOffsets && (e.styles.popper = Object.assign({}, e.styles.popper, fe(Object.assign({}, c, {
+            null != e.modifiersData.popperOffsets && (e.styles.popper = Object.assign({}, e.styles.popper, We(Object.assign({}, c, {
                 offsets: e.modifiersData.popperOffsets,
                 position: e.options.strategy,
                 adaptive: r,
                 roundOffsets: l
-            })))), null != e.modifiersData.arrow && (e.styles.arrow = Object.assign({}, e.styles.arrow, fe(Object.assign({}, c, {
+            })))), null != e.modifiersData.arrow && (e.styles.arrow = Object.assign({}, e.styles.arrow, We(Object.assign({}, c, {
                 offsets: e.modifiersData.arrow,
                 position: "absolute",
                 adaptive: !1,
                 roundOffsets: l
             })))), e.attributes.popper = Object.assign({}, e.attributes.popper, {
                 "data-popper-placement": e.placement
             })
         },
         data: {}
     };
-    var ge = {
+    var ze = {
         passive: !0
     };
-    const me = {
+    const Re = {
         name: "eventListeners",
         enabled: !0,
         phase: "write",
         fn: function() {},
         effect: function(t) {
             var e = t.state,
                 i = t.instance,
                 n = t.options,
                 s = n.scroll,
                 o = void 0 === s || s,
                 r = n.resize,
                 a = void 0 === r || r,
-                l = Bt(e.elements.popper),
+                l = fe(e.elements.popper),
                 c = [].concat(e.scrollParents.reference, e.scrollParents.popper);
             return o && c.forEach((function(t) {
-                    t.addEventListener("scroll", i.update, ge)
-                })), a && l.addEventListener("resize", i.update, ge),
+                    t.addEventListener("scroll", i.update, ze)
+                })), a && l.addEventListener("resize", i.update, ze),
                 function() {
                     o && c.forEach((function(t) {
-                        t.removeEventListener("scroll", i.update, ge)
-                    })), a && l.removeEventListener("resize", i.update, ge)
+                        t.removeEventListener("scroll", i.update, ze)
+                    })), a && l.removeEventListener("resize", i.update, ze)
                 }
         },
         data: {}
     };
-    var _e = {
+    var qe = {
         left: "right",
         right: "left",
         bottom: "top",
         top: "bottom"
     };
 
-    function be(t) {
+    function Ve(t) {
         return t.replace(/left|right|bottom|top/g, (function(t) {
-            return _e[t]
+            return qe[t]
         }))
     }
-    var ve = {
+    var Ke = {
         start: "end",
         end: "start"
     };
 
-    function ye(t) {
+    function Qe(t) {
         return t.replace(/start|end/g, (function(t) {
-            return ve[t]
+            return Ke[t]
         }))
     }
 
-    function we(t) {
-        var e = Bt(t);
+    function Xe(t) {
+        var e = fe(t);
         return {
             scrollLeft: e.pageXOffset,
             scrollTop: e.pageYOffset
         }
     }
 
-    function Ae(t) {
-        return Gt(ie(t)).left + we(t).scrollLeft
+    function Ye(t) {
+        return Te(Le(t)).left + Xe(t).scrollLeft
     }
 
-    function Ee(t) {
-        var e = te(t),
+    function Ue(t) {
+        var e = xe(t),
             i = e.overflow,
             n = e.overflowX,
             s = e.overflowY;
         return /auto|scroll|overlay|hidden/.test(i + s + n)
     }
 
-    function Te(t) {
-        return ["html", "body", "#document"].indexOf(Wt(t)) >= 0 ? t.ownerDocument.body : zt(t) && Ee(t) ? t : Te(ne(t))
+    function Ge(t) {
+        return ["html", "body", "#document"].indexOf(ue(t)) >= 0 ? t.ownerDocument.body : me(t) && Ue(t) ? t : Ge(Se(t))
     }
 
-    function Ce(t, e) {
+    function Je(t, e) {
         var i;
         void 0 === e && (e = []);
-        var n = Te(t),
+        var n = Ge(t),
             s = n === (null == (i = t.ownerDocument) ? void 0 : i.body),
-            o = Bt(n),
-            r = s ? [o].concat(o.visualViewport || [], Ee(n) ? n : []) : n,
+            o = fe(n),
+            r = s ? [o].concat(o.visualViewport || [], Ue(n) ? n : []) : n,
             a = e.concat(r);
-        return s ? a : a.concat(Ce(ne(r)))
+        return s ? a : a.concat(Je(Se(r)))
     }
 
-    function Oe(t) {
+    function Ze(t) {
         return Object.assign({}, t, {
             left: t.x,
             top: t.y,
             right: t.x + t.width,
             bottom: t.y + t.height
         })
     }
 
-    function xe(t, e, i) {
-        return e === Tt ? Oe(function(t, e) {
-            var i = Bt(t),
-                n = ie(t),
+    function ti(t, e, i) {
+        return e === Gt ? Ze(function(t, e) {
+            var i = fe(t),
+                n = Le(t),
                 s = i.visualViewport,
                 o = n.clientWidth,
                 r = n.clientHeight,
                 a = 0,
                 l = 0;
             if (s) {
                 o = s.width, r = s.height;
-                var c = Ut();
+                var c = Ee();
                 (c || !c && "fixed" === e) && (a = s.offsetLeft, l = s.offsetTop)
             }
             return {
                 width: o,
                 height: r,
-                x: a + Ae(t),
+                x: a + Ye(t),
                 y: l
             }
-        }(t, i)) : Ft(e) ? function(t, e) {
-            var i = Gt(t, !1, "fixed" === e);
+        }(t, i)) : pe(e) ? function(t, e) {
+            var i = Te(t, !1, "fixed" === e);
             return i.top = i.top + t.clientTop, i.left = i.left + t.clientLeft, i.bottom = i.top + t.clientHeight, i.right = i.left + t.clientWidth, i.width = t.clientWidth, i.height = t.clientHeight, i.x = i.left, i.y = i.top, i
-        }(e, i) : Oe(function(t) {
-            var e, i = ie(t),
-                n = we(t),
+        }(e, i) : Ze(function(t) {
+            var e, i = Le(t),
+                n = Xe(t),
                 s = null == (e = t.ownerDocument) ? void 0 : e.body,
-                o = Kt(i.scrollWidth, i.clientWidth, s ? s.scrollWidth : 0, s ? s.clientWidth : 0),
-                r = Kt(i.scrollHeight, i.clientHeight, s ? s.scrollHeight : 0, s ? s.clientHeight : 0),
-                a = -n.scrollLeft + Ae(t),
+                o = ve(i.scrollWidth, i.clientWidth, s ? s.scrollWidth : 0, s ? s.clientWidth : 0),
+                r = ve(i.scrollHeight, i.clientHeight, s ? s.scrollHeight : 0, s ? s.clientHeight : 0),
+                a = -n.scrollLeft + Ye(t),
                 l = -n.scrollTop;
-            return "rtl" === te(s || i).direction && (a += Kt(i.clientWidth, s ? s.clientWidth : 0) - o), {
+            return "rtl" === xe(s || i).direction && (a += ve(i.clientWidth, s ? s.clientWidth : 0) - o), {
                 width: o,
                 height: r,
                 x: a,
                 y: l
             }
-        }(ie(t)))
+        }(Le(t)))
     }
 
-    function ke(t) {
+    function ei(t) {
         var e, i = t.reference,
             n = t.element,
             s = t.placement,
-            o = s ? Vt(s) : null,
-            r = s ? de(s) : null,
+            o = s ? be(s) : null,
+            r = s ? Fe(s) : null,
             a = i.x + i.width / 2 - n.width / 2,
             l = i.y + i.height / 2 - n.height / 2;
         switch (o) {
-            case gt:
+            case zt:
                 e = {
                     x: a,
                     y: i.y - n.height
                 };
                 break;
-            case mt:
+            case Rt:
                 e = {
                     x: a,
                     y: i.y + i.height
                 };
                 break;
-            case _t:
+            case qt:
                 e = {
                     x: i.x + i.width,
                     y: l
                 };
                 break;
-            case bt:
+            case Vt:
                 e = {
                     x: i.x - n.width,
                     y: l
                 };
                 break;
             default:
                 e = {
                     x: i.x,
                     y: i.y
                 }
         }
-        var c = o ? re(o) : null;
+        var c = o ? Ie(o) : null;
         if (null != c) {
             var h = "y" === c ? "height" : "width";
             switch (r) {
-                case wt:
+                case Xt:
                     e[c] = e[c] - (i[h] / 2 - n[h] / 2);
                     break;
-                case At:
+                case Yt:
                     e[c] = e[c] + (i[h] / 2 - n[h] / 2)
             }
         }
         return e
     }
 
-    function Le(t, e) {
+    function ii(t, e) {
         void 0 === e && (e = {});
         var i = e,
             n = i.placement,
             s = void 0 === n ? t.placement : n,
             o = i.strategy,
             r = void 0 === o ? t.strategy : o,
             a = i.boundary,
-            l = void 0 === a ? Et : a,
+            l = void 0 === a ? Ut : a,
             c = i.rootBoundary,
-            h = void 0 === c ? Tt : c,
+            h = void 0 === c ? Gt : c,
             d = i.elementContext,
-            u = void 0 === d ? Ct : d,
+            u = void 0 === d ? Jt : d,
             f = i.altBoundary,
             p = void 0 !== f && f,
-            g = i.padding,
-            m = void 0 === g ? 0 : g,
-            _ = le("number" != typeof m ? m : ce(m, yt)),
-            b = u === Ct ? Ot : Ct,
+            m = i.padding,
+            g = void 0 === m ? 0 : m,
+            _ = Pe("number" != typeof g ? g : Me(g, Qt)),
+            b = u === Jt ? Zt : Jt,
             v = t.rects.popper,
             y = t.elements[p ? b : u],
             w = function(t, e, i, n) {
                 var s = "clippingParents" === e ? function(t) {
-                        var e = Ce(ne(t)),
-                            i = ["absolute", "fixed"].indexOf(te(t).position) >= 0 && zt(t) ? oe(t) : t;
-                        return Ft(i) ? e.filter((function(t) {
-                            return Ft(t) && Zt(t, i) && "body" !== Wt(t)
+                        var e = Je(Se(t)),
+                            i = ["absolute", "fixed"].indexOf(xe(t).position) >= 0 && me(t) ? $e(t) : t;
+                        return pe(i) ? e.filter((function(t) {
+                            return pe(t) && Oe(t, i) && "body" !== ue(t)
                         })) : []
                     }(t) : [].concat(e),
                     o = [].concat(s, [i]),
                     r = o[0],
                     a = o.reduce((function(e, i) {
-                        var s = xe(t, i, n);
-                        return e.top = Kt(s.top, e.top), e.right = Qt(s.right, e.right), e.bottom = Qt(s.bottom, e.bottom), e.left = Kt(s.left, e.left), e
-                    }), xe(t, r, n));
+                        var s = ti(t, i, n);
+                        return e.top = ve(s.top, e.top), e.right = ye(s.right, e.right), e.bottom = ye(s.bottom, e.bottom), e.left = ve(s.left, e.left), e
+                    }), ti(t, r, n));
                 return a.width = a.right - a.left, a.height = a.bottom - a.top, a.x = a.left, a.y = a.top, a
-            }(Ft(y) ? y : y.contextElement || ie(t.elements.popper), l, h, r),
-            A = Gt(t.elements.reference),
-            E = ke({
+            }(pe(y) ? y : y.contextElement || Le(t.elements.popper), l, h, r),
+            A = Te(t.elements.reference),
+            E = ei({
                 reference: A,
                 element: v,
                 strategy: "absolute",
                 placement: s
             }),
-            T = Oe(Object.assign({}, v, E)),
-            C = u === Ct ? T : A,
+            T = Ze(Object.assign({}, v, E)),
+            C = u === Jt ? T : A,
             O = {
                 top: w.top - C.top + _.top,
                 bottom: C.bottom - w.bottom + _.bottom,
                 left: w.left - C.left + _.left,
                 right: C.right - w.right + _.right
             },
             x = t.modifiersData.offset;
-        if (u === Ct && x) {
+        if (u === Jt && x) {
             var k = x[s];
             Object.keys(O).forEach((function(t) {
-                var e = [_t, mt].indexOf(t) >= 0 ? 1 : -1,
-                    i = [gt, mt].indexOf(t) >= 0 ? "y" : "x";
+                var e = [qt, Rt].indexOf(t) >= 0 ? 1 : -1,
+                    i = [zt, Rt].indexOf(t) >= 0 ? "y" : "x";
                 O[t] += k[i] * e
             }))
         }
         return O
     }
 
-    function De(t, e) {
+    function ni(t, e) {
         void 0 === e && (e = {});
         var i = e,
             n = i.placement,
             s = i.boundary,
             o = i.rootBoundary,
             r = i.padding,
             a = i.flipVariations,
             l = i.allowedAutoPlacements,
-            c = void 0 === l ? kt : l,
-            h = de(n),
-            d = h ? a ? xt : xt.filter((function(t) {
-                return de(t) === h
-            })) : yt,
+            c = void 0 === l ? ee : l,
+            h = Fe(n),
+            d = h ? a ? te : te.filter((function(t) {
+                return Fe(t) === h
+            })) : Qt,
             u = d.filter((function(t) {
                 return c.indexOf(t) >= 0
             }));
         0 === u.length && (u = d);
         var f = u.reduce((function(e, i) {
-            return e[i] = Le(t, {
+            return e[i] = ii(t, {
                 placement: i,
                 boundary: s,
                 rootBoundary: o,
                 padding: r
-            })[Vt(i)], e
+            })[be(i)], e
         }), {});
         return Object.keys(f).sort((function(t, e) {
             return f[t] - f[e]
         }))
     }
-    const Se = {
+    const si = {
         name: "flip",
         enabled: !0,
         phase: "main",
         fn: function(t) {
             var e = t.state,
                 i = t.options,
                 n = t.name;
             if (!e.modifiersData[n]._skip) {
-                for (var s = i.mainAxis, o = void 0 === s || s, r = i.altAxis, a = void 0 === r || r, l = i.fallbackPlacements, c = i.padding, h = i.boundary, d = i.rootBoundary, u = i.altBoundary, f = i.flipVariations, p = void 0 === f || f, g = i.allowedAutoPlacements, m = e.options.placement, _ = Vt(m), b = l || (_ !== m && p ? function(t) {
-                        if (Vt(t) === vt) return [];
-                        var e = be(t);
-                        return [ye(t), e, ye(e)]
-                    }(m) : [be(m)]), v = [m].concat(b).reduce((function(t, i) {
-                        return t.concat(Vt(i) === vt ? De(e, {
+                for (var s = i.mainAxis, o = void 0 === s || s, r = i.altAxis, a = void 0 === r || r, l = i.fallbackPlacements, c = i.padding, h = i.boundary, d = i.rootBoundary, u = i.altBoundary, f = i.flipVariations, p = void 0 === f || f, m = i.allowedAutoPlacements, g = e.options.placement, _ = be(g), b = l || (_ !== g && p ? function(t) {
+                        if (be(t) === Kt) return [];
+                        var e = Ve(t);
+                        return [Qe(t), e, Qe(e)]
+                    }(g) : [Ve(g)]), v = [g].concat(b).reduce((function(t, i) {
+                        return t.concat(be(i) === Kt ? ni(e, {
                             placement: i,
                             boundary: h,
                             rootBoundary: d,
                             padding: c,
                             flipVariations: p,
-                            allowedAutoPlacements: g
+                            allowedAutoPlacements: m
                         }) : i)
                     }), []), y = e.rects.reference, w = e.rects.popper, A = new Map, E = !0, T = v[0], C = 0; C < v.length; C++) {
                     var O = v[C],
-                        x = Vt(O),
-                        k = de(O) === wt,
-                        L = [gt, mt].indexOf(x) >= 0,
-                        D = L ? "width" : "height",
-                        S = Le(e, {
+                        x = be(O),
+                        k = Fe(O) === Xt,
+                        L = [zt, Rt].indexOf(x) >= 0,
+                        S = L ? "width" : "height",
+                        D = ii(e, {
                             placement: O,
                             boundary: h,
                             rootBoundary: d,
                             altBoundary: u,
                             padding: c
                         }),
-                        I = L ? k ? _t : bt : k ? mt : gt;
-                    y[D] > w[D] && (I = be(I));
-                    var N = be(I),
-                        P = [];
-                    if (o && P.push(S[x] <= 0), a && P.push(S[I] <= 0, S[N] <= 0), P.every((function(t) {
+                        $ = L ? k ? qt : Vt : k ? Rt : zt;
+                    y[S] > w[S] && ($ = Ve($));
+                    var I = Ve($),
+                        N = [];
+                    if (o && N.push(D[x] <= 0), a && N.push(D[$] <= 0, D[I] <= 0), N.every((function(t) {
                             return t
                         }))) {
                         T = O, E = !1;
                         break
                     }
-                    A.set(O, P)
+                    A.set(O, N)
                 }
                 if (E)
-                    for (var j = function(t) {
+                    for (var P = function(t) {
                             var e = v.find((function(e) {
                                 var i = A.get(e);
                                 if (i) return i.slice(0, t).every((function(t) {
                                     return t
                                 }))
                             }));
                             if (e) return T = e, "break"
-                        }, M = p ? 3 : 1; M > 0 && "break" !== j(M); M--);
+                        }, M = p ? 3 : 1; M > 0 && "break" !== P(M); M--);
                 e.placement !== T && (e.modifiersData[n]._skip = !0, e.placement = T, e.reset = !0)
             }
         },
         requiresIfExists: ["offset"],
         data: {
             _skip: !1
         }
     };
 
-    function Ie(t, e, i) {
+    function oi(t, e, i) {
         return void 0 === i && (i = {
             x: 0,
             y: 0
         }), {
             top: t.top - e.height - i.y,
             right: t.right - e.width + i.x,
             bottom: t.bottom - e.height + i.y,
             left: t.left - e.width - i.x
         }
     }
 
-    function Ne(t) {
-        return [gt, _t, mt, bt].some((function(e) {
+    function ri(t) {
+        return [zt, qt, Rt, Vt].some((function(e) {
             return t[e] >= 0
         }))
     }
-    const Pe = {
+    const ai = {
             name: "hide",
             enabled: !0,
             phase: "main",
             requiresIfExists: ["preventOverflow"],
             fn: function(t) {
                 var e = t.state,
                     i = t.name,
                     n = e.rects.reference,
                     s = e.rects.popper,
                     o = e.modifiersData.preventOverflow,
-                    r = Le(e, {
+                    r = ii(e, {
                         elementContext: "reference"
                     }),
-                    a = Le(e, {
+                    a = ii(e, {
                         altBoundary: !0
                     }),
-                    l = Ie(r, n),
-                    c = Ie(a, s, o),
-                    h = Ne(l),
-                    d = Ne(c);
+                    l = oi(r, n),
+                    c = oi(a, s, o),
+                    h = ri(l),
+                    d = ri(c);
                 e.modifiersData[i] = {
                     referenceClippingOffsets: l,
                     popperEscapeOffsets: c,
                     isReferenceHidden: h,
                     hasPopperEscaped: d
                 }, e.attributes.popper = Object.assign({}, e.attributes.popper, {
                     "data-popper-reference-hidden": h,
                     "data-popper-escaped": d
                 })
             }
         },
-        je = {
+        li = {
             name: "offset",
             enabled: !0,
             phase: "main",
             requires: ["popperOffsets"],
             fn: function(t) {
                 var e = t.state,
                     i = t.options,
                     n = t.name,
                     s = i.offset,
                     o = void 0 === s ? [0, 0] : s,
-                    r = kt.reduce((function(t, i) {
+                    r = ee.reduce((function(t, i) {
                         return t[i] = function(t, e, i) {
-                            var n = Vt(t),
-                                s = [bt, gt].indexOf(n) >= 0 ? -1 : 1,
+                            var n = be(t),
+                                s = [Vt, zt].indexOf(n) >= 0 ? -1 : 1,
                                 o = "function" == typeof i ? i(Object.assign({}, e, {
                                     placement: t
                                 })) : i,
                                 r = o[0],
                                 a = o[1];
-                            return r = r || 0, a = (a || 0) * s, [bt, _t].indexOf(n) >= 0 ? {
+                            return r = r || 0, a = (a || 0) * s, [Vt, qt].indexOf(n) >= 0 ? {
                                 x: a,
                                 y: r
                             } : {
                                 x: r,
                                 y: a
                             }
                         }(i, e.rects, o), t
                     }), {}),
                     a = r[e.placement],
                     l = a.x,
                     c = a.y;
                 null != e.modifiersData.popperOffsets && (e.modifiersData.popperOffsets.x += l, e.modifiersData.popperOffsets.y += c), e.modifiersData[n] = r
             }
         },
-        Me = {
+        ci = {
             name: "popperOffsets",
             enabled: !0,
             phase: "read",
             fn: function(t) {
                 var e = t.state,
                     i = t.name;
-                e.modifiersData[i] = ke({
+                e.modifiersData[i] = ei({
                     reference: e.rects.reference,
                     element: e.rects.popper,
                     strategy: "absolute",
                     placement: e.placement
                 })
             },
             data: {}
         },
-        He = {
+        hi = {
             name: "preventOverflow",
             enabled: !0,
             phase: "main",
             fn: function(t) {
                 var e = t.state,
                     i = t.options,
                     n = t.name,
@@ -1602,132 +1623,132 @@
                     l = i.boundary,
                     c = i.rootBoundary,
                     h = i.altBoundary,
                     d = i.padding,
                     u = i.tether,
                     f = void 0 === u || u,
                     p = i.tetherOffset,
-                    g = void 0 === p ? 0 : p,
-                    m = Le(e, {
+                    m = void 0 === p ? 0 : p,
+                    g = ii(e, {
                         boundary: l,
                         rootBoundary: c,
                         padding: d,
                         altBoundary: h
                     }),
-                    _ = Vt(e.placement),
-                    b = de(e.placement),
+                    _ = be(e.placement),
+                    b = Fe(e.placement),
                     v = !b,
-                    y = re(_),
+                    y = Ie(_),
                     w = "x" === y ? "y" : "x",
                     A = e.modifiersData.popperOffsets,
                     E = e.rects.reference,
                     T = e.rects.popper,
-                    C = "function" == typeof g ? g(Object.assign({}, e.rects, {
+                    C = "function" == typeof m ? m(Object.assign({}, e.rects, {
                         placement: e.placement
-                    })) : g,
+                    })) : m,
                     O = "number" == typeof C ? {
                         mainAxis: C,
                         altAxis: C
                     } : Object.assign({
                         mainAxis: 0,
                         altAxis: 0
                     }, C),
                     x = e.modifiersData.offset ? e.modifiersData.offset[e.placement] : null,
                     k = {
                         x: 0,
                         y: 0
                     };
                 if (A) {
                     if (o) {
-                        var L, D = "y" === y ? gt : bt,
-                            S = "y" === y ? mt : _t,
-                            I = "y" === y ? "height" : "width",
-                            N = A[y],
-                            P = N + m[D],
-                            j = N - m[S],
-                            M = f ? -T[I] / 2 : 0,
-                            H = b === wt ? E[I] : T[I],
-                            $ = b === wt ? -T[I] : -E[I],
-                            W = e.elements.arrow,
-                            B = f && W ? Jt(W) : {
+                        var L, S = "y" === y ? zt : Vt,
+                            D = "y" === y ? Rt : qt,
+                            $ = "y" === y ? "height" : "width",
+                            I = A[y],
+                            N = I + g[S],
+                            P = I - g[D],
+                            M = f ? -T[$] / 2 : 0,
+                            j = b === Xt ? E[$] : T[$],
+                            F = b === Xt ? -T[$] : -E[$],
+                            H = e.elements.arrow,
+                            W = f && H ? Ce(H) : {
                                 width: 0,
                                 height: 0
                             },
-                            F = e.modifiersData["arrow#persistent"] ? e.modifiersData["arrow#persistent"].padding : {
+                            B = e.modifiersData["arrow#persistent"] ? e.modifiersData["arrow#persistent"].padding : {
                                 top: 0,
                                 right: 0,
                                 bottom: 0,
                                 left: 0
                             },
-                            z = F[D],
-                            q = F[S],
-                            R = ae(0, E[I], B[I]),
-                            V = v ? E[I] / 2 - M - R - z - O.mainAxis : H - R - z - O.mainAxis,
-                            K = v ? -E[I] / 2 + M + R + q + O.mainAxis : $ + R + q + O.mainAxis,
-                            Q = e.elements.arrow && oe(e.elements.arrow),
+                            z = B[S],
+                            R = B[D],
+                            q = Ne(0, E[$], W[$]),
+                            V = v ? E[$] / 2 - M - q - z - O.mainAxis : j - q - z - O.mainAxis,
+                            K = v ? -E[$] / 2 + M + q + R + O.mainAxis : F + q + R + O.mainAxis,
+                            Q = e.elements.arrow && $e(e.elements.arrow),
                             X = Q ? "y" === y ? Q.clientTop || 0 : Q.clientLeft || 0 : 0,
                             Y = null != (L = null == x ? void 0 : x[y]) ? L : 0,
-                            U = N + K - Y,
-                            G = ae(f ? Qt(P, N + V - Y - X) : P, N, f ? Kt(j, U) : j);
-                        A[y] = G, k[y] = G - N
+                            U = I + K - Y,
+                            G = Ne(f ? ye(N, I + V - Y - X) : N, I, f ? ve(P, U) : P);
+                        A[y] = G, k[y] = G - I
                     }
                     if (a) {
-                        var J, Z = "x" === y ? gt : bt,
-                            tt = "x" === y ? mt : _t,
+                        var J, Z = "x" === y ? zt : Vt,
+                            tt = "x" === y ? Rt : qt,
                             et = A[w],
                             it = "y" === w ? "height" : "width",
-                            nt = et + m[Z],
-                            st = et - m[tt],
-                            ot = -1 !== [gt, bt].indexOf(_),
+                            nt = et + g[Z],
+                            st = et - g[tt],
+                            ot = -1 !== [zt, Vt].indexOf(_),
                             rt = null != (J = null == x ? void 0 : x[w]) ? J : 0,
                             at = ot ? nt : et - E[it] - T[it] - rt + O.altAxis,
                             lt = ot ? et + E[it] + T[it] - rt - O.altAxis : st,
                             ct = f && ot ? function(t, e, i) {
-                                var n = ae(t, e, i);
+                                var n = Ne(t, e, i);
                                 return n > i ? i : n
-                            }(at, et, lt) : ae(f ? at : nt, et, f ? lt : st);
+                            }(at, et, lt) : Ne(f ? at : nt, et, f ? lt : st);
                         A[w] = ct, k[w] = ct - et
                     }
                     e.modifiersData[n] = k
                 }
             },
             requiresIfExists: ["offset"]
         };
 
-    function $e(t, e, i) {
+    function di(t, e, i) {
         void 0 === i && (i = !1);
-        var n, s, o = zt(e),
-            r = zt(e) && function(t) {
+        var n, s, o = me(e),
+            r = me(e) && function(t) {
                 var e = t.getBoundingClientRect(),
-                    i = Xt(e.width) / t.offsetWidth || 1,
-                    n = Xt(e.height) / t.offsetHeight || 1;
+                    i = we(e.width) / t.offsetWidth || 1,
+                    n = we(e.height) / t.offsetHeight || 1;
                 return 1 !== i || 1 !== n
             }(e),
-            a = ie(e),
-            l = Gt(t, r, i),
+            a = Le(e),
+            l = Te(t, r, i),
             c = {
                 scrollLeft: 0,
                 scrollTop: 0
             },
             h = {
                 x: 0,
                 y: 0
             };
-        return (o || !o && !i) && (("body" !== Wt(e) || Ee(a)) && (c = (n = e) !== Bt(n) && zt(n) ? {
+        return (o || !o && !i) && (("body" !== ue(e) || Ue(a)) && (c = (n = e) !== fe(n) && me(n) ? {
             scrollLeft: (s = n).scrollLeft,
             scrollTop: s.scrollTop
-        } : we(n)), zt(e) ? ((h = Gt(e, !0)).x += e.clientLeft, h.y += e.clientTop) : a && (h.x = Ae(a))), {
+        } : Xe(n)), me(e) ? ((h = Te(e, !0)).x += e.clientLeft, h.y += e.clientTop) : a && (h.x = Ye(a))), {
             x: l.left + c.scrollLeft - h.x,
             y: l.top + c.scrollTop - h.y,
             width: l.width,
             height: l.height
         }
     }
 
-    function We(t) {
+    function ui(t) {
         var e = new Map,
             i = new Set,
             n = [];
 
         function s(t) {
             i.add(t.name), [].concat(t.requires || [], t.requiresIfExists || []).forEach((function(t) {
                 if (!i.has(t)) {
@@ -1738,40 +1759,40 @@
         }
         return t.forEach((function(t) {
             e.set(t.name, t)
         })), t.forEach((function(t) {
             i.has(t.name) || s(t)
         })), n
     }
-    var Be = {
+    var fi = {
         placement: "bottom",
         modifiers: [],
         strategy: "absolute"
     };
 
-    function Fe() {
+    function pi() {
         for (var t = arguments.length, e = new Array(t), i = 0; i < t; i++) e[i] = arguments[i];
         return !e.some((function(t) {
             return !(t && "function" == typeof t.getBoundingClientRect)
         }))
     }
 
-    function ze(t) {
+    function mi(t) {
         void 0 === t && (t = {});
         var e = t,
             i = e.defaultModifiers,
             n = void 0 === i ? [] : i,
             s = e.defaultOptions,
-            o = void 0 === s ? Be : s;
+            o = void 0 === s ? fi : s;
         return function(t, e, i) {
             void 0 === i && (i = o);
             var s, r, a = {
                     placement: "bottom",
                     orderedModifiers: [],
-                    options: Object.assign({}, Be, o),
+                    options: Object.assign({}, fi, o),
                     modifiersData: {},
                     elements: {
                         reference: t,
                         popper: e
                     },
                     attributes: {},
                     styles: {}
@@ -1779,20 +1800,20 @@
                 l = [],
                 c = !1,
                 h = {
                     state: a,
                     setOptions: function(i) {
                         var s = "function" == typeof i ? i(a.options) : i;
                         d(), a.options = Object.assign({}, o, a.options, s), a.scrollParents = {
-                            reference: Ft(t) ? Ce(t) : t.contextElement ? Ce(t.contextElement) : [],
-                            popper: Ce(e)
+                            reference: pe(t) ? Je(t) : t.contextElement ? Je(t.contextElement) : [],
+                            popper: Je(e)
                         };
                         var r, c, u = function(t) {
-                            var e = We(t);
-                            return $t.reduce((function(t, i) {
+                            var e = ui(t);
+                            return de.reduce((function(t, i) {
                                 return t.concat(e.filter((function(t) {
                                     return t.phase === i
                                 })))
                             }), [])
                         }((r = [].concat(n, a.options.modifiers), c = r.reduce((function(t, e) {
                             var i = t[e.name];
                             return t[e.name] = i ? Object.assign({}, i, e, {
@@ -1821,18 +1842,18 @@
                         })), h.update()
                     },
                     forceUpdate: function() {
                         if (!c) {
                             var t = a.elements,
                                 e = t.reference,
                                 i = t.popper;
-                            if (Fe(e, i)) {
+                            if (pi(e, i)) {
                                 a.rects = {
-                                    reference: $e(e, oe(i), "fixed" === a.options.strategy),
-                                    popper: Jt(i)
+                                    reference: di(e, $e(i), "fixed" === a.options.strategy),
+                                    popper: Ce(i)
                                 }, a.reset = !1, a.placement = a.options.placement, a.orderedModifiers.forEach((function(t) {
                                     return a.modifiersData[t.name] = Object.assign({}, t.data)
                                 }));
                                 for (var n = 0; n < a.orderedModifiers.length; n++)
                                     if (!0 !== a.reset) {
                                         var s = a.orderedModifiers[n],
                                             o = s.fn,
@@ -1860,132 +1881,139 @@
                             }))
                         }))), r
                     }),
                     destroy: function() {
                         d(), c = !0
                     }
                 };
-            if (!Fe(t, e)) return h;
+            if (!pi(t, e)) return h;
 
             function d() {
                 l.forEach((function(t) {
                     return t()
                 })), l = []
             }
             return h.setOptions(i).then((function(t) {
                 !c && i.onFirstUpdate && i.onFirstUpdate(t)
             })), h
         }
     }
-    var qe = ze(),
-        Re = ze({
-            defaultModifiers: [me, Me, pe, Rt]
+    var gi = mi(),
+        _i = mi({
+            defaultModifiers: [Re, ci, Be, _e]
         }),
-        Ve = ze({
-            defaultModifiers: [me, Me, pe, Rt, je, Se, He, he, Pe]
+        bi = mi({
+            defaultModifiers: [Re, ci, Be, _e, li, si, hi, je, ai]
         });
-    const Ke = Object.freeze(Object.defineProperty({
+    const vi = Object.freeze(Object.defineProperty({
             __proto__: null,
-            popperGenerator: ze,
-            detectOverflow: Le,
-            createPopperBase: qe,
-            createPopper: Ve,
-            createPopperLite: Re,
-            top: gt,
-            bottom: mt,
-            right: _t,
-            left: bt,
-            auto: vt,
-            basePlacements: yt,
-            start: wt,
-            end: At,
-            clippingParents: Et,
-            viewport: Tt,
-            popper: Ct,
-            reference: Ot,
-            variationPlacements: xt,
-            placements: kt,
-            beforeRead: Lt,
-            read: Dt,
-            afterRead: St,
-            beforeMain: It,
-            main: Nt,
-            afterMain: Pt,
-            beforeWrite: jt,
-            write: Mt,
-            afterWrite: Ht,
-            modifierPhases: $t,
-            applyStyles: Rt,
-            arrow: he,
-            computeStyles: pe,
-            eventListeners: me,
-            flip: Se,
-            hide: Pe,
-            offset: je,
-            popperOffsets: Me,
-            preventOverflow: He
+            afterMain: ae,
+            afterRead: se,
+            afterWrite: he,
+            applyStyles: _e,
+            arrow: je,
+            auto: Kt,
+            basePlacements: Qt,
+            beforeMain: oe,
+            beforeRead: ie,
+            beforeWrite: le,
+            bottom: Rt,
+            clippingParents: Ut,
+            computeStyles: Be,
+            createPopper: bi,
+            createPopperBase: gi,
+            createPopperLite: _i,
+            detectOverflow: ii,
+            end: Yt,
+            eventListeners: Re,
+            flip: si,
+            hide: ai,
+            left: Vt,
+            main: re,
+            modifierPhases: de,
+            offset: li,
+            placements: ee,
+            popper: Jt,
+            popperGenerator: mi,
+            popperOffsets: ci,
+            preventOverflow: hi,
+            read: ne,
+            reference: Zt,
+            right: qt,
+            start: Xt,
+            top: zt,
+            variationPlacements: te,
+            viewport: Gt,
+            write: ce
         }, Symbol.toStringTag, {
             value: "Module"
         })),
-        Qe = "dropdown",
-        Xe = "ArrowUp",
-        Ye = "ArrowDown",
-        Ue = "click.bs.dropdown.data-api",
-        Ge = "keydown.bs.dropdown.data-api",
-        Je = "show",
-        Ze = '[data-bs-toggle="dropdown"]:not(.disabled):not(:disabled)',
-        ti = `${Ze}.show`,
-        ei = ".dropdown-menu",
-        ii = p() ? "top-end" : "top-start",
-        ni = p() ? "top-start" : "top-end",
-        si = p() ? "bottom-end" : "bottom-start",
-        oi = p() ? "bottom-start" : "bottom-end",
-        ri = p() ? "left-start" : "right-start",
-        ai = p() ? "right-start" : "left-start",
-        li = {
+        yi = "dropdown",
+        wi = ".bs.dropdown",
+        Ai = ".data-api",
+        Ei = "ArrowUp",
+        Ti = "ArrowDown",
+        Ci = `hide${wi}`,
+        Oi = `hidden${wi}`,
+        xi = `show${wi}`,
+        ki = `shown${wi}`,
+        Li = `click${wi}${Ai}`,
+        Si = `keydown${wi}${Ai}`,
+        Di = `keyup${wi}${Ai}`,
+        $i = "show",
+        Ii = '[data-bs-toggle="dropdown"]:not(.disabled):not(:disabled)',
+        Ni = `${Ii}.${$i}`,
+        Pi = ".dropdown-menu",
+        Mi = p() ? "top-end" : "top-start",
+        ji = p() ? "top-start" : "top-end",
+        Fi = p() ? "bottom-end" : "bottom-start",
+        Hi = p() ? "bottom-start" : "bottom-end",
+        Wi = p() ? "left-start" : "right-start",
+        Bi = p() ? "right-start" : "left-start",
+        zi = {
             autoClose: !0,
             boundary: "clippingParents",
             display: "dynamic",
             offset: [0, 2],
             popperConfig: null,
             reference: "toggle"
         },
-        ci = {
+        Ri = {
             autoClose: "(boolean|string)",
             boundary: "(string|element)",
             display: "string",
             offset: "(array|string|function)",
             popperConfig: "(null|object|function)",
             reference: "(string|element|object)"
         };
-    class hi extends z {
+    class qi extends W {
         constructor(t, e) {
-            super(t, e), this._popper = null, this._parent = this._element.parentNode, this._menu = Q.next(this._element, ei)[0] || Q.prev(this._element, ei)[0] || Q.findOne(ei, this._parent), this._inNavbar = this._detectNavbar()
+            super(t, e), this._popper = null, this._parent = this._element.parentNode, this._menu = z.next(this._element, Pi)[0] || z.prev(this._element, Pi)[0] || z.findOne(Pi, this._parent), this._inNavbar = this._detectNavbar()
         }
         static get Default() {
-            return li
+            return zi
         }
         static get DefaultType() {
-            return ci
+            return Ri
         }
         static get NAME() {
-            return Qe
+            return yi
         }
         toggle() {
             return this._isShown() ? this.hide() : this.show()
         }
         show() {
             if (l(this._element) || this._isShown()) return;
             const t = {
                 relatedTarget: this._element
             };
-            if (!P.trigger(this._element, "show.bs.dropdown", t).defaultPrevented) {
+            if (!N.trigger(this._element, xi, t).defaultPrevented) {
                 if (this._createPopper(), "ontouchstart" in document.documentElement && !this._parent.closest(".navbar-nav"))
-                    for (const t of [].concat(...document.body.children)) P.on(t, "mouseover", h);
-                this._element.focus(), this._element.setAttribute("aria-expanded", !0), this._menu.classList.add(Je), this._element.classList.add(Je), P.trigger(this._element, "shown.bs.dropdown", t)
+                    for (const t of [].concat(...document.body.children)) N.on(t, "mouseover", h);
+                this._element.focus(), this._element.setAttribute("aria-expanded", !0), this._menu.classList.add($i), this._element.classList.add($i), N.trigger(this._element, ki, t)
             }
         }
         hide() {
             if (l(this._element) || !this._isShown()) return;
             const t = {
                 relatedTarget: this._element
             };
@@ -1994,42 +2022,42 @@
         dispose() {
             this._popper && this._popper.destroy(), super.dispose()
         }
         update() {
             this._inNavbar = this._detectNavbar(), this._popper && this._popper.update()
         }
         _completeHide(t) {
-            if (!P.trigger(this._element, "hide.bs.dropdown", t).defaultPrevented) {
+            if (!N.trigger(this._element, Ci, t).defaultPrevented) {
                 if ("ontouchstart" in document.documentElement)
-                    for (const t of [].concat(...document.body.children)) P.off(t, "mouseover", h);
-                this._popper && this._popper.destroy(), this._menu.classList.remove(Je), this._element.classList.remove(Je), this._element.setAttribute("aria-expanded", "false"), B.removeDataAttribute(this._menu, "popper"), P.trigger(this._element, "hidden.bs.dropdown", t)
+                    for (const t of [].concat(...document.body.children)) N.off(t, "mouseover", h);
+                this._popper && this._popper.destroy(), this._menu.classList.remove($i), this._element.classList.remove($i), this._element.setAttribute("aria-expanded", "false"), F.removeDataAttribute(this._menu, "popper"), N.trigger(this._element, Oi, t)
             }
         }
         _getConfig(t) {
-            if ("object" == typeof(t = super._getConfig(t)).reference && !o(t.reference) && "function" != typeof t.reference.getBoundingClientRect) throw new TypeError(`${Qe.toUpperCase()}: Option "reference" provided type "object" without a required "getBoundingClientRect" method.`);
+            if ("object" == typeof(t = super._getConfig(t)).reference && !o(t.reference) && "function" != typeof t.reference.getBoundingClientRect) throw new TypeError(`${yi.toUpperCase()}: Option "reference" provided type "object" without a required "getBoundingClientRect" method.`);
             return t
         }
         _createPopper() {
-            if (void 0 === Ke) throw new TypeError("Bootstrap's dropdowns require Popper (https://popper.js.org)");
+            if (void 0 === vi) throw new TypeError("Bootstrap's dropdowns require Popper (https://popper.js.org)");
             let t = this._element;
             "parent" === this._config.reference ? t = this._parent : o(this._config.reference) ? t = r(this._config.reference) : "object" == typeof this._config.reference && (t = this._config.reference);
             const e = this._getPopperConfig();
-            this._popper = Ve(t, this._menu, e)
+            this._popper = bi(t, this._menu, e)
         }
         _isShown() {
-            return this._menu.classList.contains(Je)
+            return this._menu.classList.contains($i)
         }
         _getPlacement() {
             const t = this._parent;
-            if (t.classList.contains("dropend")) return ri;
-            if (t.classList.contains("dropstart")) return ai;
+            if (t.classList.contains("dropend")) return Wi;
+            if (t.classList.contains("dropstart")) return Bi;
             if (t.classList.contains("dropup-center")) return "top";
             if (t.classList.contains("dropdown-center")) return "bottom";
             const e = "end" === getComputedStyle(this._menu).getPropertyValue("--bs-position").trim();
-            return t.classList.contains("dropup") ? e ? ni : ii : e ? oi : si
+            return t.classList.contains("dropup") ? e ? ji : Mi : e ? Hi : Fi
         }
         _detectNavbar() {
             return null !== this._element.closest(".navbar")
         }
         _getOffset() {
             const {
                 offset: t
@@ -2047,318 +2075,329 @@
                 }, {
                     name: "offset",
                     options: {
                         offset: this._getOffset()
                     }
                 }]
             };
-            return (this._inNavbar || "static" === this._config.display) && (B.setDataAttribute(this._menu, "popper", "static"), t.modifiers = [{
+            return (this._inNavbar || "static" === this._config.display) && (F.setDataAttribute(this._menu, "popper", "static"), t.modifiers = [{
                 name: "applyStyles",
                 enabled: !1
             }]), {
                 ...t,
-                ..."function" == typeof this._config.popperConfig ? this._config.popperConfig(t) : this._config.popperConfig
+                ...g(this._config.popperConfig, [t])
             }
         }
         _selectMenuItem({
             key: t,
             target: e
         }) {
-            const i = Q.find(".dropdown-menu .dropdown-item:not(.disabled):not(:disabled)", this._menu).filter((t => a(t)));
-            i.length && b(i, e, t === Ye, !i.includes(e)).focus()
+            const i = z.find(".dropdown-menu .dropdown-item:not(.disabled):not(:disabled)", this._menu).filter((t => a(t)));
+            i.length && b(i, e, t === Ti, !i.includes(e)).focus()
         }
         static jQueryInterface(t) {
             return this.each((function() {
-                const e = hi.getOrCreateInstance(this, t);
+                const e = qi.getOrCreateInstance(this, t);
                 if ("string" == typeof t) {
                     if (void 0 === e[t]) throw new TypeError(`No method named "${t}"`);
                     e[t]()
                 }
             }))
         }
         static clearMenus(t) {
             if (2 === t.button || "keyup" === t.type && "Tab" !== t.key) return;
-            const e = Q.find(ti);
+            const e = z.find(Ni);
             for (const i of e) {
-                const e = hi.getInstance(i);
+                const e = qi.getInstance(i);
                 if (!e || !1 === e._config.autoClose) continue;
                 const n = t.composedPath(),
                     s = n.includes(e._menu);
                 if (n.includes(e._element) || "inside" === e._config.autoClose && !s || "outside" === e._config.autoClose && s) continue;
                 if (e._menu.contains(t.target) && ("keyup" === t.type && "Tab" === t.key || /input|select|option|textarea|form/i.test(t.target.tagName))) continue;
                 const o = {
                     relatedTarget: e._element
                 };
                 "click" === t.type && (o.clickEvent = t), e._completeHide(o)
             }
         }
         static dataApiKeydownHandler(t) {
             const e = /input|textarea/i.test(t.target.tagName),
                 i = "Escape" === t.key,
-                n = [Xe, Ye].includes(t.key);
+                n = [Ei, Ti].includes(t.key);
             if (!n && !i) return;
             if (e && !i) return;
             t.preventDefault();
-            const s = this.matches(Ze) ? this : Q.prev(this, Ze)[0] || Q.next(this, Ze)[0] || Q.findOne(Ze, t.delegateTarget.parentNode),
-                o = hi.getOrCreateInstance(s);
+            const s = this.matches(Ii) ? this : z.prev(this, Ii)[0] || z.next(this, Ii)[0] || z.findOne(Ii, t.delegateTarget.parentNode),
+                o = qi.getOrCreateInstance(s);
             if (n) return t.stopPropagation(), o.show(), void o._selectMenuItem(t);
             o._isShown() && (t.stopPropagation(), o.hide(), s.focus())
         }
     }
-    P.on(document, Ge, Ze, hi.dataApiKeydownHandler), P.on(document, Ge, ei, hi.dataApiKeydownHandler), P.on(document, Ue, hi.clearMenus), P.on(document, "keyup.bs.dropdown.data-api", hi.clearMenus), P.on(document, Ue, Ze, (function(t) {
-        t.preventDefault(), hi.getOrCreateInstance(this).toggle()
-    })), g(hi);
-    const di = ".fixed-top, .fixed-bottom, .is-fixed, .sticky-top",
-        ui = ".sticky-top",
-        fi = "padding-right",
-        pi = "margin-right";
-    class gi {
-        constructor() {
-            this._element = document.body
-        }
-        getWidth() {
-            const t = document.documentElement.clientWidth;
-            return Math.abs(window.innerWidth - t)
-        }
-        hide() {
-            const t = this.getWidth();
-            this._disableOverFlow(), this._setElementAttributes(this._element, fi, (e => e + t)), this._setElementAttributes(di, fi, (e => e + t)), this._setElementAttributes(ui, pi, (e => e - t))
-        }
-        reset() {
-            this._resetElementAttributes(this._element, "overflow"), this._resetElementAttributes(this._element, fi), this._resetElementAttributes(di, fi), this._resetElementAttributes(ui, pi)
-        }
-        isOverflowing() {
-            return this.getWidth() > 0
-        }
-        _disableOverFlow() {
-            this._saveInitialAttribute(this._element, "overflow"), this._element.style.overflow = "hidden"
-        }
-        _setElementAttributes(t, e, i) {
-            const n = this.getWidth();
-            this._applyManipulationCallback(t, (t => {
-                if (t !== this._element && window.innerWidth > t.clientWidth + n) return;
-                this._saveInitialAttribute(t, e);
-                const s = window.getComputedStyle(t).getPropertyValue(e);
-                t.style.setProperty(e, `${i(Number.parseFloat(s))}px`)
-            }))
-        }
-        _saveInitialAttribute(t, e) {
-            const i = t.style.getPropertyValue(e);
-            i && B.setDataAttribute(t, e, i)
-        }
-        _resetElementAttributes(t, e) {
-            this._applyManipulationCallback(t, (t => {
-                const i = B.getDataAttribute(t, e);
-                null !== i ? (B.removeDataAttribute(t, e), t.style.setProperty(e, i)) : t.style.removeProperty(e)
-            }))
-        }
-        _applyManipulationCallback(t, e) {
-            if (o(t)) e(t);
-            else
-                for (const i of Q.find(t, this._element)) e(i)
-        }
-    }
-    const mi = "show",
-        _i = "mousedown.bs.backdrop",
-        bi = {
+    N.on(document, Si, Ii, qi.dataApiKeydownHandler), N.on(document, Si, Pi, qi.dataApiKeydownHandler), N.on(document, Li, qi.clearMenus), N.on(document, Di, qi.clearMenus), N.on(document, Li, Ii, (function(t) {
+        t.preventDefault(), qi.getOrCreateInstance(this).toggle()
+    })), m(qi);
+    const Vi = "backdrop",
+        Ki = "show",
+        Qi = `mousedown.bs.${Vi}`,
+        Xi = {
             className: "modal-backdrop",
             clickCallback: null,
             isAnimated: !1,
             isVisible: !0,
             rootElement: "body"
         },
-        vi = {
+        Yi = {
             className: "string",
             clickCallback: "(function|null)",
             isAnimated: "boolean",
             isVisible: "boolean",
             rootElement: "(element|string)"
         };
-    class yi extends F {
+    class Ui extends H {
         constructor(t) {
             super(), this._config = this._getConfig(t), this._isAppended = !1, this._element = null
         }
         static get Default() {
-            return bi
+            return Xi
         }
         static get DefaultType() {
-            return vi
+            return Yi
         }
         static get NAME() {
-            return "backdrop"
+            return Vi
         }
         show(t) {
-            if (!this._config.isVisible) return void m(t);
+            if (!this._config.isVisible) return void g(t);
             this._append();
             const e = this._getElement();
-            this._config.isAnimated && d(e), e.classList.add(mi), this._emulateAnimation((() => {
-                m(t)
+            this._config.isAnimated && d(e), e.classList.add(Ki), this._emulateAnimation((() => {
+                g(t)
             }))
         }
         hide(t) {
-            this._config.isVisible ? (this._getElement().classList.remove(mi), this._emulateAnimation((() => {
-                this.dispose(), m(t)
-            }))) : m(t)
+            this._config.isVisible ? (this._getElement().classList.remove(Ki), this._emulateAnimation((() => {
+                this.dispose(), g(t)
+            }))) : g(t)
         }
         dispose() {
-            this._isAppended && (P.off(this._element, _i), this._element.remove(), this._isAppended = !1)
+            this._isAppended && (N.off(this._element, Qi), this._element.remove(), this._isAppended = !1)
         }
         _getElement() {
             if (!this._element) {
                 const t = document.createElement("div");
                 t.className = this._config.className, this._config.isAnimated && t.classList.add("fade"), this._element = t
             }
             return this._element
         }
         _configAfterMerge(t) {
             return t.rootElement = r(t.rootElement), t
         }
         _append() {
             if (this._isAppended) return;
             const t = this._getElement();
-            this._config.rootElement.append(t), P.on(t, _i, (() => {
-                m(this._config.clickCallback)
+            this._config.rootElement.append(t), N.on(t, Qi, (() => {
+                g(this._config.clickCallback)
             })), this._isAppended = !0
         }
         _emulateAnimation(t) {
             _(t, this._getElement(), this._config.isAnimated)
         }
     }
-    const wi = ".bs.focustrap",
-        Ai = "backward",
-        Ei = {
+    const Gi = ".bs.focustrap",
+        Ji = `focusin${Gi}`,
+        Zi = `keydown.tab${Gi}`,
+        tn = "backward",
+        en = {
             autofocus: !0,
             trapElement: null
         },
-        Ti = {
+        nn = {
             autofocus: "boolean",
             trapElement: "element"
         };
-    class Ci extends F {
+    class sn extends H {
         constructor(t) {
             super(), this._config = this._getConfig(t), this._isActive = !1, this._lastTabNavDirection = null
         }
         static get Default() {
-            return Ei
+            return en
         }
         static get DefaultType() {
-            return Ti
+            return nn
         }
         static get NAME() {
             return "focustrap"
         }
         activate() {
-            this._isActive || (this._config.autofocus && this._config.trapElement.focus(), P.off(document, wi), P.on(document, "focusin.bs.focustrap", (t => this._handleFocusin(t))), P.on(document, "keydown.tab.bs.focustrap", (t => this._handleKeydown(t))), this._isActive = !0)
+            this._isActive || (this._config.autofocus && this._config.trapElement.focus(), N.off(document, Gi), N.on(document, Ji, (t => this._handleFocusin(t))), N.on(document, Zi, (t => this._handleKeydown(t))), this._isActive = !0)
         }
         deactivate() {
-            this._isActive && (this._isActive = !1, P.off(document, wi))
+            this._isActive && (this._isActive = !1, N.off(document, Gi))
         }
         _handleFocusin(t) {
             const {
                 trapElement: e
             } = this._config;
             if (t.target === document || t.target === e || e.contains(t.target)) return;
-            const i = Q.focusableChildren(e);
-            0 === i.length ? e.focus() : this._lastTabNavDirection === Ai ? i[i.length - 1].focus() : i[0].focus()
+            const i = z.focusableChildren(e);
+            0 === i.length ? e.focus() : this._lastTabNavDirection === tn ? i[i.length - 1].focus() : i[0].focus()
         }
         _handleKeydown(t) {
-            "Tab" === t.key && (this._lastTabNavDirection = t.shiftKey ? Ai : "forward")
+            "Tab" === t.key && (this._lastTabNavDirection = t.shiftKey ? tn : "forward")
         }
     }
-    const Oi = "hidden.bs.modal",
-        xi = "show.bs.modal",
-        ki = "modal-open",
-        Li = "show",
-        Di = "modal-static",
-        Si = {
+    const on = ".fixed-top, .fixed-bottom, .is-fixed, .sticky-top",
+        rn = ".sticky-top",
+        an = "padding-right",
+        ln = "margin-right";
+    class cn {
+        constructor() {
+            this._element = document.body
+        }
+        getWidth() {
+            const t = document.documentElement.clientWidth;
+            return Math.abs(window.innerWidth - t)
+        }
+        hide() {
+            const t = this.getWidth();
+            this._disableOverFlow(), this._setElementAttributes(this._element, an, (e => e + t)), this._setElementAttributes(on, an, (e => e + t)), this._setElementAttributes(rn, ln, (e => e - t))
+        }
+        reset() {
+            this._resetElementAttributes(this._element, "overflow"), this._resetElementAttributes(this._element, an), this._resetElementAttributes(on, an), this._resetElementAttributes(rn, ln)
+        }
+        isOverflowing() {
+            return this.getWidth() > 0
+        }
+        _disableOverFlow() {
+            this._saveInitialAttribute(this._element, "overflow"), this._element.style.overflow = "hidden"
+        }
+        _setElementAttributes(t, e, i) {
+            const n = this.getWidth();
+            this._applyManipulationCallback(t, (t => {
+                if (t !== this._element && window.innerWidth > t.clientWidth + n) return;
+                this._saveInitialAttribute(t, e);
+                const s = window.getComputedStyle(t).getPropertyValue(e);
+                t.style.setProperty(e, `${i(Number.parseFloat(s))}px`)
+            }))
+        }
+        _saveInitialAttribute(t, e) {
+            const i = t.style.getPropertyValue(e);
+            i && F.setDataAttribute(t, e, i)
+        }
+        _resetElementAttributes(t, e) {
+            this._applyManipulationCallback(t, (t => {
+                const i = F.getDataAttribute(t, e);
+                null !== i ? (F.removeDataAttribute(t, e), t.style.setProperty(e, i)) : t.style.removeProperty(e)
+            }))
+        }
+        _applyManipulationCallback(t, e) {
+            if (o(t)) e(t);
+            else
+                for (const i of z.find(t, this._element)) e(i)
+        }
+    }
+    const hn = ".bs.modal",
+        dn = `hide${hn}`,
+        un = `hidePrevented${hn}`,
+        fn = `hidden${hn}`,
+        pn = `show${hn}`,
+        mn = `shown${hn}`,
+        gn = `resize${hn}`,
+        _n = `click.dismiss${hn}`,
+        bn = `mousedown.dismiss${hn}`,
+        vn = `keydown.dismiss${hn}`,
+        yn = `click${hn}.data-api`,
+        wn = "modal-open",
+        An = "show",
+        En = "modal-static",
+        Tn = {
             backdrop: !0,
             focus: !0,
             keyboard: !0
         },
-        Ii = {
+        Cn = {
             backdrop: "(boolean|string)",
             focus: "boolean",
             keyboard: "boolean"
         };
-    class Ni extends z {
+    class On extends W {
         constructor(t, e) {
-            super(t, e), this._dialog = Q.findOne(".modal-dialog", this._element), this._backdrop = this._initializeBackDrop(), this._focustrap = this._initializeFocusTrap(), this._isShown = !1, this._isTransitioning = !1, this._scrollBar = new gi, this._addEventListeners()
+            super(t, e), this._dialog = z.findOne(".modal-dialog", this._element), this._backdrop = this._initializeBackDrop(), this._focustrap = this._initializeFocusTrap(), this._isShown = !1, this._isTransitioning = !1, this._scrollBar = new cn, this._addEventListeners()
         }
         static get Default() {
-            return Si
+            return Tn
         }
         static get DefaultType() {
-            return Ii
+            return Cn
         }
         static get NAME() {
             return "modal"
         }
         toggle(t) {
             return this._isShown ? this.hide() : this.show(t)
         }
         show(t) {
-            this._isShown || this._isTransitioning || P.trigger(this._element, xi, {
+            this._isShown || this._isTransitioning || N.trigger(this._element, pn, {
                 relatedTarget: t
-            }).defaultPrevented || (this._isShown = !0, this._isTransitioning = !0, this._scrollBar.hide(), document.body.classList.add(ki), this._adjustDialog(), this._backdrop.show((() => this._showElement(t))))
+            }).defaultPrevented || (this._isShown = !0, this._isTransitioning = !0, this._scrollBar.hide(), document.body.classList.add(wn), this._adjustDialog(), this._backdrop.show((() => this._showElement(t))))
         }
         hide() {
-            this._isShown && !this._isTransitioning && (P.trigger(this._element, "hide.bs.modal").defaultPrevented || (this._isShown = !1, this._isTransitioning = !0, this._focustrap.deactivate(), this._element.classList.remove(Li), this._queueCallback((() => this._hideModal()), this._element, this._isAnimated())))
+            this._isShown && !this._isTransitioning && (N.trigger(this._element, dn).defaultPrevented || (this._isShown = !1, this._isTransitioning = !0, this._focustrap.deactivate(), this._element.classList.remove(An), this._queueCallback((() => this._hideModal()), this._element, this._isAnimated())))
         }
         dispose() {
-            for (const t of [window, this._dialog]) P.off(t, ".bs.modal");
-            this._backdrop.dispose(), this._focustrap.deactivate(), super.dispose()
+            N.off(window, hn), N.off(this._dialog, hn), this._backdrop.dispose(), this._focustrap.deactivate(), super.dispose()
         }
         handleUpdate() {
             this._adjustDialog()
         }
         _initializeBackDrop() {
-            return new yi({
+            return new Ui({
                 isVisible: Boolean(this._config.backdrop),
                 isAnimated: this._isAnimated()
             })
         }
         _initializeFocusTrap() {
-            return new Ci({
+            return new sn({
                 trapElement: this._element
             })
         }
         _showElement(t) {
             document.body.contains(this._element) || document.body.append(this._element), this._element.style.display = "block", this._element.removeAttribute("aria-hidden"), this._element.setAttribute("aria-modal", !0), this._element.setAttribute("role", "dialog"), this._element.scrollTop = 0;
-            const e = Q.findOne(".modal-body", this._dialog);
-            e && (e.scrollTop = 0), d(this._element), this._element.classList.add(Li), this._queueCallback((() => {
-                this._config.focus && this._focustrap.activate(), this._isTransitioning = !1, P.trigger(this._element, "shown.bs.modal", {
+            const e = z.findOne(".modal-body", this._dialog);
+            e && (e.scrollTop = 0), d(this._element), this._element.classList.add(An), this._queueCallback((() => {
+                this._config.focus && this._focustrap.activate(), this._isTransitioning = !1, N.trigger(this._element, mn, {
                     relatedTarget: t
                 })
             }), this._dialog, this._isAnimated())
         }
         _addEventListeners() {
-            P.on(this._element, "keydown.dismiss.bs.modal", (t => {
-                if ("Escape" === t.key) return this._config.keyboard ? (t.preventDefault(), void this.hide()) : void this._triggerBackdropTransition()
-            })), P.on(window, "resize.bs.modal", (() => {
+            N.on(this._element, vn, (t => {
+                "Escape" === t.key && (this._config.keyboard ? this.hide() : this._triggerBackdropTransition())
+            })), N.on(window, gn, (() => {
                 this._isShown && !this._isTransitioning && this._adjustDialog()
-            })), P.on(this._element, "mousedown.dismiss.bs.modal", (t => {
-                P.one(this._element, "click.dismiss.bs.modal", (e => {
+            })), N.on(this._element, bn, (t => {
+                N.one(this._element, _n, (e => {
                     this._element === t.target && this._element === e.target && ("static" !== this._config.backdrop ? this._config.backdrop && this.hide() : this._triggerBackdropTransition())
                 }))
             }))
         }
         _hideModal() {
             this._element.style.display = "none", this._element.setAttribute("aria-hidden", !0), this._element.removeAttribute("aria-modal"), this._element.removeAttribute("role"), this._isTransitioning = !1, this._backdrop.hide((() => {
-                document.body.classList.remove(ki), this._resetAdjustments(), this._scrollBar.reset(), P.trigger(this._element, Oi)
+                document.body.classList.remove(wn), this._resetAdjustments(), this._scrollBar.reset(), N.trigger(this._element, fn)
             }))
         }
         _isAnimated() {
             return this._element.classList.contains("fade")
         }
         _triggerBackdropTransition() {
-            if (P.trigger(this._element, "hidePrevented.bs.modal").defaultPrevented) return;
+            if (N.trigger(this._element, un).defaultPrevented) return;
             const t = this._element.scrollHeight > document.documentElement.clientHeight,
                 e = this._element.style.overflowY;
-            "hidden" === e || this._element.classList.contains(Di) || (t || (this._element.style.overflowY = "hidden"), this._element.classList.add(Di), this._queueCallback((() => {
-                this._element.classList.remove(Di), this._queueCallback((() => {
+            "hidden" === e || this._element.classList.contains(En) || (t || (this._element.style.overflowY = "hidden"), this._element.classList.add(En), this._queueCallback((() => {
+                this._element.classList.remove(En), this._queueCallback((() => {
                     this._element.style.overflowY = e
                 }), this._dialog)
             }), this._dialog), this._element.focus())
         }
         _adjustDialog() {
             const t = this._element.scrollHeight > document.documentElement.clientHeight,
                 e = this._scrollBar.getWidth(),
@@ -2373,134 +2412,136 @@
             }
         }
         _resetAdjustments() {
             this._element.style.paddingLeft = "", this._element.style.paddingRight = ""
         }
         static jQueryInterface(t, e) {
             return this.each((function() {
-                const i = Ni.getOrCreateInstance(this, t);
+                const i = On.getOrCreateInstance(this, t);
                 if ("string" == typeof t) {
                     if (void 0 === i[t]) throw new TypeError(`No method named "${t}"`);
                     i[t](e)
                 }
             }))
         }
     }
-    P.on(document, "click.bs.modal.data-api", '[data-bs-toggle="modal"]', (function(t) {
-        const e = n(this);
-        ["A", "AREA"].includes(this.tagName) && t.preventDefault(), P.one(e, xi, (t => {
-            t.defaultPrevented || P.one(e, Oi, (() => {
+    N.on(document, yn, '[data-bs-toggle="modal"]', (function(t) {
+        const e = z.getElementFromSelector(this);
+        ["A", "AREA"].includes(this.tagName) && t.preventDefault(), N.one(e, pn, (t => {
+            t.defaultPrevented || N.one(e, fn, (() => {
                 a(this) && this.focus()
             }))
         }));
-        const i = Q.findOne(".modal.show");
-        i && Ni.getInstance(i).hide(), Ni.getOrCreateInstance(e).toggle(this)
-    })), q(Ni), g(Ni);
-    const Pi = "show",
-        ji = "showing",
-        Mi = "hiding",
-        Hi = ".offcanvas.show",
-        $i = "hidePrevented.bs.offcanvas",
-        Wi = "hidden.bs.offcanvas",
-        Bi = {
+        const i = z.findOne(".modal.show");
+        i && On.getInstance(i).hide(), On.getOrCreateInstance(e).toggle(this)
+    })), R(On), m(On);
+    const xn = ".bs.offcanvas",
+        kn = ".data-api",
+        Ln = `load${xn}${kn}`,
+        Sn = "show",
+        Dn = "showing",
+        $n = "hiding",
+        In = ".offcanvas.show",
+        Nn = `show${xn}`,
+        Pn = `shown${xn}`,
+        Mn = `hide${xn}`,
+        jn = `hidePrevented${xn}`,
+        Fn = `hidden${xn}`,
+        Hn = `resize${xn}`,
+        Wn = `click${xn}${kn}`,
+        Bn = `keydown.dismiss${xn}`,
+        zn = {
             backdrop: !0,
             keyboard: !0,
             scroll: !1
         },
-        Fi = {
+        Rn = {
             backdrop: "(boolean|string)",
             keyboard: "boolean",
             scroll: "boolean"
         };
-    class zi extends z {
+    class qn extends W {
         constructor(t, e) {
             super(t, e), this._isShown = !1, this._backdrop = this._initializeBackDrop(), this._focustrap = this._initializeFocusTrap(), this._addEventListeners()
         }
         static get Default() {
-            return Bi
+            return zn
         }
         static get DefaultType() {
-            return Fi
+            return Rn
         }
         static get NAME() {
             return "offcanvas"
         }
         toggle(t) {
             return this._isShown ? this.hide() : this.show(t)
         }
         show(t) {
-            this._isShown || P.trigger(this._element, "show.bs.offcanvas", {
+            this._isShown || N.trigger(this._element, Nn, {
                 relatedTarget: t
-            }).defaultPrevented || (this._isShown = !0, this._backdrop.show(), this._config.scroll || (new gi).hide(), this._element.setAttribute("aria-modal", !0), this._element.setAttribute("role", "dialog"), this._element.classList.add(ji), this._queueCallback((() => {
-                this._config.scroll && !this._config.backdrop || this._focustrap.activate(), this._element.classList.add(Pi), this._element.classList.remove(ji), P.trigger(this._element, "shown.bs.offcanvas", {
+            }).defaultPrevented || (this._isShown = !0, this._backdrop.show(), this._config.scroll || (new cn).hide(), this._element.setAttribute("aria-modal", !0), this._element.setAttribute("role", "dialog"), this._element.classList.add(Dn), this._queueCallback((() => {
+                this._config.scroll && !this._config.backdrop || this._focustrap.activate(), this._element.classList.add(Sn), this._element.classList.remove(Dn), N.trigger(this._element, Pn, {
                     relatedTarget: t
                 })
             }), this._element, !0))
         }
         hide() {
-            this._isShown && (P.trigger(this._element, "hide.bs.offcanvas").defaultPrevented || (this._focustrap.deactivate(), this._element.blur(), this._isShown = !1, this._element.classList.add(Mi), this._backdrop.hide(), this._queueCallback((() => {
-                this._element.classList.remove(Pi, Mi), this._element.removeAttribute("aria-modal"), this._element.removeAttribute("role"), this._config.scroll || (new gi).reset(), P.trigger(this._element, Wi)
+            this._isShown && (N.trigger(this._element, Mn).defaultPrevented || (this._focustrap.deactivate(), this._element.blur(), this._isShown = !1, this._element.classList.add($n), this._backdrop.hide(), this._queueCallback((() => {
+                this._element.classList.remove(Sn, $n), this._element.removeAttribute("aria-modal"), this._element.removeAttribute("role"), this._config.scroll || (new cn).reset(), N.trigger(this._element, Fn)
             }), this._element, !0)))
         }
         dispose() {
             this._backdrop.dispose(), this._focustrap.deactivate(), super.dispose()
         }
         _initializeBackDrop() {
             const t = Boolean(this._config.backdrop);
-            return new yi({
+            return new Ui({
                 className: "offcanvas-backdrop",
                 isVisible: t,
                 isAnimated: !0,
                 rootElement: this._element.parentNode,
                 clickCallback: t ? () => {
-                    "static" !== this._config.backdrop ? this.hide() : P.trigger(this._element, $i)
+                    "static" !== this._config.backdrop ? this.hide() : N.trigger(this._element, jn)
                 } : null
             })
         }
         _initializeFocusTrap() {
-            return new Ci({
+            return new sn({
                 trapElement: this._element
             })
         }
         _addEventListeners() {
-            P.on(this._element, "keydown.dismiss.bs.offcanvas", (t => {
-                "Escape" === t.key && (this._config.keyboard ? this.hide() : P.trigger(this._element, $i))
+            N.on(this._element, Bn, (t => {
+                "Escape" === t.key && (this._config.keyboard ? this.hide() : N.trigger(this._element, jn))
             }))
         }
         static jQueryInterface(t) {
             return this.each((function() {
-                const e = zi.getOrCreateInstance(this, t);
+                const e = qn.getOrCreateInstance(this, t);
                 if ("string" == typeof t) {
                     if (void 0 === e[t] || t.startsWith("_") || "constructor" === t) throw new TypeError(`No method named "${t}"`);
                     e[t](this)
                 }
             }))
         }
     }
-    P.on(document, "click.bs.offcanvas.data-api", '[data-bs-toggle="offcanvas"]', (function(t) {
-        const e = n(this);
+    N.on(document, Wn, '[data-bs-toggle="offcanvas"]', (function(t) {
+        const e = z.getElementFromSelector(this);
         if (["A", "AREA"].includes(this.tagName) && t.preventDefault(), l(this)) return;
-        P.one(e, Wi, (() => {
+        N.one(e, Fn, (() => {
             a(this) && this.focus()
         }));
-        const i = Q.findOne(Hi);
-        i && i !== e && zi.getInstance(i).hide(), zi.getOrCreateInstance(e).toggle(this)
-    })), P.on(window, "load.bs.offcanvas.data-api", (() => {
-        for (const t of Q.find(Hi)) zi.getOrCreateInstance(t).show()
-    })), P.on(window, "resize.bs.offcanvas", (() => {
-        for (const t of Q.find("[aria-modal][class*=show][class*=offcanvas-]")) "fixed" !== getComputedStyle(t).position && zi.getOrCreateInstance(t).hide()
-    })), q(zi), g(zi);
-    const qi = new Set(["background", "cite", "href", "itemtype", "longdesc", "poster", "src", "xlink:href"]),
-        Ri = /^(?:(?:https?|mailto|ftp|tel|file|sms):|[^#&/:?]*(?:[#/?]|$))/i,
-        Vi = /^data:(?:image\/(?:bmp|gif|jpeg|jpg|png|tiff|webp)|video\/(?:mpeg|mp4|ogg|webm)|audio\/(?:mp3|oga|ogg|opus));base64,[\d+/a-z]+=*$/i,
-        Ki = (t, e) => {
-            const i = t.nodeName.toLowerCase();
-            return e.includes(i) ? !qi.has(i) || Boolean(Ri.test(t.nodeValue) || Vi.test(t.nodeValue)) : e.filter((t => t instanceof RegExp)).some((t => t.test(i)))
-        },
-        Qi = {
+        const i = z.findOne(In);
+        i && i !== e && qn.getInstance(i).hide(), qn.getOrCreateInstance(e).toggle(this)
+    })), N.on(window, Ln, (() => {
+        for (const t of z.find(In)) qn.getOrCreateInstance(t).show()
+    })), N.on(window, Hn, (() => {
+        for (const t of z.find("[aria-modal][class*=show][class*=offcanvas-]")) "fixed" !== getComputedStyle(t).position && qn.getOrCreateInstance(t).hide()
+    })), R(qn), m(qn);
+    const Vn = {
             "*": ["class", "dir", "id", "lang", "role", /^aria-[\w-]*$/i],
             a: ["target", "href", "title", "rel"],
             area: [],
             b: [],
             br: [],
             col: [],
             code: [],
@@ -2524,45 +2565,51 @@
             span: [],
             sub: [],
             sup: [],
             strong: [],
             u: [],
             ul: []
         },
-        Xi = {
-            allowList: Qi,
+        Kn = new Set(["background", "cite", "href", "itemtype", "longdesc", "poster", "src", "xlink:href"]),
+        Qn = /^(?!javascript:)(?:[a-z0-9+.-]+:|[^&:/?#]*(?:[/?#]|$))/i,
+        Xn = (t, e) => {
+            const i = t.nodeName.toLowerCase();
+            return e.includes(i) ? !Kn.has(i) || Boolean(Qn.test(t.nodeValue)) : e.filter((t => t instanceof RegExp)).some((t => t.test(i)))
+        },
+        Yn = {
+            allowList: Vn,
             content: {},
             extraClass: "",
             html: !1,
             sanitize: !0,
             sanitizeFn: null,
             template: "<div></div>"
         },
-        Yi = {
+        Un = {
             allowList: "object",
             content: "object",
             extraClass: "(string|function)",
             html: "boolean",
             sanitize: "boolean",
             sanitizeFn: "(null|function)",
             template: "string"
         },
-        Ui = {
+        Gn = {
             entry: "(string|element|function|null)",
             selector: "(string|element)"
         };
-    class Gi extends F {
+    class Jn extends H {
         constructor(t) {
             super(), this._config = this._getConfig(t)
         }
         static get Default() {
-            return Xi
+            return Yn
         }
         static get DefaultType() {
-            return Yi
+            return Un
         }
         static get NAME() {
             return "TemplateFactory"
         }
         getContent() {
             return Object.values(this._config.content).map((t => this._resolvePossibleFunction(t))).filter(Boolean)
         }
@@ -2586,18 +2633,18 @@
         _typeCheckConfig(t) {
             super._typeCheckConfig(t), this._checkContent(t.content)
         }
         _checkContent(t) {
             for (const [e, i] of Object.entries(t)) super._typeCheckConfig({
                 selector: e,
                 entry: i
-            }, Ui)
+            }, Gn)
         }
         _setContent(t, e, i) {
-            const n = Q.findOne(i, t);
+            const n = z.findOne(i, t);
             n && ((e = this._resolvePossibleFunction(e)) ? o(e) ? this._putElementInTemplate(r(e), n) : this._config.html ? n.innerHTML = this._maybeSanitize(e) : n.textContent = e : n.remove())
         }
         _maybeSanitize(t) {
             return this._config.sanitize ? function(t, e, i) {
                 if (!t.length) return t;
                 if (i && "function" == typeof i) return i(t);
                 const n = (new window.DOMParser).parseFromString(t, "text/html"),
@@ -2606,61 +2653,61 @@
                     const i = t.nodeName.toLowerCase();
                     if (!Object.keys(e).includes(i)) {
                         t.remove();
                         continue
                     }
                     const n = [].concat(...t.attributes),
                         s = [].concat(e["*"] || [], e[i] || []);
-                    for (const e of n) Ki(e, s) || t.removeAttribute(e.nodeName)
+                    for (const e of n) Xn(e, s) || t.removeAttribute(e.nodeName)
                 }
                 return n.body.innerHTML
             }(t, this._config.allowList, this._config.sanitizeFn) : t
         }
         _resolvePossibleFunction(t) {
-            return "function" == typeof t ? t(this) : t
+            return g(t, [this])
         }
         _putElementInTemplate(t, e) {
             if (this._config.html) return e.innerHTML = "", void e.append(t);
             e.textContent = t.textContent
         }
     }
-    const Ji = new Set(["sanitize", "allowList", "sanitizeFn"]),
-        Zi = "fade",
-        tn = "show",
-        en = ".modal",
-        nn = "hide.bs.modal",
-        sn = "hover",
-        on = "focus",
-        rn = {
+    const Zn = new Set(["sanitize", "allowList", "sanitizeFn"]),
+        ts = "fade",
+        es = "show",
+        is = ".modal",
+        ns = "hide.bs.modal",
+        ss = "hover",
+        os = "focus",
+        rs = {
             AUTO: "auto",
             TOP: "top",
             RIGHT: p() ? "left" : "right",
             BOTTOM: "bottom",
             LEFT: p() ? "right" : "left"
         },
-        an = {
-            allowList: Qi,
+        as = {
+            allowList: Vn,
             animation: !0,
             boundary: "clippingParents",
             container: !1,
             customClass: "",
             delay: 0,
             fallbackPlacements: ["top", "right", "bottom", "left"],
             html: !1,
-            offset: [0, 0],
+            offset: [0, 6],
             placement: "top",
             popperConfig: null,
             sanitize: !0,
             sanitizeFn: null,
             selector: !1,
             template: '<div class="tooltip" role="tooltip"><div class="tooltip-arrow"></div><div class="tooltip-inner"></div></div>',
             title: "",
             trigger: "hover focus"
         },
-        ln = {
+        ls = {
             allowList: "object",
             animation: "boolean",
             boundary: "(string|element)",
             container: "(string|element|boolean)",
             customClass: "(string|function)",
             delay: "(number|object)",
             fallbackPlacements: "array",
@@ -2671,24 +2718,24 @@
             sanitize: "boolean",
             sanitizeFn: "(null|function)",
             selector: "(string|boolean)",
             template: "string",
             title: "(string|element|function)",
             trigger: "string"
         };
-    class cn extends z {
+    class cs extends W {
         constructor(t, e) {
-            if (void 0 === Ke) throw new TypeError("Bootstrap's tooltips require Popper (https://popper.js.org)");
+            if (void 0 === vi) throw new TypeError("Bootstrap's tooltips require Popper (https://popper.js.org)");
             super(t, e), this._isEnabled = !0, this._timeout = 0, this._isHovered = null, this._activeTrigger = {}, this._popper = null, this._templateFactory = null, this._newContent = null, this.tip = null, this._setListeners(), this._config.selector || this._fixTitle()
         }
         static get Default() {
-            return an
+            return as
         }
         static get DefaultType() {
-            return ln
+            return ls
         }
         static get NAME() {
             return "tooltip"
         }
         enable() {
             this._isEnabled = !0
         }
@@ -2698,40 +2745,40 @@
         toggleEnabled() {
             this._isEnabled = !this._isEnabled
         }
         toggle() {
             this._isEnabled && (this._activeTrigger.click = !this._activeTrigger.click, this._isShown() ? this._leave() : this._enter())
         }
         dispose() {
-            clearTimeout(this._timeout), P.off(this._element.closest(en), nn, this._hideModalHandler), this._element.getAttribute("data-bs-original-title") && this._element.setAttribute("title", this._element.getAttribute("data-bs-original-title")), this._disposePopper(), super.dispose()
+            clearTimeout(this._timeout), N.off(this._element.closest(is), ns, this._hideModalHandler), this._element.getAttribute("data-bs-original-title") && this._element.setAttribute("title", this._element.getAttribute("data-bs-original-title")), this._disposePopper(), super.dispose()
         }
         show() {
             if ("none" === this._element.style.display) throw new Error("Please use show on visible elements");
             if (!this._isWithContent() || !this._isEnabled) return;
-            const t = P.trigger(this._element, this.constructor.eventName("show")),
+            const t = N.trigger(this._element, this.constructor.eventName("show")),
                 e = (c(this._element) || this._element.ownerDocument.documentElement).contains(this._element);
             if (t.defaultPrevented || !e) return;
             this._disposePopper();
             const i = this._getTipElement();
             this._element.setAttribute("aria-describedby", i.getAttribute("id"));
             const {
                 container: n
             } = this._config;
-            if (this._element.ownerDocument.documentElement.contains(this.tip) || (n.append(i), P.trigger(this._element, this.constructor.eventName("inserted"))), this._popper = this._createPopper(i), i.classList.add(tn), "ontouchstart" in document.documentElement)
-                for (const t of [].concat(...document.body.children)) P.on(t, "mouseover", h);
+            if (this._element.ownerDocument.documentElement.contains(this.tip) || (n.append(i), N.trigger(this._element, this.constructor.eventName("inserted"))), this._popper = this._createPopper(i), i.classList.add(es), "ontouchstart" in document.documentElement)
+                for (const t of [].concat(...document.body.children)) N.on(t, "mouseover", h);
             this._queueCallback((() => {
-                P.trigger(this._element, this.constructor.eventName("shown")), !1 === this._isHovered && this._leave(), this._isHovered = !1
+                N.trigger(this._element, this.constructor.eventName("shown")), !1 === this._isHovered && this._leave(), this._isHovered = !1
             }), this.tip, this._isAnimated())
         }
         hide() {
-            if (this._isShown() && !P.trigger(this._element, this.constructor.eventName("hide")).defaultPrevented) {
-                if (this._getTipElement().classList.remove(tn), "ontouchstart" in document.documentElement)
-                    for (const t of [].concat(...document.body.children)) P.off(t, "mouseover", h);
-                this._activeTrigger.click = !1, this._activeTrigger.focus = !1, this._activeTrigger.hover = !1, this._isHovered = null, this._queueCallback((() => {
-                    this._isWithActiveTrigger() || (this._isHovered || this._disposePopper(), this._element.removeAttribute("aria-describedby"), P.trigger(this._element, this.constructor.eventName("hidden")))
+            if (this._isShown() && !N.trigger(this._element, this.constructor.eventName("hide")).defaultPrevented) {
+                if (this._getTipElement().classList.remove(es), "ontouchstart" in document.documentElement)
+                    for (const t of [].concat(...document.body.children)) N.off(t, "mouseover", h);
+                this._activeTrigger.click = !1, this._activeTrigger[os] = !1, this._activeTrigger[ss] = !1, this._isHovered = null, this._queueCallback((() => {
+                    this._isWithActiveTrigger() || (this._isHovered || this._disposePopper(), this._element.removeAttribute("aria-describedby"), N.trigger(this._element, this.constructor.eventName("hidden")))
                 }), this.tip, this._isAnimated())
             }
         }
         update() {
             this._popper && this._popper.update()
         }
         _isWithContent() {
@@ -2739,28 +2786,28 @@
         }
         _getTipElement() {
             return this.tip || (this.tip = this._createTipElement(this._newContent || this._getContentForTemplate())), this.tip
         }
         _createTipElement(t) {
             const e = this._getTemplateFactory(t).toHtml();
             if (!e) return null;
-            e.classList.remove(Zi, tn), e.classList.add(`bs-${this.constructor.NAME}-auto`);
+            e.classList.remove(ts, es), e.classList.add(`bs-${this.constructor.NAME}-auto`);
             const i = (t => {
                 do {
                     t += Math.floor(1e6 * Math.random())
                 } while (document.getElementById(t));
                 return t
             })(this.constructor.NAME).toString();
-            return e.setAttribute("id", i), this._isAnimated() && e.classList.add(Zi), e
+            return e.setAttribute("id", i), this._isAnimated() && e.classList.add(ts), e
         }
         setContent(t) {
             this._newContent = t, this._isShown() && (this._disposePopper(), this.show())
         }
         _getTemplateFactory(t) {
-            return this._templateFactory ? this._templateFactory.changeContent(t) : this._templateFactory = new Gi({
+            return this._templateFactory ? this._templateFactory.changeContent(t) : this._templateFactory = new Jn({
                 ...this._config,
                 content: t,
                 extraClass: this._resolvePossibleFunction(this._config.customClass)
             }), this._templateFactory
         }
         _getContentForTemplate() {
             return {
@@ -2770,32 +2817,32 @@
         _getTitle() {
             return this._resolvePossibleFunction(this._config.title) || this._element.getAttribute("data-bs-original-title")
         }
         _initializeOnDelegatedTarget(t) {
             return this.constructor.getOrCreateInstance(t.delegateTarget, this._getDelegateConfig())
         }
         _isAnimated() {
-            return this._config.animation || this.tip && this.tip.classList.contains(Zi)
+            return this._config.animation || this.tip && this.tip.classList.contains(ts)
         }
         _isShown() {
-            return this.tip && this.tip.classList.contains(tn)
+            return this.tip && this.tip.classList.contains(es)
         }
         _createPopper(t) {
-            const e = "function" == typeof this._config.placement ? this._config.placement.call(this, t, this._element) : this._config.placement,
-                i = rn[e.toUpperCase()];
-            return Ve(this._element, t, this._getPopperConfig(i))
+            const e = g(this._config.placement, [this, t, this._element]),
+                i = rs[e.toUpperCase()];
+            return bi(this._element, t, this._getPopperConfig(i))
         }
         _getOffset() {
             const {
                 offset: t
             } = this._config;
             return "string" == typeof t ? t.split(",").map((t => Number.parseInt(t, 10))) : "function" == typeof t ? e => t(e, this._element) : t
         }
         _resolvePossibleFunction(t) {
-            return "function" == typeof t ? t.call(this._element) : t
+            return g(t, [this._element])
         }
         _getPopperConfig(t) {
             const e = {
                 placement: t,
                 modifiers: [{
                     name: "flip",
                     options: {
@@ -2823,37 +2870,37 @@
                     fn: t => {
                         this._getTipElement().setAttribute("data-popper-placement", t.state.placement)
                     }
                 }]
             };
             return {
                 ...e,
-                ..."function" == typeof this._config.popperConfig ? this._config.popperConfig(e) : this._config.popperConfig
+                ...g(this._config.popperConfig, [e])
             }
         }
         _setListeners() {
             const t = this._config.trigger.split(" ");
             for (const e of t)
-                if ("click" === e) P.on(this._element, this.constructor.eventName("click"), this._config.selector, (t => {
+                if ("click" === e) N.on(this._element, this.constructor.eventName("click"), this._config.selector, (t => {
                     this._initializeOnDelegatedTarget(t).toggle()
                 }));
                 else if ("manual" !== e) {
-                const t = e === sn ? this.constructor.eventName("mouseenter") : this.constructor.eventName("focusin"),
-                    i = e === sn ? this.constructor.eventName("mouseleave") : this.constructor.eventName("focusout");
-                P.on(this._element, t, this._config.selector, (t => {
+                const t = e === ss ? this.constructor.eventName("mouseenter") : this.constructor.eventName("focusin"),
+                    i = e === ss ? this.constructor.eventName("mouseleave") : this.constructor.eventName("focusout");
+                N.on(this._element, t, this._config.selector, (t => {
                     const e = this._initializeOnDelegatedTarget(t);
-                    e._activeTrigger["focusin" === t.type ? on : sn] = !0, e._enter()
-                })), P.on(this._element, i, this._config.selector, (t => {
+                    e._activeTrigger["focusin" === t.type ? os : ss] = !0, e._enter()
+                })), N.on(this._element, i, this._config.selector, (t => {
                     const e = this._initializeOnDelegatedTarget(t);
-                    e._activeTrigger["focusout" === t.type ? on : sn] = e._element.contains(t.relatedTarget), e._leave()
+                    e._activeTrigger["focusout" === t.type ? os : ss] = e._element.contains(t.relatedTarget), e._leave()
                 }))
             }
             this._hideModalHandler = () => {
                 this._element && this.hide()
-            }, P.on(this._element.closest(en), nn, this._hideModalHandler)
+            }, N.on(this._element.closest(is), ns, this._hideModalHandler)
         }
         _fixTitle() {
             const t = this._element.getAttribute("title");
             t && (this._element.getAttribute("aria-label") || this._element.textContent.trim() || this._element.setAttribute("aria-label", t), this._element.setAttribute("data-bs-original-title", t), this._element.removeAttribute("title"))
         }
         _enter() {
             this._isShown() || this._isHovered ? this._isHovered = !0 : (this._isHovered = !0, this._setTimeout((() => {
@@ -2868,64 +2915,64 @@
         _setTimeout(t, e) {
             clearTimeout(this._timeout), this._timeout = setTimeout(t, e)
         }
         _isWithActiveTrigger() {
             return Object.values(this._activeTrigger).includes(!0)
         }
         _getConfig(t) {
-            const e = B.getDataAttributes(this._element);
-            for (const t of Object.keys(e)) Ji.has(t) && delete e[t];
+            const e = F.getDataAttributes(this._element);
+            for (const t of Object.keys(e)) Zn.has(t) && delete e[t];
             return t = {
                 ...e,
                 ..."object" == typeof t && t ? t : {}
             }, t = this._mergeConfigObj(t), t = this._configAfterMerge(t), this._typeCheckConfig(t), t
         }
         _configAfterMerge(t) {
             return t.container = !1 === t.container ? document.body : r(t.container), "number" == typeof t.delay && (t.delay = {
                 show: t.delay,
                 hide: t.delay
             }), "number" == typeof t.title && (t.title = t.title.toString()), "number" == typeof t.content && (t.content = t.content.toString()), t
         }
         _getDelegateConfig() {
             const t = {};
-            for (const e in this._config) this.constructor.Default[e] !== this._config[e] && (t[e] = this._config[e]);
+            for (const [e, i] of Object.entries(this._config)) this.constructor.Default[e] !== i && (t[e] = i);
             return t.selector = !1, t.trigger = "manual", t
         }
         _disposePopper() {
             this._popper && (this._popper.destroy(), this._popper = null), this.tip && (this.tip.remove(), this.tip = null)
         }
         static jQueryInterface(t) {
             return this.each((function() {
-                const e = cn.getOrCreateInstance(this, t);
+                const e = cs.getOrCreateInstance(this, t);
                 if ("string" == typeof t) {
                     if (void 0 === e[t]) throw new TypeError(`No method named "${t}"`);
                     e[t]()
                 }
             }))
         }
     }
-    g(cn);
-    const hn = {
-            ...cn.Default,
+    m(cs);
+    const hs = {
+            ...cs.Default,
             content: "",
             offset: [0, 8],
             placement: "right",
             template: '<div class="popover" role="tooltip"><div class="popover-arrow"></div><h3 class="popover-header"></h3><div class="popover-body"></div></div>',
             trigger: "click"
         },
-        dn = {
-            ...cn.DefaultType,
+        ds = {
+            ...cs.DefaultType,
             content: "(null|string|element|function)"
         };
-    class un extends cn {
+    class us extends cs {
         static get Default() {
-            return hn
+            return hs
         }
         static get DefaultType() {
-            return dn
+            return ds
         }
         static get NAME() {
             return "popover"
         }
         _isWithContent() {
             return this._getTitle() || this._getContent()
         }
@@ -2936,52 +2983,57 @@
             }
         }
         _getContent() {
             return this._resolvePossibleFunction(this._config.content)
         }
         static jQueryInterface(t) {
             return this.each((function() {
-                const e = un.getOrCreateInstance(this, t);
+                const e = us.getOrCreateInstance(this, t);
                 if ("string" == typeof t) {
                     if (void 0 === e[t]) throw new TypeError(`No method named "${t}"`);
                     e[t]()
                 }
             }))
         }
     }
-    g(un);
-    const fn = "click.bs.scrollspy",
-        pn = "active",
-        gn = "[href]",
-        mn = {
+    m(us);
+    const fs = ".bs.scrollspy",
+        ps = `activate${fs}`,
+        ms = `click${fs}`,
+        gs = `load${fs}.data-api`,
+        _s = "active",
+        bs = "[href]",
+        vs = ".nav-link",
+        ys = `${vs}, .nav-item > ${vs}, .list-group-item`,
+        ws = {
             offset: null,
             rootMargin: "0px 0px -25%",
             smoothScroll: !1,
             target: null,
             threshold: [.1, .5, 1]
         },
-        _n = {
+        As = {
             offset: "(number|null)",
             rootMargin: "string",
             smoothScroll: "boolean",
             target: "element",
             threshold: "array"
         };
-    class bn extends z {
+    class Es extends W {
         constructor(t, e) {
             super(t, e), this._targetLinks = new Map, this._observableSections = new Map, this._rootElement = "visible" === getComputedStyle(this._element).overflowY ? null : this._element, this._activeTarget = null, this._observer = null, this._previousScrollData = {
                 visibleEntryTop: 0,
                 parentScrollTop: 0
             }, this.refresh()
         }
         static get Default() {
-            return mn
+            return ws
         }
         static get DefaultType() {
-            return _n
+            return As
         }
         static get NAME() {
             return "scrollspy"
         }
         refresh() {
             this._initializeTargetsAndObservables(), this._maybeEnableSmoothScroll(), this._observer ? this._observer.disconnect() : this._observer = this._getNewObserver();
             for (const t of this._observableSections.values()) this._observer.observe(t)
@@ -2989,15 +3041,15 @@
         dispose() {
             this._observer.disconnect(), super.dispose()
         }
         _configAfterMerge(t) {
             return t.target = r(t.target) || document.body, t.rootMargin = t.offset ? `${t.offset}px 0px -30%` : t.rootMargin, "string" == typeof t.threshold && (t.threshold = t.threshold.split(",").map((t => Number.parseFloat(t)))), t
         }
         _maybeEnableSmoothScroll() {
-            this._config.smoothScroll && (P.off(this._config.target, fn), P.on(this._config.target, fn, gn, (t => {
+            this._config.smoothScroll && (N.off(this._config.target, ms), N.on(this._config.target, ms, bs, (t => {
                 const e = this._observableSections.get(t.target.hash);
                 if (e) {
                     t.preventDefault();
                     const i = this._rootElement || window,
                         n = e.offsetTop - this._element.offsetTop;
                     if (i.scrollTo) return void i.scrollTo({
                         top: n,
@@ -3032,102 +3084,119 @@
                 if (s && t) {
                     if (i(o), !n) return
                 } else s || t || i(o)
             }
         }
         _initializeTargetsAndObservables() {
             this._targetLinks = new Map, this._observableSections = new Map;
-            const t = Q.find(gn, this._config.target);
+            const t = z.find(bs, this._config.target);
             for (const e of t) {
                 if (!e.hash || l(e)) continue;
-                const t = Q.findOne(e.hash, this._element);
-                a(t) && (this._targetLinks.set(e.hash, e), this._observableSections.set(e.hash, t))
+                const t = z.findOne(decodeURI(e.hash), this._element);
+                a(t) && (this._targetLinks.set(decodeURI(e.hash), e), this._observableSections.set(e.hash, t))
             }
         }
         _process(t) {
-            this._activeTarget !== t && (this._clearActiveClass(this._config.target), this._activeTarget = t, t.classList.add(pn), this._activateParents(t), P.trigger(this._element, "activate.bs.scrollspy", {
+            this._activeTarget !== t && (this._clearActiveClass(this._config.target), this._activeTarget = t, t.classList.add(_s), this._activateParents(t), N.trigger(this._element, ps, {
                 relatedTarget: t
             }))
         }
         _activateParents(t) {
-            if (t.classList.contains("dropdown-item")) Q.findOne(".dropdown-toggle", t.closest(".dropdown")).classList.add(pn);
+            if (t.classList.contains("dropdown-item")) z.findOne(".dropdown-toggle", t.closest(".dropdown")).classList.add(_s);
             else
-                for (const e of Q.parents(t, ".nav, .list-group"))
-                    for (const t of Q.prev(e, ".nav-link, .nav-item > .nav-link, .list-group-item")) t.classList.add(pn)
+                for (const e of z.parents(t, ".nav, .list-group"))
+                    for (const t of z.prev(e, ys)) t.classList.add(_s)
         }
         _clearActiveClass(t) {
-            t.classList.remove(pn);
-            const e = Q.find("[href].active", t);
-            for (const t of e) t.classList.remove(pn)
+            t.classList.remove(_s);
+            const e = z.find(`${bs}.${_s}`, t);
+            for (const t of e) t.classList.remove(_s)
         }
         static jQueryInterface(t) {
             return this.each((function() {
-                const e = bn.getOrCreateInstance(this, t);
+                const e = Es.getOrCreateInstance(this, t);
                 if ("string" == typeof t) {
                     if (void 0 === e[t] || t.startsWith("_") || "constructor" === t) throw new TypeError(`No method named "${t}"`);
                     e[t]()
                 }
             }))
         }
     }
-    P.on(window, "load.bs.scrollspy.data-api", (() => {
-        for (const t of Q.find('[data-bs-spy="scroll"]')) bn.getOrCreateInstance(t)
-    })), g(bn);
-    const vn = "ArrowLeft",
-        yn = "ArrowRight",
-        wn = "ArrowUp",
-        An = "ArrowDown",
-        En = "active",
-        Tn = "fade",
-        Cn = "show",
-        On = '[data-bs-toggle="tab"], [data-bs-toggle="pill"], [data-bs-toggle="list"]',
-        xn = `.nav-link:not(.dropdown-toggle), .list-group-item:not(.dropdown-toggle), [role="tab"]:not(.dropdown-toggle), ${On}`;
-    class kn extends z {
+    N.on(window, gs, (() => {
+        for (const t of z.find('[data-bs-spy="scroll"]')) Es.getOrCreateInstance(t)
+    })), m(Es);
+    const Ts = ".bs.tab",
+        Cs = `hide${Ts}`,
+        Os = `hidden${Ts}`,
+        xs = `show${Ts}`,
+        ks = `shown${Ts}`,
+        Ls = `click${Ts}`,
+        Ss = `keydown${Ts}`,
+        Ds = `load${Ts}`,
+        $s = "ArrowLeft",
+        Is = "ArrowRight",
+        Ns = "ArrowUp",
+        Ps = "ArrowDown",
+        Ms = "Home",
+        js = "End",
+        Fs = "active",
+        Hs = "fade",
+        Ws = "show",
+        Bs = ":not(.dropdown-toggle)",
+        zs = '[data-bs-toggle="tab"], [data-bs-toggle="pill"], [data-bs-toggle="list"]',
+        Rs = `.nav-link${Bs}, .list-group-item${Bs}, [role="tab"]${Bs}, ${zs}`,
+        qs = `.${Fs}[data-bs-toggle="tab"], .${Fs}[data-bs-toggle="pill"], .${Fs}[data-bs-toggle="list"]`;
+    class Vs extends W {
         constructor(t) {
-            super(t), this._parent = this._element.closest('.list-group, .nav, [role="tablist"]'), this._parent && (this._setInitialAttributes(this._parent, this._getChildren()), P.on(this._element, "keydown.bs.tab", (t => this._keydown(t))))
+            super(t), this._parent = this._element.closest('.list-group, .nav, [role="tablist"]'), this._parent && (this._setInitialAttributes(this._parent, this._getChildren()), N.on(this._element, Ss, (t => this._keydown(t))))
         }
         static get NAME() {
             return "tab"
         }
         show() {
             const t = this._element;
             if (this._elemIsActive(t)) return;
             const e = this._getActiveElem(),
-                i = e ? P.trigger(e, "hide.bs.tab", {
+                i = e ? N.trigger(e, Cs, {
                     relatedTarget: t
                 }) : null;
-            P.trigger(t, "show.bs.tab", {
+            N.trigger(t, xs, {
                 relatedTarget: e
             }).defaultPrevented || i && i.defaultPrevented || (this._deactivate(e, t), this._activate(t, e))
         }
         _activate(t, e) {
-            t && (t.classList.add(En), this._activate(n(t)), this._queueCallback((() => {
-                "tab" === t.getAttribute("role") ? (t.removeAttribute("tabindex"), t.setAttribute("aria-selected", !0), this._toggleDropDown(t, !0), P.trigger(t, "shown.bs.tab", {
+            t && (t.classList.add(Fs), this._activate(z.getElementFromSelector(t)), this._queueCallback((() => {
+                "tab" === t.getAttribute("role") ? (t.removeAttribute("tabindex"), t.setAttribute("aria-selected", !0), this._toggleDropDown(t, !0), N.trigger(t, ks, {
                     relatedTarget: e
-                })) : t.classList.add(Cn)
-            }), t, t.classList.contains(Tn)))
+                })) : t.classList.add(Ws)
+            }), t, t.classList.contains(Hs)))
         }
         _deactivate(t, e) {
-            t && (t.classList.remove(En), t.blur(), this._deactivate(n(t)), this._queueCallback((() => {
-                "tab" === t.getAttribute("role") ? (t.setAttribute("aria-selected", !1), t.setAttribute("tabindex", "-1"), this._toggleDropDown(t, !1), P.trigger(t, "hidden.bs.tab", {
+            t && (t.classList.remove(Fs), t.blur(), this._deactivate(z.getElementFromSelector(t)), this._queueCallback((() => {
+                "tab" === t.getAttribute("role") ? (t.setAttribute("aria-selected", !1), t.setAttribute("tabindex", "-1"), this._toggleDropDown(t, !1), N.trigger(t, Os, {
                     relatedTarget: e
-                })) : t.classList.remove(Cn)
-            }), t, t.classList.contains(Tn)))
+                })) : t.classList.remove(Ws)
+            }), t, t.classList.contains(Hs)))
         }
         _keydown(t) {
-            if (![vn, yn, wn, An].includes(t.key)) return;
+            if (![$s, Is, Ns, Ps, Ms, js].includes(t.key)) return;
             t.stopPropagation(), t.preventDefault();
-            const e = [yn, An].includes(t.key),
-                i = b(this._getChildren().filter((t => !l(t))), t.target, e, !0);
+            const e = this._getChildren().filter((t => !l(t)));
+            let i;
+            if ([Ms, js].includes(t.key)) i = e[t.key === Ms ? 0 : e.length - 1];
+            else {
+                const n = [Is, Ps].includes(t.key);
+                i = b(e, t.target, n, !0)
+            }
             i && (i.focus({
                 preventScroll: !0
-            }), kn.getOrCreateInstance(i).show())
+            }), Vs.getOrCreateInstance(i).show())
         }
         _getChildren() {
-            return Q.find(xn, this._parent)
+            return z.find(Rs, this._parent)
         }
         _getActiveElem() {
             return this._getChildren().find((t => this._elemIsActive(t))) || null
         }
         _setInitialAttributes(t, e) {
             this._setAttributeIfNotExists(t, "role", "tablist");
             for (const t of e) this._setInitialAttributesOnChild(t)
@@ -3135,94 +3204,103 @@
         _setInitialAttributesOnChild(t) {
             t = this._getInnerElement(t);
             const e = this._elemIsActive(t),
                 i = this._getOuterElement(t);
             t.setAttribute("aria-selected", e), i !== t && this._setAttributeIfNotExists(i, "role", "presentation"), e || t.setAttribute("tabindex", "-1"), this._setAttributeIfNotExists(t, "role", "tab"), this._setInitialAttributesOnTargetPanel(t)
         }
         _setInitialAttributesOnTargetPanel(t) {
-            const e = n(t);
-            e && (this._setAttributeIfNotExists(e, "role", "tabpanel"), t.id && this._setAttributeIfNotExists(e, "aria-labelledby", `#${t.id}`))
+            const e = z.getElementFromSelector(t);
+            e && (this._setAttributeIfNotExists(e, "role", "tabpanel"), t.id && this._setAttributeIfNotExists(e, "aria-labelledby", `${t.id}`))
         }
         _toggleDropDown(t, e) {
             const i = this._getOuterElement(t);
             if (!i.classList.contains("dropdown")) return;
             const n = (t, n) => {
-                const s = Q.findOne(t, i);
+                const s = z.findOne(t, i);
                 s && s.classList.toggle(n, e)
             };
-            n(".dropdown-toggle", En), n(".dropdown-menu", Cn), i.setAttribute("aria-expanded", e)
+            n(".dropdown-toggle", Fs), n(".dropdown-menu", Ws), i.setAttribute("aria-expanded", e)
         }
         _setAttributeIfNotExists(t, e, i) {
             t.hasAttribute(e) || t.setAttribute(e, i)
         }
         _elemIsActive(t) {
-            return t.classList.contains(En)
+            return t.classList.contains(Fs)
         }
         _getInnerElement(t) {
-            return t.matches(xn) ? t : Q.findOne(xn, t)
+            return t.matches(Rs) ? t : z.findOne(Rs, t)
         }
         _getOuterElement(t) {
             return t.closest(".nav-item, .list-group-item") || t
         }
         static jQueryInterface(t) {
             return this.each((function() {
-                const e = kn.getOrCreateInstance(this);
+                const e = Vs.getOrCreateInstance(this);
                 if ("string" == typeof t) {
                     if (void 0 === e[t] || t.startsWith("_") || "constructor" === t) throw new TypeError(`No method named "${t}"`);
                     e[t]()
                 }
             }))
         }
     }
-    P.on(document, "click.bs.tab", On, (function(t) {
-        ["A", "AREA"].includes(this.tagName) && t.preventDefault(), l(this) || kn.getOrCreateInstance(this).show()
-    })), P.on(window, "load.bs.tab", (() => {
-        for (const t of Q.find('.active[data-bs-toggle="tab"], .active[data-bs-toggle="pill"], .active[data-bs-toggle="list"]')) kn.getOrCreateInstance(t)
-    })), g(kn);
-    const Ln = "hide",
-        Dn = "show",
-        Sn = "showing",
-        In = {
+    N.on(document, Ls, zs, (function(t) {
+        ["A", "AREA"].includes(this.tagName) && t.preventDefault(), l(this) || Vs.getOrCreateInstance(this).show()
+    })), N.on(window, Ds, (() => {
+        for (const t of z.find(qs)) Vs.getOrCreateInstance(t)
+    })), m(Vs);
+    const Ks = ".bs.toast",
+        Qs = `mouseover${Ks}`,
+        Xs = `mouseout${Ks}`,
+        Ys = `focusin${Ks}`,
+        Us = `focusout${Ks}`,
+        Gs = `hide${Ks}`,
+        Js = `hidden${Ks}`,
+        Zs = `show${Ks}`,
+        to = `shown${Ks}`,
+        eo = "hide",
+        io = "show",
+        no = "showing",
+        so = {
             animation: "boolean",
             autohide: "boolean",
             delay: "number"
         },
-        Nn = {
+        oo = {
             animation: !0,
             autohide: !0,
             delay: 5e3
         };
-    class Pn extends z {
+    class ro extends W {
         constructor(t, e) {
             super(t, e), this._timeout = null, this._hasMouseInteraction = !1, this._hasKeyboardInteraction = !1, this._setListeners()
         }
         static get Default() {
-            return Nn
+            return oo
         }
         static get DefaultType() {
-            return In
+            return so
         }
         static get NAME() {
             return "toast"
         }
         show() {
-            P.trigger(this._element, "show.bs.toast").defaultPrevented || (this._clearTimeout(), this._config.animation && this._element.classList.add("fade"), this._element.classList.remove(Ln), d(this._element), this._element.classList.add(Dn, Sn), this._queueCallback((() => {
-                this._element.classList.remove(Sn), P.trigger(this._element, "shown.bs.toast"), this._maybeScheduleHide()
+            N.trigger(this._element, Zs).defaultPrevented || (this._clearTimeout(), this._config.animation && this._element.classList.add("fade"), this._element.classList.remove(eo), d(this._element), this._element.classList.add(io, no), this._queueCallback((() => {
+                this._element.classList.remove(no), N.trigger(this._element, to), this._maybeScheduleHide()
             }), this._element, this._config.animation))
         }
         hide() {
-            this.isShown() && (P.trigger(this._element, "hide.bs.toast").defaultPrevented || (this._element.classList.add(Sn), this._queueCallback((() => {
-                this._element.classList.add(Ln), this._element.classList.remove(Sn, Dn), P.trigger(this._element, "hidden.bs.toast")
+            this.isShown() && (N.trigger(this._element, Gs).defaultPrevented || (this._element.classList.add(no), this._queueCallback((() => {
+                this._element.classList.add(eo), this._element.classList.remove(no, io), N.trigger(this._element, Js)
             }), this._element, this._config.animation)))
         }
         dispose() {
-            this._clearTimeout(), this.isShown() && this._element.classList.remove(Dn), super.dispose()
+            this._clearTimeout(), this.isShown() && this._element.classList.remove(io), super.dispose()
         }
         isShown() {
-            return this._element.classList.contains(Dn)
+            return this._element.classList.contains(io)
         }
         _maybeScheduleHide() {
             this._config.autohide && (this._hasMouseInteraction || this._hasKeyboardInteraction || (this._timeout = setTimeout((() => {
                 this.hide()
             }), this._config.delay)))
         }
         _onInteraction(t, e) {
@@ -3236,38 +3314,38 @@
                     this._hasKeyboardInteraction = e
             }
             if (e) return void this._clearTimeout();
             const i = t.relatedTarget;
             this._element === i || this._element.contains(i) || this._maybeScheduleHide()
         }
         _setListeners() {
-            P.on(this._element, "mouseover.bs.toast", (t => this._onInteraction(t, !0))), P.on(this._element, "mouseout.bs.toast", (t => this._onInteraction(t, !1))), P.on(this._element, "focusin.bs.toast", (t => this._onInteraction(t, !0))), P.on(this._element, "focusout.bs.toast", (t => this._onInteraction(t, !1)))
+            N.on(this._element, Qs, (t => this._onInteraction(t, !0))), N.on(this._element, Xs, (t => this._onInteraction(t, !1))), N.on(this._element, Ys, (t => this._onInteraction(t, !0))), N.on(this._element, Us, (t => this._onInteraction(t, !1)))
         }
         _clearTimeout() {
             clearTimeout(this._timeout), this._timeout = null
         }
         static jQueryInterface(t) {
             return this.each((function() {
-                const e = Pn.getOrCreateInstance(this, t);
+                const e = ro.getOrCreateInstance(this, t);
                 if ("string" == typeof t) {
                     if (void 0 === e[t]) throw new TypeError(`No method named "${t}"`);
                     e[t](this)
                 }
             }))
         }
     }
-    return q(Pn), g(Pn), {
-        Alert: R,
-        Button: K,
-        Carousel: at,
-        Collapse: pt,
-        Dropdown: hi,
-        Modal: Ni,
-        Offcanvas: zi,
-        Popover: un,
-        ScrollSpy: bn,
-        Tab: kn,
-        Toast: Pn,
-        Tooltip: cn
+    return R(ro), m(ro), {
+        Alert: Q,
+        Button: Y,
+        Carousel: xt,
+        Collapse: Bt,
+        Dropdown: qi,
+        Modal: On,
+        Offcanvas: qn,
+        Popover: us,
+        ScrollSpy: Es,
+        Tab: Vs,
+        Toast: ro,
+        Tooltip: cs
     }
 }));
 //# sourceMappingURL=bootstrap.bundle.min.js.map
```

### Comparing `fietsboek-0.8.0/fietsboek/static/bootstrap.css` & `fietsboek-0.9.0/fietsboek/static/bootstrap.css`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 @charset "UTF-8";
 /*!
- * Bootstrap  v5.2.3 (https://getbootstrap.com/)
- * Copyright 2011-2022 The Bootstrap Authors
- * Copyright 2011-2022 Twitter, Inc.
+ * Bootstrap  v5.3.1 (https://getbootstrap.com/)
+ * Copyright 2011-2023 The Bootstrap Authors
  * Licensed under MIT (https://github.com/twbs/bootstrap/blob/main/LICENSE)
  */
-:root {
+:root,
+[data-bs-theme=light] {
   --bs-blue: #0d6efd;
   --bs-indigo: #6610f2;
   --bs-purple: #6f42c1;
   --bs-pink: #d63384;
   --bs-red: #dc3545;
   --bs-orange: #fd7e14;
   --bs-yellow: #ffc107;
@@ -41,41 +41,145 @@
   --bs-secondary-rgb: 108, 117, 125;
   --bs-success-rgb: 25, 135, 84;
   --bs-info-rgb: 13, 202, 240;
   --bs-warning-rgb: 255, 193, 7;
   --bs-danger-rgb: 220, 53, 69;
   --bs-light-rgb: 248, 249, 250;
   --bs-dark-rgb: 33, 37, 41;
+  --bs-primary-text-emphasis: #052c65;
+  --bs-secondary-text-emphasis: #2b2f32;
+  --bs-success-text-emphasis: #0a3622;
+  --bs-info-text-emphasis: #055160;
+  --bs-warning-text-emphasis: #664d03;
+  --bs-danger-text-emphasis: #58151c;
+  --bs-light-text-emphasis: #495057;
+  --bs-dark-text-emphasis: #495057;
+  --bs-primary-bg-subtle: #cfe2ff;
+  --bs-secondary-bg-subtle: #e2e3e5;
+  --bs-success-bg-subtle: #d1e7dd;
+  --bs-info-bg-subtle: #cff4fc;
+  --bs-warning-bg-subtle: #fff3cd;
+  --bs-danger-bg-subtle: #f8d7da;
+  --bs-light-bg-subtle: #fcfcfd;
+  --bs-dark-bg-subtle: #ced4da;
+  --bs-primary-border-subtle: #9ec5fe;
+  --bs-secondary-border-subtle: #c4c8cb;
+  --bs-success-border-subtle: #a3cfbb;
+  --bs-info-border-subtle: #9eeaf9;
+  --bs-warning-border-subtle: #ffe69c;
+  --bs-danger-border-subtle: #f1aeb5;
+  --bs-light-border-subtle: #e9ecef;
+  --bs-dark-border-subtle: #adb5bd;
   --bs-white-rgb: 255, 255, 255;
   --bs-black-rgb: 0, 0, 0;
-  --bs-body-color-rgb: 33, 37, 41;
-  --bs-body-bg-rgb: 255, 255, 255;
   --bs-font-sans-serif: system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", "Noto Sans", "Liberation Sans", Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";
   --bs-font-monospace: SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;
   --bs-gradient: linear-gradient(180deg, rgba(255, 255, 255, 0.15), rgba(255, 255, 255, 0));
   --bs-body-font-family: var(--bs-font-sans-serif);
   --bs-body-font-size: 1rem;
   --bs-body-font-weight: 400;
   --bs-body-line-height: 1.5;
   --bs-body-color: #212529;
+  --bs-body-color-rgb: 33, 37, 41;
   --bs-body-bg: #fff;
+  --bs-body-bg-rgb: 255, 255, 255;
+  --bs-emphasis-color: #000;
+  --bs-emphasis-color-rgb: 0, 0, 0;
+  --bs-secondary-color: rgba(33, 37, 41, 0.75);
+  --bs-secondary-color-rgb: 33, 37, 41;
+  --bs-secondary-bg: #e9ecef;
+  --bs-secondary-bg-rgb: 233, 236, 239;
+  --bs-tertiary-color: rgba(33, 37, 41, 0.5);
+  --bs-tertiary-color-rgb: 33, 37, 41;
+  --bs-tertiary-bg: #f8f9fa;
+  --bs-tertiary-bg-rgb: 248, 249, 250;
+  --bs-heading-color: inherit;
+  --bs-link-color: #0d6efd;
+  --bs-link-color-rgb: 13, 110, 253;
+  --bs-link-decoration: underline;
+  --bs-link-hover-color: #0a58ca;
+  --bs-link-hover-color-rgb: 10, 88, 202;
+  --bs-code-color: #d63384;
+  --bs-highlight-bg: #fff3cd;
   --bs-border-width: 1px;
   --bs-border-style: solid;
   --bs-border-color: #dee2e6;
   --bs-border-color-translucent: rgba(0, 0, 0, 0.175);
   --bs-border-radius: 0.375rem;
   --bs-border-radius-sm: 0.25rem;
   --bs-border-radius-lg: 0.5rem;
   --bs-border-radius-xl: 1rem;
-  --bs-border-radius-2xl: 2rem;
+  --bs-border-radius-xxl: 2rem;
+  --bs-border-radius-2xl: var(--bs-border-radius-xxl);
   --bs-border-radius-pill: 50rem;
-  --bs-link-color: #0d6efd;
-  --bs-link-hover-color: #0a58ca;
-  --bs-code-color: #d63384;
-  --bs-highlight-bg: #fff3cd;
+  --bs-box-shadow: 0 0.5rem 1rem rgba(0, 0, 0, 0.15);
+  --bs-box-shadow-sm: 0 0.125rem 0.25rem rgba(0, 0, 0, 0.075);
+  --bs-box-shadow-lg: 0 1rem 3rem rgba(0, 0, 0, 0.175);
+  --bs-box-shadow-inset: inset 0 1px 2px rgba(0, 0, 0, 0.075);
+  --bs-focus-ring-width: 0.25rem;
+  --bs-focus-ring-opacity: 0.25;
+  --bs-focus-ring-color: rgba(13, 110, 253, 0.25);
+  --bs-form-valid-color: #198754;
+  --bs-form-valid-border-color: #198754;
+  --bs-form-invalid-color: #dc3545;
+  --bs-form-invalid-border-color: #dc3545;
+}
+
+[data-bs-theme=dark] {
+  color-scheme: dark;
+  --bs-body-color: #dee2e6;
+  --bs-body-color-rgb: 222, 226, 230;
+  --bs-body-bg: #212529;
+  --bs-body-bg-rgb: 33, 37, 41;
+  --bs-emphasis-color: #fff;
+  --bs-emphasis-color-rgb: 255, 255, 255;
+  --bs-secondary-color: rgba(222, 226, 230, 0.75);
+  --bs-secondary-color-rgb: 222, 226, 230;
+  --bs-secondary-bg: #343a40;
+  --bs-secondary-bg-rgb: 52, 58, 64;
+  --bs-tertiary-color: rgba(222, 226, 230, 0.5);
+  --bs-tertiary-color-rgb: 222, 226, 230;
+  --bs-tertiary-bg: #2b3035;
+  --bs-tertiary-bg-rgb: 43, 48, 53;
+  --bs-primary-text-emphasis: #6ea8fe;
+  --bs-secondary-text-emphasis: #a7acb1;
+  --bs-success-text-emphasis: #75b798;
+  --bs-info-text-emphasis: #6edff6;
+  --bs-warning-text-emphasis: #ffda6a;
+  --bs-danger-text-emphasis: #ea868f;
+  --bs-light-text-emphasis: #f8f9fa;
+  --bs-dark-text-emphasis: #dee2e6;
+  --bs-primary-bg-subtle: #031633;
+  --bs-secondary-bg-subtle: #161719;
+  --bs-success-bg-subtle: #051b11;
+  --bs-info-bg-subtle: #032830;
+  --bs-warning-bg-subtle: #332701;
+  --bs-danger-bg-subtle: #2c0b0e;
+  --bs-light-bg-subtle: #343a40;
+  --bs-dark-bg-subtle: #1a1d20;
+  --bs-primary-border-subtle: #084298;
+  --bs-secondary-border-subtle: #41464b;
+  --bs-success-border-subtle: #0f5132;
+  --bs-info-border-subtle: #087990;
+  --bs-warning-border-subtle: #997404;
+  --bs-danger-border-subtle: #842029;
+  --bs-light-border-subtle: #495057;
+  --bs-dark-border-subtle: #343a40;
+  --bs-heading-color: inherit;
+  --bs-link-color: #6ea8fe;
+  --bs-link-hover-color: #8bb9fe;
+  --bs-link-color-rgb: 110, 168, 254;
+  --bs-link-hover-color-rgb: 139, 185, 254;
+  --bs-code-color: #e685b5;
+  --bs-border-color: #495057;
+  --bs-border-color-translucent: rgba(255, 255, 255, 0.15);
+  --bs-form-valid-color: #75b798;
+  --bs-form-valid-border-color: #75b798;
+  --bs-form-invalid-color: #ea868f;
+  --bs-form-invalid-border-color: #ea868f;
 }
 
 *,
 *::before,
 *::after {
   box-sizing: border-box;
 }
@@ -99,23 +203,24 @@
   -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
 }
 
 hr {
   margin: 1rem 0;
   color: inherit;
   border: 0;
-  border-top: 1px solid;
+  border-top: var(--bs-border-width) solid;
   opacity: 0.25;
 }
 
 h6, .h6, h5, .h5, h4, .h4, h3, .h3, h2, .h2, h1, .h1 {
   margin-top: 0;
   margin-bottom: 0.5rem;
   font-weight: 500;
   line-height: 1.2;
+  color: var(--bs-heading-color);
 }
 
 h1, .h1 {
   font-size: calc(1.375rem + 1.5vw);
 }
 @media (min-width: 1200px) {
   h1, .h1 {
@@ -236,19 +341,19 @@
 }
 
 sup {
   top: -0.5em;
 }
 
 a {
-  color: var(--bs-link-color);
+  color: rgba(var(--bs-link-color-rgb), var(--bs-link-opacity, 1));
   text-decoration: underline;
 }
 a:hover {
-  color: var(--bs-link-hover-color);
+  --bs-link-color-rgb: var(--bs-link-hover-color-rgb);
 }
 
 a:not([href]):not([class]), a:not([href]):not([class]):hover {
   color: inherit;
   text-decoration: none;
 }
 
@@ -307,15 +412,15 @@
   caption-side: bottom;
   border-collapse: collapse;
 }
 
 caption {
   padding-top: 0.5rem;
   padding-bottom: 0.5rem;
-  color: #6c757d;
+  color: var(--bs-secondary-color);
   text-align: left;
 }
 
 th {
   text-align: inherit;
   text-align: -webkit-match-parent;
 }
@@ -431,16 +536,16 @@
 }
 
 ::-webkit-inner-spin-button {
   height: auto;
 }
 
 [type=search] {
-  outline-offset: -2px;
   -webkit-appearance: textfield;
+  outline-offset: -2px;
 }
 
 /* rtl:raw:
 [type="tel"],
 [type="url"],
 [type="email"],
 [type="number"] {
@@ -600,17 +705,17 @@
 .img-fluid {
   max-width: 100%;
   height: auto;
 }
 
 .img-thumbnail {
   padding: 0.25rem;
-  background-color: #fff;
-  border: 1px solid var(--bs-border-color);
-  border-radius: 0.375rem;
+  background-color: var(--bs-body-bg);
+  border: var(--bs-border-width) solid var(--bs-border-color);
+  border-radius: var(--bs-border-radius);
   max-width: 100%;
   height: auto;
 }
 
 .figure {
   display: inline-block;
 }
@@ -618,15 +723,15 @@
 .figure-img {
   margin-bottom: 0.5rem;
   line-height: 1;
 }
 
 .figure-caption {
   font-size: 0.875em;
-  color: #6c757d;
+  color: var(--bs-secondary-color);
 }
 
 .container,
 .container-fluid,
 .container-xxl,
 .container-xl,
 .container-lg,
@@ -662,14 +767,23 @@
   }
 }
 @media (min-width: 1400px) {
   .container-xxl, .container-xl, .container-lg, .container-md, .container-sm, .container {
     max-width: 1320px;
   }
 }
+:root {
+  --bs-breakpoint-xs: 0;
+  --bs-breakpoint-sm: 576px;
+  --bs-breakpoint-md: 768px;
+  --bs-breakpoint-lg: 992px;
+  --bs-breakpoint-xl: 1200px;
+  --bs-breakpoint-xxl: 1400px;
+}
+
 .row {
   --bs-gutter-x: 1.5rem;
   --bs-gutter-y: 0;
   display: flex;
   flex-wrap: wrap;
   margin-top: calc(-1 * var(--bs-gutter-y));
   margin-right: calc(-0.5 * var(--bs-gutter-x));
@@ -1009,59 +1123,59 @@
   .offset-sm-10 {
     margin-left: 83.33333333%;
   }
   .offset-sm-11 {
     margin-left: 91.66666667%;
   }
   .g-sm-0,
-.gx-sm-0 {
+  .gx-sm-0 {
     --bs-gutter-x: 0;
   }
   .g-sm-0,
-.gy-sm-0 {
+  .gy-sm-0 {
     --bs-gutter-y: 0;
   }
   .g-sm-1,
-.gx-sm-1 {
+  .gx-sm-1 {
     --bs-gutter-x: 0.25rem;
   }
   .g-sm-1,
-.gy-sm-1 {
+  .gy-sm-1 {
     --bs-gutter-y: 0.25rem;
   }
   .g-sm-2,
-.gx-sm-2 {
+  .gx-sm-2 {
     --bs-gutter-x: 0.5rem;
   }
   .g-sm-2,
-.gy-sm-2 {
+  .gy-sm-2 {
     --bs-gutter-y: 0.5rem;
   }
   .g-sm-3,
-.gx-sm-3 {
+  .gx-sm-3 {
     --bs-gutter-x: 1rem;
   }
   .g-sm-3,
-.gy-sm-3 {
+  .gy-sm-3 {
     --bs-gutter-y: 1rem;
   }
   .g-sm-4,
-.gx-sm-4 {
+  .gx-sm-4 {
     --bs-gutter-x: 1.5rem;
   }
   .g-sm-4,
-.gy-sm-4 {
+  .gy-sm-4 {
     --bs-gutter-y: 1.5rem;
   }
   .g-sm-5,
-.gx-sm-5 {
+  .gx-sm-5 {
     --bs-gutter-x: 3rem;
   }
   .g-sm-5,
-.gy-sm-5 {
+  .gy-sm-5 {
     --bs-gutter-y: 3rem;
   }
 }
 @media (min-width: 768px) {
   .col-md {
     flex: 1 0 0%;
   }
@@ -1178,59 +1292,59 @@
   .offset-md-10 {
     margin-left: 83.33333333%;
   }
   .offset-md-11 {
     margin-left: 91.66666667%;
   }
   .g-md-0,
-.gx-md-0 {
+  .gx-md-0 {
     --bs-gutter-x: 0;
   }
   .g-md-0,
-.gy-md-0 {
+  .gy-md-0 {
     --bs-gutter-y: 0;
   }
   .g-md-1,
-.gx-md-1 {
+  .gx-md-1 {
     --bs-gutter-x: 0.25rem;
   }
   .g-md-1,
-.gy-md-1 {
+  .gy-md-1 {
     --bs-gutter-y: 0.25rem;
   }
   .g-md-2,
-.gx-md-2 {
+  .gx-md-2 {
     --bs-gutter-x: 0.5rem;
   }
   .g-md-2,
-.gy-md-2 {
+  .gy-md-2 {
     --bs-gutter-y: 0.5rem;
   }
   .g-md-3,
-.gx-md-3 {
+  .gx-md-3 {
     --bs-gutter-x: 1rem;
   }
   .g-md-3,
-.gy-md-3 {
+  .gy-md-3 {
     --bs-gutter-y: 1rem;
   }
   .g-md-4,
-.gx-md-4 {
+  .gx-md-4 {
     --bs-gutter-x: 1.5rem;
   }
   .g-md-4,
-.gy-md-4 {
+  .gy-md-4 {
     --bs-gutter-y: 1.5rem;
   }
   .g-md-5,
-.gx-md-5 {
+  .gx-md-5 {
     --bs-gutter-x: 3rem;
   }
   .g-md-5,
-.gy-md-5 {
+  .gy-md-5 {
     --bs-gutter-y: 3rem;
   }
 }
 @media (min-width: 992px) {
   .col-lg {
     flex: 1 0 0%;
   }
@@ -1347,59 +1461,59 @@
   .offset-lg-10 {
     margin-left: 83.33333333%;
   }
   .offset-lg-11 {
     margin-left: 91.66666667%;
   }
   .g-lg-0,
-.gx-lg-0 {
+  .gx-lg-0 {
     --bs-gutter-x: 0;
   }
   .g-lg-0,
-.gy-lg-0 {
+  .gy-lg-0 {
     --bs-gutter-y: 0;
   }
   .g-lg-1,
-.gx-lg-1 {
+  .gx-lg-1 {
     --bs-gutter-x: 0.25rem;
   }
   .g-lg-1,
-.gy-lg-1 {
+  .gy-lg-1 {
     --bs-gutter-y: 0.25rem;
   }
   .g-lg-2,
-.gx-lg-2 {
+  .gx-lg-2 {
     --bs-gutter-x: 0.5rem;
   }
   .g-lg-2,
-.gy-lg-2 {
+  .gy-lg-2 {
     --bs-gutter-y: 0.5rem;
   }
   .g-lg-3,
-.gx-lg-3 {
+  .gx-lg-3 {
     --bs-gutter-x: 1rem;
   }
   .g-lg-3,
-.gy-lg-3 {
+  .gy-lg-3 {
     --bs-gutter-y: 1rem;
   }
   .g-lg-4,
-.gx-lg-4 {
+  .gx-lg-4 {
     --bs-gutter-x: 1.5rem;
   }
   .g-lg-4,
-.gy-lg-4 {
+  .gy-lg-4 {
     --bs-gutter-y: 1.5rem;
   }
   .g-lg-5,
-.gx-lg-5 {
+  .gx-lg-5 {
     --bs-gutter-x: 3rem;
   }
   .g-lg-5,
-.gy-lg-5 {
+  .gy-lg-5 {
     --bs-gutter-y: 3rem;
   }
 }
 @media (min-width: 1200px) {
   .col-xl {
     flex: 1 0 0%;
   }
@@ -1516,59 +1630,59 @@
   .offset-xl-10 {
     margin-left: 83.33333333%;
   }
   .offset-xl-11 {
     margin-left: 91.66666667%;
   }
   .g-xl-0,
-.gx-xl-0 {
+  .gx-xl-0 {
     --bs-gutter-x: 0;
   }
   .g-xl-0,
-.gy-xl-0 {
+  .gy-xl-0 {
     --bs-gutter-y: 0;
   }
   .g-xl-1,
-.gx-xl-1 {
+  .gx-xl-1 {
     --bs-gutter-x: 0.25rem;
   }
   .g-xl-1,
-.gy-xl-1 {
+  .gy-xl-1 {
     --bs-gutter-y: 0.25rem;
   }
   .g-xl-2,
-.gx-xl-2 {
+  .gx-xl-2 {
     --bs-gutter-x: 0.5rem;
   }
   .g-xl-2,
-.gy-xl-2 {
+  .gy-xl-2 {
     --bs-gutter-y: 0.5rem;
   }
   .g-xl-3,
-.gx-xl-3 {
+  .gx-xl-3 {
     --bs-gutter-x: 1rem;
   }
   .g-xl-3,
-.gy-xl-3 {
+  .gy-xl-3 {
     --bs-gutter-y: 1rem;
   }
   .g-xl-4,
-.gx-xl-4 {
+  .gx-xl-4 {
     --bs-gutter-x: 1.5rem;
   }
   .g-xl-4,
-.gy-xl-4 {
+  .gy-xl-4 {
     --bs-gutter-y: 1.5rem;
   }
   .g-xl-5,
-.gx-xl-5 {
+  .gx-xl-5 {
     --bs-gutter-x: 3rem;
   }
   .g-xl-5,
-.gy-xl-5 {
+  .gy-xl-5 {
     --bs-gutter-y: 3rem;
   }
 }
 @media (min-width: 1400px) {
   .col-xxl {
     flex: 1 0 0%;
   }
@@ -1685,136 +1799,140 @@
   .offset-xxl-10 {
     margin-left: 83.33333333%;
   }
   .offset-xxl-11 {
     margin-left: 91.66666667%;
   }
   .g-xxl-0,
-.gx-xxl-0 {
+  .gx-xxl-0 {
     --bs-gutter-x: 0;
   }
   .g-xxl-0,
-.gy-xxl-0 {
+  .gy-xxl-0 {
     --bs-gutter-y: 0;
   }
   .g-xxl-1,
-.gx-xxl-1 {
+  .gx-xxl-1 {
     --bs-gutter-x: 0.25rem;
   }
   .g-xxl-1,
-.gy-xxl-1 {
+  .gy-xxl-1 {
     --bs-gutter-y: 0.25rem;
   }
   .g-xxl-2,
-.gx-xxl-2 {
+  .gx-xxl-2 {
     --bs-gutter-x: 0.5rem;
   }
   .g-xxl-2,
-.gy-xxl-2 {
+  .gy-xxl-2 {
     --bs-gutter-y: 0.5rem;
   }
   .g-xxl-3,
-.gx-xxl-3 {
+  .gx-xxl-3 {
     --bs-gutter-x: 1rem;
   }
   .g-xxl-3,
-.gy-xxl-3 {
+  .gy-xxl-3 {
     --bs-gutter-y: 1rem;
   }
   .g-xxl-4,
-.gx-xxl-4 {
+  .gx-xxl-4 {
     --bs-gutter-x: 1.5rem;
   }
   .g-xxl-4,
-.gy-xxl-4 {
+  .gy-xxl-4 {
     --bs-gutter-y: 1.5rem;
   }
   .g-xxl-5,
-.gx-xxl-5 {
+  .gx-xxl-5 {
     --bs-gutter-x: 3rem;
   }
   .g-xxl-5,
-.gy-xxl-5 {
+  .gy-xxl-5 {
     --bs-gutter-y: 3rem;
   }
 }
 .table {
+  --bs-table-color-type: initial;
+  --bs-table-bg-type: initial;
+  --bs-table-color-state: initial;
+  --bs-table-bg-state: initial;
   --bs-table-color: var(--bs-body-color);
-  --bs-table-bg: transparent;
+  --bs-table-bg: var(--bs-body-bg);
   --bs-table-border-color: var(--bs-border-color);
   --bs-table-accent-bg: transparent;
   --bs-table-striped-color: var(--bs-body-color);
   --bs-table-striped-bg: rgba(0, 0, 0, 0.05);
   --bs-table-active-color: var(--bs-body-color);
   --bs-table-active-bg: rgba(0, 0, 0, 0.1);
   --bs-table-hover-color: var(--bs-body-color);
   --bs-table-hover-bg: rgba(0, 0, 0, 0.075);
   width: 100%;
   margin-bottom: 1rem;
-  color: var(--bs-table-color);
   vertical-align: top;
   border-color: var(--bs-table-border-color);
 }
 .table > :not(caption) > * > * {
   padding: 0.5rem 0.5rem;
+  color: var(--bs-table-color-state, var(--bs-table-color-type, var(--bs-table-color)));
   background-color: var(--bs-table-bg);
-  border-bottom-width: 1px;
-  box-shadow: inset 0 0 0 9999px var(--bs-table-accent-bg);
+  border-bottom-width: var(--bs-border-width);
+  box-shadow: inset 0 0 0 9999px var(--bs-table-bg-state, var(--bs-table-bg-type, var(--bs-table-accent-bg)));
 }
 .table > tbody {
   vertical-align: inherit;
 }
 .table > thead {
   vertical-align: bottom;
 }
 
 .table-group-divider {
-  border-top: 2px solid currentcolor;
+  border-top: calc(var(--bs-border-width) * 2) solid currentcolor;
 }
 
 .caption-top {
   caption-side: top;
 }
 
 .table-sm > :not(caption) > * > * {
   padding: 0.25rem 0.25rem;
 }
 
 .table-bordered > :not(caption) > * {
-  border-width: 1px 0;
+  border-width: var(--bs-border-width) 0;
 }
 .table-bordered > :not(caption) > * > * {
-  border-width: 0 1px;
+  border-width: 0 var(--bs-border-width);
 }
 
 .table-borderless > :not(caption) > * > * {
   border-bottom-width: 0;
 }
 .table-borderless > :not(:first-child) {
   border-top-width: 0;
 }
 
 .table-striped > tbody > tr:nth-of-type(odd) > * {
-  --bs-table-accent-bg: var(--bs-table-striped-bg);
-  color: var(--bs-table-striped-color);
+  --bs-table-color-type: var(--bs-table-striped-color);
+  --bs-table-bg-type: var(--bs-table-striped-bg);
 }
 
 .table-striped-columns > :not(caption) > tr > :nth-child(even) {
-  --bs-table-accent-bg: var(--bs-table-striped-bg);
-  color: var(--bs-table-striped-color);
+  --bs-table-color-type: var(--bs-table-striped-color);
+  --bs-table-bg-type: var(--bs-table-striped-bg);
 }
 
 .table-active {
-  --bs-table-accent-bg: var(--bs-table-active-bg);
-  color: var(--bs-table-active-color);
+  --bs-table-color-state: var(--bs-table-active-color);
+  --bs-table-bg-state: var(--bs-table-active-bg);
 }
 
 .table-hover > tbody > tr:hover > * {
-  --bs-table-accent-bg: var(--bs-table-hover-bg);
-  color: var(--bs-table-hover-color);
+  --bs-table-color-state: var(--bs-table-hover-color);
+  --bs-table-bg-state: var(--bs-table-hover-bg);
 }
 
 .table-primary {
   --bs-table-color: #000;
   --bs-table-bg: #cfe2ff;
   --bs-table-border-color: #bacbe6;
   --bs-table-striped-bg: #c5d7f2;
@@ -1961,160 +2079,166 @@
   }
 }
 .form-label {
   margin-bottom: 0.5rem;
 }
 
 .col-form-label {
-  padding-top: calc(0.375rem + 1px);
-  padding-bottom: calc(0.375rem + 1px);
+  padding-top: calc(0.375rem + var(--bs-border-width));
+  padding-bottom: calc(0.375rem + var(--bs-border-width));
   margin-bottom: 0;
   font-size: inherit;
   line-height: 1.5;
 }
 
 .col-form-label-lg {
-  padding-top: calc(0.5rem + 1px);
-  padding-bottom: calc(0.5rem + 1px);
+  padding-top: calc(0.5rem + var(--bs-border-width));
+  padding-bottom: calc(0.5rem + var(--bs-border-width));
   font-size: 1.25rem;
 }
 
 .col-form-label-sm {
-  padding-top: calc(0.25rem + 1px);
-  padding-bottom: calc(0.25rem + 1px);
+  padding-top: calc(0.25rem + var(--bs-border-width));
+  padding-bottom: calc(0.25rem + var(--bs-border-width));
   font-size: 0.875rem;
 }
 
 .form-text {
   margin-top: 0.25rem;
   font-size: 0.875em;
-  color: #6c757d;
+  color: var(--bs-secondary-color);
 }
 
 .form-control {
   display: block;
   width: 100%;
   padding: 0.375rem 0.75rem;
   font-size: 1rem;
   font-weight: 400;
   line-height: 1.5;
-  color: #212529;
-  background-color: #fff;
-  background-clip: padding-box;
-  border: 1px solid #ced4da;
+  color: var(--bs-body-color);
   -webkit-appearance: none;
   -moz-appearance: none;
   appearance: none;
-  border-radius: 0.375rem;
+  background-color: var(--bs-body-bg);
+  background-clip: padding-box;
+  border: var(--bs-border-width) solid var(--bs-border-color);
+  border-radius: var(--bs-border-radius);
   transition: border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
 }
 @media (prefers-reduced-motion: reduce) {
   .form-control {
     transition: none;
   }
 }
 .form-control[type=file] {
   overflow: hidden;
 }
 .form-control[type=file]:not(:disabled):not([readonly]) {
   cursor: pointer;
 }
 .form-control:focus {
-  color: #212529;
-  background-color: #fff;
+  color: var(--bs-body-color);
+  background-color: var(--bs-body-bg);
   border-color: #86b7fe;
   outline: 0;
   box-shadow: 0 0 0 0.25rem rgba(13, 110, 253, 0.25);
 }
 .form-control::-webkit-date-and-time-value {
+  min-width: 85px;
   height: 1.5em;
+  margin: 0;
+}
+.form-control::-webkit-datetime-edit {
+  display: block;
+  padding: 0;
 }
 .form-control::-moz-placeholder {
-  color: #6c757d;
+  color: var(--bs-secondary-color);
   opacity: 1;
 }
 .form-control::placeholder {
-  color: #6c757d;
+  color: var(--bs-secondary-color);
   opacity: 1;
 }
 .form-control:disabled {
-  background-color: #e9ecef;
+  background-color: var(--bs-secondary-bg);
   opacity: 1;
 }
 .form-control::-webkit-file-upload-button {
   padding: 0.375rem 0.75rem;
   margin: -0.375rem -0.75rem;
   -webkit-margin-end: 0.75rem;
   margin-inline-end: 0.75rem;
-  color: #212529;
-  background-color: #e9ecef;
+  color: var(--bs-body-color);
+  background-color: var(--bs-tertiary-bg);
   pointer-events: none;
   border-color: inherit;
   border-style: solid;
   border-width: 0;
-  border-inline-end-width: 1px;
+  border-inline-end-width: var(--bs-border-width);
   border-radius: 0;
   -webkit-transition: color 0.15s ease-in-out, background-color 0.15s ease-in-out, border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
   transition: color 0.15s ease-in-out, background-color 0.15s ease-in-out, border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
 }
 .form-control::file-selector-button {
   padding: 0.375rem 0.75rem;
   margin: -0.375rem -0.75rem;
   -webkit-margin-end: 0.75rem;
   margin-inline-end: 0.75rem;
-  color: #212529;
-  background-color: #e9ecef;
+  color: var(--bs-body-color);
+  background-color: var(--bs-tertiary-bg);
   pointer-events: none;
   border-color: inherit;
   border-style: solid;
   border-width: 0;
-  border-inline-end-width: 1px;
+  border-inline-end-width: var(--bs-border-width);
   border-radius: 0;
   transition: color 0.15s ease-in-out, background-color 0.15s ease-in-out, border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
 }
 @media (prefers-reduced-motion: reduce) {
   .form-control::-webkit-file-upload-button {
     -webkit-transition: none;
     transition: none;
   }
   .form-control::file-selector-button {
     transition: none;
   }
 }
 .form-control:hover:not(:disabled):not([readonly])::-webkit-file-upload-button {
-  background-color: #dde0e3;
+  background-color: var(--bs-secondary-bg);
 }
 .form-control:hover:not(:disabled):not([readonly])::file-selector-button {
-  background-color: #dde0e3;
+  background-color: var(--bs-secondary-bg);
 }
 
 .form-control-plaintext {
   display: block;
   width: 100%;
   padding: 0.375rem 0;
   margin-bottom: 0;
   line-height: 1.5;
-  color: #212529;
+  color: var(--bs-body-color);
   background-color: transparent;
   border: solid transparent;
-  border-width: 1px 0;
+  border-width: var(--bs-border-width) 0;
 }
 .form-control-plaintext:focus {
   outline: 0;
 }
 .form-control-plaintext.form-control-sm, .form-control-plaintext.form-control-lg {
   padding-right: 0;
   padding-left: 0;
 }
 
 .form-control-sm {
-  min-height: calc(1.5em + 0.5rem + 2px);
+  min-height: calc(1.5em + 0.5rem + calc(var(--bs-border-width) * 2));
   padding: 0.25rem 0.5rem;
   font-size: 0.875rem;
-  border-radius: 0.25rem;
+  border-radius: var(--bs-border-radius-sm);
 }
 .form-control-sm::-webkit-file-upload-button {
   padding: 0.25rem 0.5rem;
   margin: -0.25rem -0.5rem;
   -webkit-margin-end: 0.5rem;
   margin-inline-end: 0.5rem;
 }
@@ -2122,18 +2246,18 @@
   padding: 0.25rem 0.5rem;
   margin: -0.25rem -0.5rem;
   -webkit-margin-end: 0.5rem;
   margin-inline-end: 0.5rem;
 }
 
 .form-control-lg {
-  min-height: calc(1.5em + 1rem + 2px);
+  min-height: calc(1.5em + 1rem + calc(var(--bs-border-width) * 2));
   padding: 0.5rem 1rem;
   font-size: 1.25rem;
-  border-radius: 0.5rem;
+  border-radius: var(--bs-border-radius-lg);
 }
 .form-control-lg::-webkit-file-upload-button {
   padding: 0.5rem 1rem;
   margin: -0.5rem -1rem;
   -webkit-margin-end: 1rem;
   margin-inline-end: 1rem;
 }
@@ -2141,65 +2265,66 @@
   padding: 0.5rem 1rem;
   margin: -0.5rem -1rem;
   -webkit-margin-end: 1rem;
   margin-inline-end: 1rem;
 }
 
 textarea.form-control {
-  min-height: calc(1.5em + 0.75rem + 2px);
+  min-height: calc(1.5em + 0.75rem + calc(var(--bs-border-width) * 2));
 }
 textarea.form-control-sm {
-  min-height: calc(1.5em + 0.5rem + 2px);
+  min-height: calc(1.5em + 0.5rem + calc(var(--bs-border-width) * 2));
 }
 textarea.form-control-lg {
-  min-height: calc(1.5em + 1rem + 2px);
+  min-height: calc(1.5em + 1rem + calc(var(--bs-border-width) * 2));
 }
 
 .form-control-color {
   width: 3rem;
-  height: calc(1.5em + 0.75rem + 2px);
+  height: calc(1.5em + 0.75rem + calc(var(--bs-border-width) * 2));
   padding: 0.375rem;
 }
 .form-control-color:not(:disabled):not([readonly]) {
   cursor: pointer;
 }
 .form-control-color::-moz-color-swatch {
   border: 0 !important;
-  border-radius: 0.375rem;
+  border-radius: var(--bs-border-radius);
 }
 .form-control-color::-webkit-color-swatch {
-  border-radius: 0.375rem;
+  border: 0 !important;
+  border-radius: var(--bs-border-radius);
 }
 .form-control-color.form-control-sm {
-  height: calc(1.5em + 0.5rem + 2px);
+  height: calc(1.5em + 0.5rem + calc(var(--bs-border-width) * 2));
 }
 .form-control-color.form-control-lg {
-  height: calc(1.5em + 1rem + 2px);
+  height: calc(1.5em + 1rem + calc(var(--bs-border-width) * 2));
 }
 
 .form-select {
+  --bs-form-select-bg-img: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill='none' stroke='%23343a40' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='m2 5 6 6 6-6'/%3e%3c/svg%3e");
   display: block;
   width: 100%;
   padding: 0.375rem 2.25rem 0.375rem 0.75rem;
-  -moz-padding-start: calc(0.75rem - 3px);
   font-size: 1rem;
   font-weight: 400;
   line-height: 1.5;
-  color: #212529;
-  background-color: #fff;
-  background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill='none' stroke='%23343a40' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='m2 5 6 6 6-6'/%3e%3c/svg%3e");
+  color: var(--bs-body-color);
+  -webkit-appearance: none;
+  -moz-appearance: none;
+  appearance: none;
+  background-color: var(--bs-body-bg);
+  background-image: var(--bs-form-select-bg-img), var(--bs-form-select-bg-icon, none);
   background-repeat: no-repeat;
   background-position: right 0.75rem center;
   background-size: 16px 12px;
-  border: 1px solid #ced4da;
-  border-radius: 0.375rem;
+  border: var(--bs-border-width) solid var(--bs-border-color);
+  border-radius: var(--bs-border-radius);
   transition: border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
-  -webkit-appearance: none;
-  -moz-appearance: none;
-  appearance: none;
 }
 @media (prefers-reduced-motion: reduce) {
   .form-select {
     transition: none;
   }
 }
 .form-select:focus {
@@ -2208,35 +2333,39 @@
   box-shadow: 0 0 0 0.25rem rgba(13, 110, 253, 0.25);
 }
 .form-select[multiple], .form-select[size]:not([size="1"]) {
   padding-right: 0.75rem;
   background-image: none;
 }
 .form-select:disabled {
-  background-color: #e9ecef;
+  background-color: var(--bs-secondary-bg);
 }
 .form-select:-moz-focusring {
   color: transparent;
-  text-shadow: 0 0 0 #212529;
+  text-shadow: 0 0 0 var(--bs-body-color);
 }
 
 .form-select-sm {
   padding-top: 0.25rem;
   padding-bottom: 0.25rem;
   padding-left: 0.5rem;
   font-size: 0.875rem;
-  border-radius: 0.25rem;
+  border-radius: var(--bs-border-radius-sm);
 }
 
 .form-select-lg {
   padding-top: 0.5rem;
   padding-bottom: 0.5rem;
   padding-left: 1rem;
   font-size: 1.25rem;
-  border-radius: 0.5rem;
+  border-radius: var(--bs-border-radius-lg);
+}
+
+[data-bs-theme=dark] .form-select {
+  --bs-form-select-bg-img: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill='none' stroke='%23dee2e6' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='m2 5 6 6 6-6'/%3e%3c/svg%3e");
 }
 
 .form-check {
   display: block;
   min-height: 1.5rem;
   padding-left: 1.5em;
   margin-bottom: 0.125rem;
@@ -2254,26 +2383,28 @@
 .form-check-reverse .form-check-input {
   float: right;
   margin-right: -1.5em;
   margin-left: 0;
 }
 
 .form-check-input {
+  --bs-form-check-bg: var(--bs-body-bg);
   width: 1em;
   height: 1em;
   margin-top: 0.25em;
   vertical-align: top;
-  background-color: #fff;
-  background-repeat: no-repeat;
-  background-position: center;
-  background-size: contain;
-  border: 1px solid rgba(0, 0, 0, 0.25);
   -webkit-appearance: none;
   -moz-appearance: none;
   appearance: none;
+  background-color: var(--bs-form-check-bg);
+  background-image: var(--bs-form-check-bg-image);
+  background-repeat: no-repeat;
+  background-position: center;
+  background-size: contain;
+  border: var(--bs-border-width) solid var(--bs-border-color);
   -webkit-print-color-adjust: exact;
   color-adjust: exact;
   print-color-adjust: exact;
 }
 .form-check-input[type=checkbox] {
   border-radius: 0.25em;
 }
@@ -2289,23 +2420,23 @@
   box-shadow: 0 0 0 0.25rem rgba(13, 110, 253, 0.25);
 }
 .form-check-input:checked {
   background-color: #0d6efd;
   border-color: #0d6efd;
 }
 .form-check-input:checked[type=checkbox] {
-  background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 20 20'%3e%3cpath fill='none' stroke='%23fff' stroke-linecap='round' stroke-linejoin='round' stroke-width='3' d='m6 10 3 3 6-6'/%3e%3c/svg%3e");
+  --bs-form-check-bg-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 20 20'%3e%3cpath fill='none' stroke='%23fff' stroke-linecap='round' stroke-linejoin='round' stroke-width='3' d='m6 10 3 3 6-6'/%3e%3c/svg%3e");
 }
 .form-check-input:checked[type=radio] {
-  background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='2' fill='%23fff'/%3e%3c/svg%3e");
+  --bs-form-check-bg-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='2' fill='%23fff'/%3e%3c/svg%3e");
 }
 .form-check-input[type=checkbox]:indeterminate {
   background-color: #0d6efd;
   border-color: #0d6efd;
-  background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 20 20'%3e%3cpath fill='none' stroke='%23fff' stroke-linecap='round' stroke-linejoin='round' stroke-width='3' d='M6 10h8'/%3e%3c/svg%3e");
+  --bs-form-check-bg-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 20 20'%3e%3cpath fill='none' stroke='%23fff' stroke-linecap='round' stroke-linejoin='round' stroke-width='3' d='M6 10h8'/%3e%3c/svg%3e");
 }
 .form-check-input:disabled {
   pointer-events: none;
   filter: none;
   opacity: 0.5;
 }
 .form-check-input[disabled] ~ .form-check-label, .form-check-input:disabled ~ .form-check-label {
@@ -2313,32 +2444,33 @@
   opacity: 0.5;
 }
 
 .form-switch {
   padding-left: 2.5em;
 }
 .form-switch .form-check-input {
+  --bs-form-switch-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='3' fill='rgba%280, 0, 0, 0.25%29'/%3e%3c/svg%3e");
   width: 2em;
   margin-left: -2.5em;
-  background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='3' fill='rgba%280, 0, 0, 0.25%29'/%3e%3c/svg%3e");
+  background-image: var(--bs-form-switch-bg);
   background-position: left center;
   border-radius: 2em;
   transition: background-position 0.15s ease-in-out;
 }
 @media (prefers-reduced-motion: reduce) {
   .form-switch .form-check-input {
     transition: none;
   }
 }
 .form-switch .form-check-input:focus {
-  background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='3' fill='%2386b7fe'/%3e%3c/svg%3e");
+  --bs-form-switch-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='3' fill='%2386b7fe'/%3e%3c/svg%3e");
 }
 .form-switch .form-check-input:checked {
   background-position: right center;
-  background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='3' fill='%23fff'/%3e%3c/svg%3e");
+  --bs-form-switch-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='3' fill='%23fff'/%3e%3c/svg%3e");
 }
 .form-switch.form-check-reverse {
   padding-right: 2.5em;
   padding-left: 0;
 }
 .form-switch.form-check-reverse .form-check-input {
   margin-right: -2.5em;
@@ -2357,22 +2489,26 @@
 }
 .btn-check[disabled] + .btn, .btn-check:disabled + .btn {
   pointer-events: none;
   filter: none;
   opacity: 0.65;
 }
 
+[data-bs-theme=dark] .form-switch .form-check-input:not(:checked):not(:focus) {
+  --bs-form-switch-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='3' fill='rgba%28255, 255, 255, 0.25%29'/%3e%3c/svg%3e");
+}
+
 .form-range {
   width: 100%;
   height: 1.5rem;
   padding: 0;
-  background-color: transparent;
   -webkit-appearance: none;
   -moz-appearance: none;
   appearance: none;
+  background-color: transparent;
 }
 .form-range:focus {
   outline: 0;
 }
 .form-range:focus::-webkit-slider-thumb {
   box-shadow: 0 0 0 1px #fff, 0 0 0 0.25rem rgba(13, 110, 253, 0.25);
 }
@@ -2382,21 +2518,21 @@
 .form-range::-moz-focus-outer {
   border: 0;
 }
 .form-range::-webkit-slider-thumb {
   width: 1rem;
   height: 1rem;
   margin-top: -0.25rem;
+  -webkit-appearance: none;
+  appearance: none;
   background-color: #0d6efd;
   border: 0;
   border-radius: 1rem;
   -webkit-transition: background-color 0.15s ease-in-out, border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
   transition: background-color 0.15s ease-in-out, border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
-  -webkit-appearance: none;
-  appearance: none;
 }
 @media (prefers-reduced-motion: reduce) {
   .form-range::-webkit-slider-thumb {
     -webkit-transition: none;
     transition: none;
   }
 }
@@ -2404,28 +2540,28 @@
   background-color: #b6d4fe;
 }
 .form-range::-webkit-slider-runnable-track {
   width: 100%;
   height: 0.5rem;
   color: transparent;
   cursor: pointer;
-  background-color: #dee2e6;
+  background-color: var(--bs-tertiary-bg);
   border-color: transparent;
   border-radius: 1rem;
 }
 .form-range::-moz-range-thumb {
   width: 1rem;
   height: 1rem;
+  -moz-appearance: none;
+  appearance: none;
   background-color: #0d6efd;
   border: 0;
   border-radius: 1rem;
   -moz-transition: background-color 0.15s ease-in-out, border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
   transition: background-color 0.15s ease-in-out, border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
-  -moz-appearance: none;
-  appearance: none;
 }
 @media (prefers-reduced-motion: reduce) {
   .form-range::-moz-range-thumb {
     -moz-transition: none;
     transition: none;
   }
 }
@@ -2433,50 +2569,51 @@
   background-color: #b6d4fe;
 }
 .form-range::-moz-range-track {
   width: 100%;
   height: 0.5rem;
   color: transparent;
   cursor: pointer;
-  background-color: #dee2e6;
+  background-color: var(--bs-tertiary-bg);
   border-color: transparent;
   border-radius: 1rem;
 }
 .form-range:disabled {
   pointer-events: none;
 }
 .form-range:disabled::-webkit-slider-thumb {
-  background-color: #adb5bd;
+  background-color: var(--bs-secondary-color);
 }
 .form-range:disabled::-moz-range-thumb {
-  background-color: #adb5bd;
+  background-color: var(--bs-secondary-color);
 }
 
 .form-floating {
   position: relative;
 }
 .form-floating > .form-control,
 .form-floating > .form-control-plaintext,
 .form-floating > .form-select {
-  height: calc(3.5rem + 2px);
+  height: calc(3.5rem + calc(var(--bs-border-width) * 2));
+  min-height: calc(3.5rem + calc(var(--bs-border-width) * 2));
   line-height: 1.25;
 }
 .form-floating > label {
   position: absolute;
   top: 0;
   left: 0;
-  width: 100%;
+  z-index: 2;
   height: 100%;
   padding: 1rem 0.75rem;
   overflow: hidden;
   text-align: start;
   text-overflow: ellipsis;
   white-space: nowrap;
   pointer-events: none;
-  border: 1px solid transparent;
+  border: var(--bs-border-width) solid transparent;
   transform-origin: 0 0;
   transition: opacity 0.1s ease-in-out, transform 0.1s ease-in-out;
 }
 @media (prefers-reduced-motion: reduce) {
   .form-floating > label {
     transition: none;
   }
@@ -2508,30 +2645,59 @@
   padding-bottom: 0.625rem;
 }
 .form-floating > .form-select {
   padding-top: 1.625rem;
   padding-bottom: 0.625rem;
 }
 .form-floating > .form-control:not(:-moz-placeholder-shown) ~ label {
-  opacity: 0.65;
+  color: rgba(var(--bs-body-color-rgb), 0.65);
   transform: scale(0.85) translateY(-0.5rem) translateX(0.15rem);
 }
 .form-floating > .form-control:focus ~ label,
 .form-floating > .form-control:not(:placeholder-shown) ~ label,
 .form-floating > .form-control-plaintext ~ label,
 .form-floating > .form-select ~ label {
-  opacity: 0.65;
+  color: rgba(var(--bs-body-color-rgb), 0.65);
   transform: scale(0.85) translateY(-0.5rem) translateX(0.15rem);
 }
+.form-floating > .form-control:not(:-moz-placeholder-shown) ~ label::after {
+  position: absolute;
+  inset: 1rem 0.375rem;
+  z-index: -1;
+  height: 1.5em;
+  content: "";
+  background-color: var(--bs-body-bg);
+  border-radius: var(--bs-border-radius);
+}
+.form-floating > .form-control:focus ~ label::after,
+.form-floating > .form-control:not(:placeholder-shown) ~ label::after,
+.form-floating > .form-control-plaintext ~ label::after,
+.form-floating > .form-select ~ label::after {
+  position: absolute;
+  inset: 1rem 0.375rem;
+  z-index: -1;
+  height: 1.5em;
+  content: "";
+  background-color: var(--bs-body-bg);
+  border-radius: var(--bs-border-radius);
+}
 .form-floating > .form-control:-webkit-autofill ~ label {
-  opacity: 0.65;
+  color: rgba(var(--bs-body-color-rgb), 0.65);
   transform: scale(0.85) translateY(-0.5rem) translateX(0.15rem);
 }
 .form-floating > .form-control-plaintext ~ label {
-  border-width: 1px 0;
+  border-width: var(--bs-border-width) 0;
+}
+.form-floating > :disabled ~ label,
+.form-floating > .form-control:disabled ~ label {
+  color: #6c757d;
+}
+.form-floating > :disabled ~ label::after,
+.form-floating > .form-control:disabled ~ label::after {
+  background-color: var(--bs-secondary-bg);
 }
 
 .input-group {
   position: relative;
   display: flex;
   flex-wrap: wrap;
   align-items: stretch;
@@ -2561,38 +2727,38 @@
 .input-group-text {
   display: flex;
   align-items: center;
   padding: 0.375rem 0.75rem;
   font-size: 1rem;
   font-weight: 400;
   line-height: 1.5;
-  color: #212529;
+  color: var(--bs-body-color);
   text-align: center;
   white-space: nowrap;
-  background-color: #e9ecef;
-  border: 1px solid #ced4da;
-  border-radius: 0.375rem;
+  background-color: var(--bs-tertiary-bg);
+  border: var(--bs-border-width) solid var(--bs-border-color);
+  border-radius: var(--bs-border-radius);
 }
 
 .input-group-lg > .form-control,
 .input-group-lg > .form-select,
 .input-group-lg > .input-group-text,
 .input-group-lg > .btn {
   padding: 0.5rem 1rem;
   font-size: 1.25rem;
-  border-radius: 0.5rem;
+  border-radius: var(--bs-border-radius-lg);
 }
 
 .input-group-sm > .form-control,
 .input-group-sm > .form-select,
 .input-group-sm > .input-group-text,
 .input-group-sm > .btn {
   padding: 0.25rem 0.5rem;
   font-size: 0.875rem;
-  border-radius: 0.25rem;
+  border-radius: var(--bs-border-radius-sm);
 }
 
 .input-group-lg > .form-select,
 .input-group-sm > .form-select {
   padding-right: 3rem;
 }
 
@@ -2607,100 +2773,100 @@
 .input-group.has-validation > .dropdown-toggle:nth-last-child(n+4),
 .input-group.has-validation > .form-floating:nth-last-child(n+3) > .form-control,
 .input-group.has-validation > .form-floating:nth-last-child(n+3) > .form-select {
   border-top-right-radius: 0;
   border-bottom-right-radius: 0;
 }
 .input-group > :not(:first-child):not(.dropdown-menu):not(.valid-tooltip):not(.valid-feedback):not(.invalid-tooltip):not(.invalid-feedback) {
-  margin-left: -1px;
+  margin-left: calc(var(--bs-border-width) * -1);
   border-top-left-radius: 0;
   border-bottom-left-radius: 0;
 }
 .input-group > .form-floating:not(:first-child) > .form-control,
 .input-group > .form-floating:not(:first-child) > .form-select {
   border-top-left-radius: 0;
   border-bottom-left-radius: 0;
 }
 
 .valid-feedback {
   display: none;
   width: 100%;
   margin-top: 0.25rem;
   font-size: 0.875em;
-  color: #198754;
+  color: var(--bs-form-valid-color);
 }
 
 .valid-tooltip {
   position: absolute;
   top: 100%;
   z-index: 5;
   display: none;
   max-width: 100%;
   padding: 0.25rem 0.5rem;
   margin-top: 0.1rem;
   font-size: 0.875rem;
   color: #fff;
-  background-color: rgba(25, 135, 84, 0.9);
-  border-radius: 0.375rem;
+  background-color: var(--bs-success);
+  border-radius: var(--bs-border-radius);
 }
 
 .was-validated :valid ~ .valid-feedback,
 .was-validated :valid ~ .valid-tooltip,
 .is-valid ~ .valid-feedback,
 .is-valid ~ .valid-tooltip {
   display: block;
 }
 
 .was-validated .form-control:valid, .form-control.is-valid {
-  border-color: #198754;
+  border-color: var(--bs-form-valid-border-color);
   padding-right: calc(1.5em + 0.75rem);
   background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 8 8'%3e%3cpath fill='%23198754' d='M2.3 6.73.6 4.53c-.4-1.04.46-1.4 1.1-.8l1.1 1.4 3.4-3.8c.6-.63 1.6-.27 1.2.7l-4 4.6c-.43.5-.8.4-1.1.1z'/%3e%3c/svg%3e");
   background-repeat: no-repeat;
   background-position: right calc(0.375em + 0.1875rem) center;
   background-size: calc(0.75em + 0.375rem) calc(0.75em + 0.375rem);
 }
 .was-validated .form-control:valid:focus, .form-control.is-valid:focus {
-  border-color: #198754;
-  box-shadow: 0 0 0 0.25rem rgba(25, 135, 84, 0.25);
+  border-color: var(--bs-form-valid-border-color);
+  box-shadow: 0 0 0 0.25rem rgba(var(--bs-success-rgb), 0.25);
 }
 
 .was-validated textarea.form-control:valid, textarea.form-control.is-valid {
   padding-right: calc(1.5em + 0.75rem);
   background-position: top calc(0.375em + 0.1875rem) right calc(0.375em + 0.1875rem);
 }
 
 .was-validated .form-select:valid, .form-select.is-valid {
-  border-color: #198754;
+  border-color: var(--bs-form-valid-border-color);
 }
 .was-validated .form-select:valid:not([multiple]):not([size]), .was-validated .form-select:valid:not([multiple])[size="1"], .form-select.is-valid:not([multiple]):not([size]), .form-select.is-valid:not([multiple])[size="1"] {
+  --bs-form-select-bg-icon: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 8 8'%3e%3cpath fill='%23198754' d='M2.3 6.73.6 4.53c-.4-1.04.46-1.4 1.1-.8l1.1 1.4 3.4-3.8c.6-.63 1.6-.27 1.2.7l-4 4.6c-.43.5-.8.4-1.1.1z'/%3e%3c/svg%3e");
   padding-right: 4.125rem;
-  background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill='none' stroke='%23343a40' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='m2 5 6 6 6-6'/%3e%3c/svg%3e"), url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 8 8'%3e%3cpath fill='%23198754' d='M2.3 6.73.6 4.53c-.4-1.04.46-1.4 1.1-.8l1.1 1.4 3.4-3.8c.6-.63 1.6-.27 1.2.7l-4 4.6c-.43.5-.8.4-1.1.1z'/%3e%3c/svg%3e");
   background-position: right 0.75rem center, center right 2.25rem;
   background-size: 16px 12px, calc(0.75em + 0.375rem) calc(0.75em + 0.375rem);
 }
 .was-validated .form-select:valid:focus, .form-select.is-valid:focus {
-  border-color: #198754;
-  box-shadow: 0 0 0 0.25rem rgba(25, 135, 84, 0.25);
+  border-color: var(--bs-form-valid-border-color);
+  box-shadow: 0 0 0 0.25rem rgba(var(--bs-success-rgb), 0.25);
 }
 
 .was-validated .form-control-color:valid, .form-control-color.is-valid {
   width: calc(3rem + calc(1.5em + 0.75rem));
 }
 
 .was-validated .form-check-input:valid, .form-check-input.is-valid {
-  border-color: #198754;
+  border-color: var(--bs-form-valid-border-color);
 }
 .was-validated .form-check-input:valid:checked, .form-check-input.is-valid:checked {
-  background-color: #198754;
+  background-color: var(--bs-form-valid-color);
 }
 .was-validated .form-check-input:valid:focus, .form-check-input.is-valid:focus {
-  box-shadow: 0 0 0 0.25rem rgba(25, 135, 84, 0.25);
+  box-shadow: 0 0 0 0.25rem rgba(var(--bs-success-rgb), 0.25);
 }
 .was-validated .form-check-input:valid ~ .form-check-label, .form-check-input.is-valid ~ .form-check-label {
-  color: #198754;
+  color: var(--bs-form-valid-color);
 }
 
 .form-check-inline .form-check-input ~ .valid-feedback {
   margin-left: 0.5em;
 }
 
 .was-validated .input-group > .form-control:not(:focus):valid, .input-group > .form-control:not(:focus).is-valid,
@@ -2712,85 +2878,85 @@
 }
 
 .invalid-feedback {
   display: none;
   width: 100%;
   margin-top: 0.25rem;
   font-size: 0.875em;
-  color: #dc3545;
+  color: var(--bs-form-invalid-color);
 }
 
 .invalid-tooltip {
   position: absolute;
   top: 100%;
   z-index: 5;
   display: none;
   max-width: 100%;
   padding: 0.25rem 0.5rem;
   margin-top: 0.1rem;
   font-size: 0.875rem;
   color: #fff;
-  background-color: rgba(220, 53, 69, 0.9);
-  border-radius: 0.375rem;
+  background-color: var(--bs-danger);
+  border-radius: var(--bs-border-radius);
 }
 
 .was-validated :invalid ~ .invalid-feedback,
 .was-validated :invalid ~ .invalid-tooltip,
 .is-invalid ~ .invalid-feedback,
 .is-invalid ~ .invalid-tooltip {
   display: block;
 }
 
 .was-validated .form-control:invalid, .form-control.is-invalid {
-  border-color: #dc3545;
+  border-color: var(--bs-form-invalid-border-color);
   padding-right: calc(1.5em + 0.75rem);
   background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 12 12' width='12' height='12' fill='none' stroke='%23dc3545'%3e%3ccircle cx='6' cy='6' r='4.5'/%3e%3cpath stroke-linejoin='round' d='M5.8 3.6h.4L6 6.5z'/%3e%3ccircle cx='6' cy='8.2' r='.6' fill='%23dc3545' stroke='none'/%3e%3c/svg%3e");
   background-repeat: no-repeat;
   background-position: right calc(0.375em + 0.1875rem) center;
   background-size: calc(0.75em + 0.375rem) calc(0.75em + 0.375rem);
 }
 .was-validated .form-control:invalid:focus, .form-control.is-invalid:focus {
-  border-color: #dc3545;
-  box-shadow: 0 0 0 0.25rem rgba(220, 53, 69, 0.25);
+  border-color: var(--bs-form-invalid-border-color);
+  box-shadow: 0 0 0 0.25rem rgba(var(--bs-danger-rgb), 0.25);
 }
 
 .was-validated textarea.form-control:invalid, textarea.form-control.is-invalid {
   padding-right: calc(1.5em + 0.75rem);
   background-position: top calc(0.375em + 0.1875rem) right calc(0.375em + 0.1875rem);
 }
 
 .was-validated .form-select:invalid, .form-select.is-invalid {
-  border-color: #dc3545;
+  border-color: var(--bs-form-invalid-border-color);
 }
 .was-validated .form-select:invalid:not([multiple]):not([size]), .was-validated .form-select:invalid:not([multiple])[size="1"], .form-select.is-invalid:not([multiple]):not([size]), .form-select.is-invalid:not([multiple])[size="1"] {
+  --bs-form-select-bg-icon: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 12 12' width='12' height='12' fill='none' stroke='%23dc3545'%3e%3ccircle cx='6' cy='6' r='4.5'/%3e%3cpath stroke-linejoin='round' d='M5.8 3.6h.4L6 6.5z'/%3e%3ccircle cx='6' cy='8.2' r='.6' fill='%23dc3545' stroke='none'/%3e%3c/svg%3e");
   padding-right: 4.125rem;
-  background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill='none' stroke='%23343a40' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='m2 5 6 6 6-6'/%3e%3c/svg%3e"), url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 12 12' width='12' height='12' fill='none' stroke='%23dc3545'%3e%3ccircle cx='6' cy='6' r='4.5'/%3e%3cpath stroke-linejoin='round' d='M5.8 3.6h.4L6 6.5z'/%3e%3ccircle cx='6' cy='8.2' r='.6' fill='%23dc3545' stroke='none'/%3e%3c/svg%3e");
   background-position: right 0.75rem center, center right 2.25rem;
   background-size: 16px 12px, calc(0.75em + 0.375rem) calc(0.75em + 0.375rem);
 }
 .was-validated .form-select:invalid:focus, .form-select.is-invalid:focus {
-  border-color: #dc3545;
-  box-shadow: 0 0 0 0.25rem rgba(220, 53, 69, 0.25);
+  border-color: var(--bs-form-invalid-border-color);
+  box-shadow: 0 0 0 0.25rem rgba(var(--bs-danger-rgb), 0.25);
 }
 
 .was-validated .form-control-color:invalid, .form-control-color.is-invalid {
   width: calc(3rem + calc(1.5em + 0.75rem));
 }
 
 .was-validated .form-check-input:invalid, .form-check-input.is-invalid {
-  border-color: #dc3545;
+  border-color: var(--bs-form-invalid-border-color);
 }
 .was-validated .form-check-input:invalid:checked, .form-check-input.is-invalid:checked {
-  background-color: #dc3545;
+  background-color: var(--bs-form-invalid-color);
 }
 .was-validated .form-check-input:invalid:focus, .form-check-input.is-invalid:focus {
-  box-shadow: 0 0 0 0.25rem rgba(220, 53, 69, 0.25);
+  box-shadow: 0 0 0 0.25rem rgba(var(--bs-danger-rgb), 0.25);
 }
 .was-validated .form-check-input:invalid ~ .form-check-label, .form-check-input.is-invalid ~ .form-check-label {
-  color: #dc3545;
+  color: var(--bs-form-invalid-color);
 }
 
 .form-check-inline .form-check-input ~ .invalid-feedback {
   margin-left: 0.5em;
 }
 
 .was-validated .input-group > .form-control:not(:focus):invalid, .input-group > .form-control:not(:focus).is-invalid,
@@ -2804,19 +2970,19 @@
 .btn {
   --bs-btn-padding-x: 0.75rem;
   --bs-btn-padding-y: 0.375rem;
   --bs-btn-font-family: ;
   --bs-btn-font-size: 1rem;
   --bs-btn-font-weight: 400;
   --bs-btn-line-height: 1.5;
-  --bs-btn-color: #212529;
+  --bs-btn-color: var(--bs-body-color);
   --bs-btn-bg: transparent;
-  --bs-btn-border-width: 1px;
+  --bs-btn-border-width: var(--bs-border-width);
   --bs-btn-border-color: transparent;
-  --bs-btn-border-radius: 0.375rem;
+  --bs-btn-border-radius: var(--bs-border-radius);
   --bs-btn-hover-border-color: transparent;
   --bs-btn-box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.15), 0 1px 1px rgba(0, 0, 0, 0.075);
   --bs-btn-disabled-opacity: 0.65;
   --bs-btn-focus-box-shadow: 0 0 0 0.25rem rgba(var(--bs-btn-focus-shadow-rgb), .5);
   display: inline-block;
   padding: var(--bs-btn-padding-y) var(--bs-btn-padding-x);
   font-family: var(--bs-btn-font-family);
@@ -3158,37 +3324,37 @@
   --bs-btn-border-color: transparent;
   --bs-btn-hover-color: var(--bs-link-hover-color);
   --bs-btn-hover-border-color: transparent;
   --bs-btn-active-color: var(--bs-link-hover-color);
   --bs-btn-active-border-color: transparent;
   --bs-btn-disabled-color: #6c757d;
   --bs-btn-disabled-border-color: transparent;
-  --bs-btn-box-shadow: none;
+  --bs-btn-box-shadow: 0 0 0 #000;
   --bs-btn-focus-shadow-rgb: 49, 132, 253;
   text-decoration: underline;
 }
 .btn-link:focus-visible {
   color: var(--bs-btn-color);
 }
 .btn-link:hover {
   color: var(--bs-btn-hover-color);
 }
 
 .btn-lg, .btn-group-lg > .btn {
   --bs-btn-padding-y: 0.5rem;
   --bs-btn-padding-x: 1rem;
   --bs-btn-font-size: 1.25rem;
-  --bs-btn-border-radius: 0.5rem;
+  --bs-btn-border-radius: var(--bs-border-radius-lg);
 }
 
 .btn-sm, .btn-group-sm > .btn {
   --bs-btn-padding-y: 0.25rem;
   --bs-btn-padding-x: 0.5rem;
   --bs-btn-font-size: 0.875rem;
-  --bs-btn-border-radius: 0.25rem;
+  --bs-btn-border-radius: var(--bs-border-radius-sm);
 }
 
 .fade {
   transition: opacity 0.15s linear;
 }
 @media (prefers-reduced-motion: reduce) {
   .fade {
@@ -3253,29 +3419,29 @@
 .dropdown-menu {
   --bs-dropdown-zindex: 1000;
   --bs-dropdown-min-width: 10rem;
   --bs-dropdown-padding-x: 0;
   --bs-dropdown-padding-y: 0.5rem;
   --bs-dropdown-spacer: 0.125rem;
   --bs-dropdown-font-size: 1rem;
-  --bs-dropdown-color: #212529;
-  --bs-dropdown-bg: #fff;
+  --bs-dropdown-color: var(--bs-body-color);
+  --bs-dropdown-bg: var(--bs-body-bg);
   --bs-dropdown-border-color: var(--bs-border-color-translucent);
-  --bs-dropdown-border-radius: 0.375rem;
-  --bs-dropdown-border-width: 1px;
-  --bs-dropdown-inner-border-radius: calc(0.375rem - 1px);
+  --bs-dropdown-border-radius: var(--bs-border-radius);
+  --bs-dropdown-border-width: var(--bs-border-width);
+  --bs-dropdown-inner-border-radius: calc(var(--bs-border-radius) - var(--bs-border-width));
   --bs-dropdown-divider-bg: var(--bs-border-color-translucent);
   --bs-dropdown-divider-margin-y: 0.5rem;
   --bs-dropdown-box-shadow: 0 0.5rem 1rem rgba(0, 0, 0, 0.15);
-  --bs-dropdown-link-color: #212529;
-  --bs-dropdown-link-hover-color: #1e2125;
-  --bs-dropdown-link-hover-bg: #e9ecef;
+  --bs-dropdown-link-color: var(--bs-body-color);
+  --bs-dropdown-link-hover-color: var(--bs-body-color);
+  --bs-dropdown-link-hover-bg: var(--bs-tertiary-bg);
   --bs-dropdown-link-active-color: #fff;
   --bs-dropdown-link-active-bg: #0d6efd;
-  --bs-dropdown-link-disabled-color: #adb5bd;
+  --bs-dropdown-link-disabled-color: var(--bs-tertiary-color);
   --bs-dropdown-item-padding-x: 1rem;
   --bs-dropdown-item-padding-y: 0.25rem;
   --bs-dropdown-header-color: #6c757d;
   --bs-dropdown-header-padding-x: 1rem;
   --bs-dropdown-header-padding-y: 0.5rem;
   position: absolute;
   z-index: var(--bs-dropdown-zindex);
@@ -3486,14 +3652,15 @@
   font-weight: 400;
   color: var(--bs-dropdown-link-color);
   text-align: inherit;
   text-decoration: none;
   white-space: nowrap;
   background-color: transparent;
   border: 0;
+  border-radius: var(--bs-dropdown-item-border-radius, 0);
 }
 .dropdown-item:hover, .dropdown-item:focus {
   color: var(--bs-dropdown-link-hover-color);
   background-color: var(--bs-dropdown-link-hover-bg);
 }
 .dropdown-item.active, .dropdown-item:active {
   color: var(--bs-dropdown-link-active-color);
@@ -3572,19 +3739,19 @@
   justify-content: flex-start;
 }
 .btn-toolbar .input-group {
   width: auto;
 }
 
 .btn-group {
-  border-radius: 0.375rem;
+  border-radius: var(--bs-border-radius);
 }
 .btn-group > :not(.btn-check:first-child) + .btn,
 .btn-group > .btn-group:not(:first-child) {
-  margin-left: -1px;
+  margin-left: calc(var(--bs-border-width) * -1);
 }
 .btn-group > .btn:not(:last-child):not(.dropdown-toggle),
 .btn-group > .btn.dropdown-toggle-split:first-child,
 .btn-group > .btn-group:not(:last-child) > .btn {
   border-top-right-radius: 0;
   border-bottom-right-radius: 0;
 }
@@ -3623,15 +3790,15 @@
 }
 .btn-group-vertical > .btn,
 .btn-group-vertical > .btn-group {
   width: 100%;
 }
 .btn-group-vertical > .btn:not(:first-child),
 .btn-group-vertical > .btn-group:not(:first-child) {
-  margin-top: -1px;
+  margin-top: calc(var(--bs-border-width) * -1);
 }
 .btn-group-vertical > .btn:not(:last-child):not(.dropdown-toggle),
 .btn-group-vertical > .btn-group:not(:last-child) > .btn {
   border-bottom-right-radius: 0;
   border-bottom-left-radius: 0;
 }
 .btn-group-vertical > .btn ~ .btn,
@@ -3642,104 +3809,118 @@
 
 .nav {
   --bs-nav-link-padding-x: 1rem;
   --bs-nav-link-padding-y: 0.5rem;
   --bs-nav-link-font-weight: ;
   --bs-nav-link-color: var(--bs-link-color);
   --bs-nav-link-hover-color: var(--bs-link-hover-color);
-  --bs-nav-link-disabled-color: #6c757d;
+  --bs-nav-link-disabled-color: var(--bs-secondary-color);
   display: flex;
   flex-wrap: wrap;
   padding-left: 0;
   margin-bottom: 0;
   list-style: none;
 }
 
 .nav-link {
   display: block;
   padding: var(--bs-nav-link-padding-y) var(--bs-nav-link-padding-x);
   font-size: var(--bs-nav-link-font-size);
   font-weight: var(--bs-nav-link-font-weight);
   color: var(--bs-nav-link-color);
   text-decoration: none;
+  background: none;
+  border: 0;
   transition: color 0.15s ease-in-out, background-color 0.15s ease-in-out, border-color 0.15s ease-in-out;
 }
 @media (prefers-reduced-motion: reduce) {
   .nav-link {
     transition: none;
   }
 }
 .nav-link:hover, .nav-link:focus {
   color: var(--bs-nav-link-hover-color);
 }
-.nav-link.disabled {
+.nav-link:focus-visible {
+  outline: 0;
+  box-shadow: 0 0 0 0.25rem rgba(13, 110, 253, 0.25);
+}
+.nav-link.disabled, .nav-link:disabled {
   color: var(--bs-nav-link-disabled-color);
   pointer-events: none;
   cursor: default;
 }
 
 .nav-tabs {
-  --bs-nav-tabs-border-width: 1px;
-  --bs-nav-tabs-border-color: #dee2e6;
-  --bs-nav-tabs-border-radius: 0.375rem;
-  --bs-nav-tabs-link-hover-border-color: #e9ecef #e9ecef #dee2e6;
-  --bs-nav-tabs-link-active-color: #495057;
-  --bs-nav-tabs-link-active-bg: #fff;
-  --bs-nav-tabs-link-active-border-color: #dee2e6 #dee2e6 #fff;
+  --bs-nav-tabs-border-width: var(--bs-border-width);
+  --bs-nav-tabs-border-color: var(--bs-border-color);
+  --bs-nav-tabs-border-radius: var(--bs-border-radius);
+  --bs-nav-tabs-link-hover-border-color: var(--bs-secondary-bg) var(--bs-secondary-bg) var(--bs-border-color);
+  --bs-nav-tabs-link-active-color: var(--bs-emphasis-color);
+  --bs-nav-tabs-link-active-bg: var(--bs-body-bg);
+  --bs-nav-tabs-link-active-border-color: var(--bs-border-color) var(--bs-border-color) var(--bs-body-bg);
   border-bottom: var(--bs-nav-tabs-border-width) solid var(--bs-nav-tabs-border-color);
 }
 .nav-tabs .nav-link {
   margin-bottom: calc(-1 * var(--bs-nav-tabs-border-width));
-  background: none;
   border: var(--bs-nav-tabs-border-width) solid transparent;
   border-top-left-radius: var(--bs-nav-tabs-border-radius);
   border-top-right-radius: var(--bs-nav-tabs-border-radius);
 }
 .nav-tabs .nav-link:hover, .nav-tabs .nav-link:focus {
   isolation: isolate;
   border-color: var(--bs-nav-tabs-link-hover-border-color);
 }
-.nav-tabs .nav-link.disabled, .nav-tabs .nav-link:disabled {
-  color: var(--bs-nav-link-disabled-color);
-  background-color: transparent;
-  border-color: transparent;
-}
 .nav-tabs .nav-link.active,
 .nav-tabs .nav-item.show .nav-link {
   color: var(--bs-nav-tabs-link-active-color);
   background-color: var(--bs-nav-tabs-link-active-bg);
   border-color: var(--bs-nav-tabs-link-active-border-color);
 }
 .nav-tabs .dropdown-menu {
   margin-top: calc(-1 * var(--bs-nav-tabs-border-width));
   border-top-left-radius: 0;
   border-top-right-radius: 0;
 }
 
 .nav-pills {
-  --bs-nav-pills-border-radius: 0.375rem;
+  --bs-nav-pills-border-radius: var(--bs-border-radius);
   --bs-nav-pills-link-active-color: #fff;
   --bs-nav-pills-link-active-bg: #0d6efd;
 }
 .nav-pills .nav-link {
-  background: none;
-  border: 0;
   border-radius: var(--bs-nav-pills-border-radius);
 }
-.nav-pills .nav-link:disabled {
-  color: var(--bs-nav-link-disabled-color);
-  background-color: transparent;
-  border-color: transparent;
-}
 .nav-pills .nav-link.active,
 .nav-pills .show > .nav-link {
   color: var(--bs-nav-pills-link-active-color);
   background-color: var(--bs-nav-pills-link-active-bg);
 }
 
+.nav-underline {
+  --bs-nav-underline-gap: 1rem;
+  --bs-nav-underline-border-width: 0.125rem;
+  --bs-nav-underline-link-active-color: var(--bs-emphasis-color);
+  gap: var(--bs-nav-underline-gap);
+}
+.nav-underline .nav-link {
+  padding-right: 0;
+  padding-left: 0;
+  border-bottom: var(--bs-nav-underline-border-width) solid transparent;
+}
+.nav-underline .nav-link:hover, .nav-underline .nav-link:focus {
+  border-bottom-color: currentcolor;
+}
+.nav-underline .nav-link.active,
+.nav-underline .show > .nav-link {
+  font-weight: 700;
+  color: var(--bs-nav-underline-link-active-color);
+  border-bottom-color: currentcolor;
+}
+
 .nav-fill > .nav-link,
 .nav-fill .nav-item {
   flex: 1 1 auto;
   text-align: center;
 }
 
 .nav-justified > .nav-link,
@@ -3760,30 +3941,30 @@
 .tab-content > .active {
   display: block;
 }
 
 .navbar {
   --bs-navbar-padding-x: 0;
   --bs-navbar-padding-y: 0.5rem;
-  --bs-navbar-color: rgba(0, 0, 0, 0.55);
-  --bs-navbar-hover-color: rgba(0, 0, 0, 0.7);
-  --bs-navbar-disabled-color: rgba(0, 0, 0, 0.3);
-  --bs-navbar-active-color: rgba(0, 0, 0, 0.9);
+  --bs-navbar-color: rgba(var(--bs-emphasis-color-rgb), 0.65);
+  --bs-navbar-hover-color: rgba(var(--bs-emphasis-color-rgb), 0.8);
+  --bs-navbar-disabled-color: rgba(var(--bs-emphasis-color-rgb), 0.3);
+  --bs-navbar-active-color: rgba(var(--bs-emphasis-color-rgb), 1);
   --bs-navbar-brand-padding-y: 0.3125rem;
   --bs-navbar-brand-margin-end: 1rem;
   --bs-navbar-brand-font-size: 1.25rem;
-  --bs-navbar-brand-color: rgba(0, 0, 0, 0.9);
-  --bs-navbar-brand-hover-color: rgba(0, 0, 0, 0.9);
+  --bs-navbar-brand-color: rgba(var(--bs-emphasis-color-rgb), 1);
+  --bs-navbar-brand-hover-color: rgba(var(--bs-emphasis-color-rgb), 1);
   --bs-navbar-nav-link-padding-x: 0.5rem;
   --bs-navbar-toggler-padding-y: 0.25rem;
   --bs-navbar-toggler-padding-x: 0.75rem;
   --bs-navbar-toggler-font-size: 1.25rem;
-  --bs-navbar-toggler-icon-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 30 30'%3e%3cpath stroke='rgba%280, 0, 0, 0.55%29' stroke-linecap='round' stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/%3e%3c/svg%3e");
-  --bs-navbar-toggler-border-color: rgba(0, 0, 0, 0.1);
-  --bs-navbar-toggler-border-radius: 0.375rem;
+  --bs-navbar-toggler-icon-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 30 30'%3e%3cpath stroke='rgba%2833, 37, 41, 0.75%29' stroke-linecap='round' stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/%3e%3c/svg%3e");
+  --bs-navbar-toggler-border-color: rgba(var(--bs-emphasis-color-rgb), 0.15);
+  --bs-navbar-toggler-border-radius: var(--bs-border-radius);
   --bs-navbar-toggler-focus-width: 0.25rem;
   --bs-navbar-toggler-transition: box-shadow 0.15s ease-in-out;
   position: relative;
   display: flex;
   flex-wrap: wrap;
   align-items: center;
   justify-content: space-between;
@@ -3823,16 +4004,15 @@
   --bs-nav-link-disabled-color: var(--bs-navbar-disabled-color);
   display: flex;
   flex-direction: column;
   padding-left: 0;
   margin-bottom: 0;
   list-style: none;
 }
-.navbar-nav .show > .nav-link,
-.navbar-nav .nav-link.active {
+.navbar-nav .nav-link.active, .navbar-nav .nav-link.show {
   color: var(--bs-navbar-active-color);
 }
 .navbar-nav .dropdown-menu {
   position: static;
 }
 
 .navbar-text {
@@ -4169,48 +4349,56 @@
 .navbar-expand .offcanvas .offcanvas-body {
   display: flex;
   flex-grow: 0;
   padding: 0;
   overflow-y: visible;
 }
 
-.navbar-dark {
+.navbar-dark,
+.navbar[data-bs-theme=dark] {
   --bs-navbar-color: rgba(255, 255, 255, 0.55);
   --bs-navbar-hover-color: rgba(255, 255, 255, 0.75);
   --bs-navbar-disabled-color: rgba(255, 255, 255, 0.25);
   --bs-navbar-active-color: #fff;
   --bs-navbar-brand-color: #fff;
   --bs-navbar-brand-hover-color: #fff;
   --bs-navbar-toggler-border-color: rgba(255, 255, 255, 0.1);
   --bs-navbar-toggler-icon-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 30 30'%3e%3cpath stroke='rgba%28255, 255, 255, 0.55%29' stroke-linecap='round' stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/%3e%3c/svg%3e");
 }
 
+[data-bs-theme=dark] .navbar-toggler-icon {
+  --bs-navbar-toggler-icon-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 30 30'%3e%3cpath stroke='rgba%28255, 255, 255, 0.55%29' stroke-linecap='round' stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/%3e%3c/svg%3e");
+}
+
 .card {
   --bs-card-spacer-y: 1rem;
   --bs-card-spacer-x: 1rem;
   --bs-card-title-spacer-y: 0.5rem;
-  --bs-card-border-width: 1px;
+  --bs-card-title-color: ;
+  --bs-card-subtitle-color: ;
+  --bs-card-border-width: var(--bs-border-width);
   --bs-card-border-color: var(--bs-border-color-translucent);
-  --bs-card-border-radius: 0.375rem;
+  --bs-card-border-radius: var(--bs-border-radius);
   --bs-card-box-shadow: ;
-  --bs-card-inner-border-radius: calc(0.375rem - 1px);
+  --bs-card-inner-border-radius: calc(var(--bs-border-radius) - (var(--bs-border-width)));
   --bs-card-cap-padding-y: 0.5rem;
   --bs-card-cap-padding-x: 1rem;
-  --bs-card-cap-bg: rgba(0, 0, 0, 0.03);
+  --bs-card-cap-bg: rgba(var(--bs-body-color-rgb), 0.03);
   --bs-card-cap-color: ;
   --bs-card-height: ;
   --bs-card-color: ;
-  --bs-card-bg: #fff;
+  --bs-card-bg: var(--bs-body-bg);
   --bs-card-img-overlay-padding: 1rem;
   --bs-card-group-margin: 0.75rem;
   position: relative;
   display: flex;
   flex-direction: column;
   min-width: 0;
   height: var(--bs-card-height);
+  color: var(--bs-body-color);
   word-wrap: break-word;
   background-color: var(--bs-card-bg);
   background-clip: border-box;
   border: var(--bs-card-border-width) solid var(--bs-card-border-color);
   border-radius: var(--bs-card-border-radius);
 }
 .card > hr {
@@ -4240,19 +4428,21 @@
   flex: 1 1 auto;
   padding: var(--bs-card-spacer-y) var(--bs-card-spacer-x);
   color: var(--bs-card-color);
 }
 
 .card-title {
   margin-bottom: var(--bs-card-title-spacer-y);
+  color: var(--bs-card-title-color);
 }
 
 .card-subtitle {
   margin-top: calc(-0.5 * var(--bs-card-title-spacer-y));
   margin-bottom: 0;
+  color: var(--bs-card-subtitle-color);
 }
 
 .card-text:last-child {
   margin-bottom: 0;
 }
 
 .card-link + .card-link {
@@ -4341,58 +4531,58 @@
     border-left: 0;
   }
   .card-group > .card:not(:last-child) {
     border-top-right-radius: 0;
     border-bottom-right-radius: 0;
   }
   .card-group > .card:not(:last-child) .card-img-top,
-.card-group > .card:not(:last-child) .card-header {
+  .card-group > .card:not(:last-child) .card-header {
     border-top-right-radius: 0;
   }
   .card-group > .card:not(:last-child) .card-img-bottom,
-.card-group > .card:not(:last-child) .card-footer {
+  .card-group > .card:not(:last-child) .card-footer {
     border-bottom-right-radius: 0;
   }
   .card-group > .card:not(:first-child) {
     border-top-left-radius: 0;
     border-bottom-left-radius: 0;
   }
   .card-group > .card:not(:first-child) .card-img-top,
-.card-group > .card:not(:first-child) .card-header {
+  .card-group > .card:not(:first-child) .card-header {
     border-top-left-radius: 0;
   }
   .card-group > .card:not(:first-child) .card-img-bottom,
-.card-group > .card:not(:first-child) .card-footer {
+  .card-group > .card:not(:first-child) .card-footer {
     border-bottom-left-radius: 0;
   }
 }
 
 .accordion {
-  --bs-accordion-color: #212529;
-  --bs-accordion-bg: #fff;
+  --bs-accordion-color: var(--bs-body-color);
+  --bs-accordion-bg: var(--bs-body-bg);
   --bs-accordion-transition: color 0.15s ease-in-out, background-color 0.15s ease-in-out, border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out, border-radius 0.15s ease;
   --bs-accordion-border-color: var(--bs-border-color);
-  --bs-accordion-border-width: 1px;
-  --bs-accordion-border-radius: 0.375rem;
-  --bs-accordion-inner-border-radius: calc(0.375rem - 1px);
+  --bs-accordion-border-width: var(--bs-border-width);
+  --bs-accordion-border-radius: var(--bs-border-radius);
+  --bs-accordion-inner-border-radius: calc(var(--bs-border-radius) - (var(--bs-border-width)));
   --bs-accordion-btn-padding-x: 1.25rem;
   --bs-accordion-btn-padding-y: 1rem;
-  --bs-accordion-btn-color: #212529;
+  --bs-accordion-btn-color: var(--bs-body-color);
   --bs-accordion-btn-bg: var(--bs-accordion-bg);
   --bs-accordion-btn-icon: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%23212529'%3e%3cpath fill-rule='evenodd' d='M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z'/%3e%3c/svg%3e");
   --bs-accordion-btn-icon-width: 1.25rem;
   --bs-accordion-btn-icon-transform: rotate(-180deg);
   --bs-accordion-btn-icon-transition: transform 0.2s ease-in-out;
-  --bs-accordion-btn-active-icon: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%230c63e4'%3e%3cpath fill-rule='evenodd' d='M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z'/%3e%3c/svg%3e");
+  --bs-accordion-btn-active-icon: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%23052c65'%3e%3cpath fill-rule='evenodd' d='M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z'/%3e%3c/svg%3e");
   --bs-accordion-btn-focus-border-color: #86b7fe;
   --bs-accordion-btn-focus-box-shadow: 0 0 0 0.25rem rgba(13, 110, 253, 0.25);
   --bs-accordion-body-padding-x: 1.25rem;
   --bs-accordion-body-padding-y: 1rem;
-  --bs-accordion-active-color: #0c63e4;
-  --bs-accordion-active-bg: #e7f1ff;
+  --bs-accordion-active-color: var(--bs-primary-text-emphasis);
+  --bs-accordion-active-bg: var(--bs-primary-bg-subtle);
 }
 
 .accordion-button {
   position: relative;
   display: flex;
   align-items: center;
   width: 100%;
@@ -4497,23 +4687,28 @@
 .accordion-flush .accordion-item:last-child {
   border-bottom: 0;
 }
 .accordion-flush .accordion-item .accordion-button, .accordion-flush .accordion-item .accordion-button.collapsed {
   border-radius: 0;
 }
 
+[data-bs-theme=dark] .accordion-button::after {
+  --bs-accordion-btn-icon: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%236ea8fe'%3e%3cpath fill-rule='evenodd' d='M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z'/%3e%3c/svg%3e");
+  --bs-accordion-btn-active-icon: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%236ea8fe'%3e%3cpath fill-rule='evenodd' d='M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z'/%3e%3c/svg%3e");
+}
+
 .breadcrumb {
   --bs-breadcrumb-padding-x: 0;
   --bs-breadcrumb-padding-y: 0;
   --bs-breadcrumb-margin-bottom: 1rem;
   --bs-breadcrumb-bg: ;
   --bs-breadcrumb-border-radius: ;
-  --bs-breadcrumb-divider-color: #6c757d;
+  --bs-breadcrumb-divider-color: var(--bs-secondary-color);
   --bs-breadcrumb-item-padding-x: 0.5rem;
-  --bs-breadcrumb-item-active-color: #6c757d;
+  --bs-breadcrumb-item-active-color: var(--bs-secondary-color);
   display: flex;
   flex-wrap: wrap;
   padding: var(--bs-breadcrumb-padding-y) var(--bs-breadcrumb-padding-x);
   margin-bottom: var(--bs-breadcrumb-margin-bottom);
   font-size: var(--bs-breadcrumb-font-size);
   list-style: none;
   background-color: var(--bs-breadcrumb-bg);
@@ -4534,30 +4729,30 @@
 }
 
 .pagination {
   --bs-pagination-padding-x: 0.75rem;
   --bs-pagination-padding-y: 0.375rem;
   --bs-pagination-font-size: 1rem;
   --bs-pagination-color: var(--bs-link-color);
-  --bs-pagination-bg: #fff;
-  --bs-pagination-border-width: 1px;
-  --bs-pagination-border-color: #dee2e6;
-  --bs-pagination-border-radius: 0.375rem;
+  --bs-pagination-bg: var(--bs-body-bg);
+  --bs-pagination-border-width: var(--bs-border-width);
+  --bs-pagination-border-color: var(--bs-border-color);
+  --bs-pagination-border-radius: var(--bs-border-radius);
   --bs-pagination-hover-color: var(--bs-link-hover-color);
-  --bs-pagination-hover-bg: #e9ecef;
-  --bs-pagination-hover-border-color: #dee2e6;
+  --bs-pagination-hover-bg: var(--bs-tertiary-bg);
+  --bs-pagination-hover-border-color: var(--bs-border-color);
   --bs-pagination-focus-color: var(--bs-link-hover-color);
-  --bs-pagination-focus-bg: #e9ecef;
+  --bs-pagination-focus-bg: var(--bs-secondary-bg);
   --bs-pagination-focus-box-shadow: 0 0 0 0.25rem rgba(13, 110, 253, 0.25);
   --bs-pagination-active-color: #fff;
   --bs-pagination-active-bg: #0d6efd;
   --bs-pagination-active-border-color: #0d6efd;
-  --bs-pagination-disabled-color: #6c757d;
-  --bs-pagination-disabled-bg: #fff;
-  --bs-pagination-disabled-border-color: #dee2e6;
+  --bs-pagination-disabled-color: var(--bs-secondary-color);
+  --bs-pagination-disabled-bg: var(--bs-secondary-bg);
+  --bs-pagination-disabled-border-color: var(--bs-border-color);
   display: flex;
   padding-left: 0;
   list-style: none;
 }
 
 .page-link {
   position: relative;
@@ -4598,46 +4793,46 @@
   color: var(--bs-pagination-disabled-color);
   pointer-events: none;
   background-color: var(--bs-pagination-disabled-bg);
   border-color: var(--bs-pagination-disabled-border-color);
 }
 
 .page-item:not(:first-child) .page-link {
-  margin-left: -1px;
+  margin-left: calc(var(--bs-border-width) * -1);
 }
 .page-item:first-child .page-link {
   border-top-left-radius: var(--bs-pagination-border-radius);
   border-bottom-left-radius: var(--bs-pagination-border-radius);
 }
 .page-item:last-child .page-link {
   border-top-right-radius: var(--bs-pagination-border-radius);
   border-bottom-right-radius: var(--bs-pagination-border-radius);
 }
 
 .pagination-lg {
   --bs-pagination-padding-x: 1.5rem;
   --bs-pagination-padding-y: 0.75rem;
   --bs-pagination-font-size: 1.25rem;
-  --bs-pagination-border-radius: 0.5rem;
+  --bs-pagination-border-radius: var(--bs-border-radius-lg);
 }
 
 .pagination-sm {
   --bs-pagination-padding-x: 0.5rem;
   --bs-pagination-padding-y: 0.25rem;
   --bs-pagination-font-size: 0.875rem;
-  --bs-pagination-border-radius: 0.25rem;
+  --bs-pagination-border-radius: var(--bs-border-radius-sm);
 }
 
 .badge {
   --bs-badge-padding-x: 0.65em;
   --bs-badge-padding-y: 0.35em;
   --bs-badge-font-size: 0.75em;
   --bs-badge-font-weight: 700;
   --bs-badge-color: #fff;
-  --bs-badge-border-radius: 0.375rem;
+  --bs-badge-border-radius: var(--bs-border-radius);
   display: inline-block;
   padding: var(--bs-badge-padding-y) var(--bs-badge-padding-x);
   font-size: var(--bs-badge-font-size);
   font-weight: var(--bs-badge-font-weight);
   line-height: 1;
   color: var(--bs-badge-color);
   text-align: center;
@@ -4657,16 +4852,17 @@
 .alert {
   --bs-alert-bg: transparent;
   --bs-alert-padding-x: 1rem;
   --bs-alert-padding-y: 1rem;
   --bs-alert-margin-bottom: 1rem;
   --bs-alert-color: inherit;
   --bs-alert-border-color: transparent;
-  --bs-alert-border: 1px solid var(--bs-alert-border-color);
-  --bs-alert-border-radius: 0.375rem;
+  --bs-alert-border: var(--bs-border-width) solid var(--bs-alert-border-color);
+  --bs-alert-border-radius: var(--bs-border-radius);
+  --bs-alert-link-color: inherit;
   position: relative;
   padding: var(--bs-alert-padding-y) var(--bs-alert-padding-x);
   margin-bottom: var(--bs-alert-margin-bottom);
   color: var(--bs-alert-color);
   background-color: var(--bs-alert-bg);
   border: var(--bs-alert-border);
   border-radius: var(--bs-alert-border-radius);
@@ -4674,110 +4870,96 @@
 
 .alert-heading {
   color: inherit;
 }
 
 .alert-link {
   font-weight: 700;
+  color: var(--bs-alert-link-color);
 }
 
 .alert-dismissible {
   padding-right: 3rem;
 }
 .alert-dismissible .btn-close {
   position: absolute;
   top: 0;
   right: 0;
   z-index: 2;
   padding: 1.25rem 1rem;
 }
 
 .alert-primary {
-  --bs-alert-color: #084298;
-  --bs-alert-bg: #cfe2ff;
-  --bs-alert-border-color: #b6d4fe;
-}
-.alert-primary .alert-link {
-  color: #06357a;
+  --bs-alert-color: var(--bs-primary-text-emphasis);
+  --bs-alert-bg: var(--bs-primary-bg-subtle);
+  --bs-alert-border-color: var(--bs-primary-border-subtle);
+  --bs-alert-link-color: var(--bs-primary-text-emphasis);
 }
 
 .alert-secondary {
-  --bs-alert-color: #41464b;
-  --bs-alert-bg: #e2e3e5;
-  --bs-alert-border-color: #d3d6d8;
-}
-.alert-secondary .alert-link {
-  color: #34383c;
+  --bs-alert-color: var(--bs-secondary-text-emphasis);
+  --bs-alert-bg: var(--bs-secondary-bg-subtle);
+  --bs-alert-border-color: var(--bs-secondary-border-subtle);
+  --bs-alert-link-color: var(--bs-secondary-text-emphasis);
 }
 
 .alert-success {
-  --bs-alert-color: #0f5132;
-  --bs-alert-bg: #d1e7dd;
-  --bs-alert-border-color: #badbcc;
-}
-.alert-success .alert-link {
-  color: #0c4128;
+  --bs-alert-color: var(--bs-success-text-emphasis);
+  --bs-alert-bg: var(--bs-success-bg-subtle);
+  --bs-alert-border-color: var(--bs-success-border-subtle);
+  --bs-alert-link-color: var(--bs-success-text-emphasis);
 }
 
 .alert-info {
-  --bs-alert-color: #055160;
-  --bs-alert-bg: #cff4fc;
-  --bs-alert-border-color: #b6effb;
-}
-.alert-info .alert-link {
-  color: #04414d;
+  --bs-alert-color: var(--bs-info-text-emphasis);
+  --bs-alert-bg: var(--bs-info-bg-subtle);
+  --bs-alert-border-color: var(--bs-info-border-subtle);
+  --bs-alert-link-color: var(--bs-info-text-emphasis);
 }
 
 .alert-warning {
-  --bs-alert-color: #664d03;
-  --bs-alert-bg: #fff3cd;
-  --bs-alert-border-color: #ffecb5;
-}
-.alert-warning .alert-link {
-  color: #523e02;
+  --bs-alert-color: var(--bs-warning-text-emphasis);
+  --bs-alert-bg: var(--bs-warning-bg-subtle);
+  --bs-alert-border-color: var(--bs-warning-border-subtle);
+  --bs-alert-link-color: var(--bs-warning-text-emphasis);
 }
 
 .alert-danger {
-  --bs-alert-color: #842029;
-  --bs-alert-bg: #f8d7da;
-  --bs-alert-border-color: #f5c2c7;
-}
-.alert-danger .alert-link {
-  color: #6a1a21;
+  --bs-alert-color: var(--bs-danger-text-emphasis);
+  --bs-alert-bg: var(--bs-danger-bg-subtle);
+  --bs-alert-border-color: var(--bs-danger-border-subtle);
+  --bs-alert-link-color: var(--bs-danger-text-emphasis);
 }
 
 .alert-light {
-  --bs-alert-color: #636464;
-  --bs-alert-bg: #fefefe;
-  --bs-alert-border-color: #fdfdfe;
-}
-.alert-light .alert-link {
-  color: #4f5050;
+  --bs-alert-color: var(--bs-light-text-emphasis);
+  --bs-alert-bg: var(--bs-light-bg-subtle);
+  --bs-alert-border-color: var(--bs-light-border-subtle);
+  --bs-alert-link-color: var(--bs-light-text-emphasis);
 }
 
 .alert-dark {
-  --bs-alert-color: #141619;
-  --bs-alert-bg: #d3d3d4;
-  --bs-alert-border-color: #bcbebf;
-}
-.alert-dark .alert-link {
-  color: #101214;
+  --bs-alert-color: var(--bs-dark-text-emphasis);
+  --bs-alert-bg: var(--bs-dark-bg-subtle);
+  --bs-alert-border-color: var(--bs-dark-border-subtle);
+  --bs-alert-link-color: var(--bs-dark-text-emphasis);
 }
 
 @keyframes progress-bar-stripes {
   0% {
     background-position-x: 1rem;
   }
 }
-.progress {
+.progress,
+.progress-stacked {
   --bs-progress-height: 1rem;
   --bs-progress-font-size: 0.75rem;
-  --bs-progress-bg: #e9ecef;
-  --bs-progress-border-radius: 0.375rem;
-  --bs-progress-box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.075);
+  --bs-progress-bg: var(--bs-secondary-bg);
+  --bs-progress-border-radius: var(--bs-border-radius);
+  --bs-progress-box-shadow: var(--bs-box-shadow-inset);
   --bs-progress-bar-color: #fff;
   --bs-progress-bar-bg: #0d6efd;
   --bs-progress-bar-transition: width 0.6s ease;
   display: flex;
   height: var(--bs-progress-height);
   overflow: hidden;
   font-size: var(--bs-progress-font-size);
@@ -4803,38 +4985,46 @@
 }
 
 .progress-bar-striped {
   background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
   background-size: var(--bs-progress-height) var(--bs-progress-height);
 }
 
+.progress-stacked > .progress {
+  overflow: visible;
+}
+
+.progress-stacked > .progress > .progress-bar {
+  width: 100%;
+}
+
 .progress-bar-animated {
   animation: 1s linear infinite progress-bar-stripes;
 }
 @media (prefers-reduced-motion: reduce) {
   .progress-bar-animated {
     animation: none;
   }
 }
 
 .list-group {
-  --bs-list-group-color: #212529;
-  --bs-list-group-bg: #fff;
-  --bs-list-group-border-color: rgba(0, 0, 0, 0.125);
-  --bs-list-group-border-width: 1px;
-  --bs-list-group-border-radius: 0.375rem;
+  --bs-list-group-color: var(--bs-body-color);
+  --bs-list-group-bg: var(--bs-body-bg);
+  --bs-list-group-border-color: var(--bs-border-color);
+  --bs-list-group-border-width: var(--bs-border-width);
+  --bs-list-group-border-radius: var(--bs-border-radius);
   --bs-list-group-item-padding-x: 1rem;
   --bs-list-group-item-padding-y: 0.5rem;
-  --bs-list-group-action-color: #495057;
-  --bs-list-group-action-hover-color: #495057;
-  --bs-list-group-action-hover-bg: #f8f9fa;
-  --bs-list-group-action-active-color: #212529;
-  --bs-list-group-action-active-bg: #e9ecef;
-  --bs-list-group-disabled-color: #6c757d;
-  --bs-list-group-disabled-bg: #fff;
+  --bs-list-group-action-color: var(--bs-secondary-color);
+  --bs-list-group-action-hover-color: var(--bs-emphasis-color);
+  --bs-list-group-action-hover-bg: var(--bs-tertiary-bg);
+  --bs-list-group-action-active-color: var(--bs-body-color);
+  --bs-list-group-action-active-bg: var(--bs-secondary-bg);
+  --bs-list-group-disabled-color: var(--bs-secondary-color);
+  --bs-list-group-disabled-bg: var(--bs-body-bg);
   --bs-list-group-active-color: #fff;
   --bs-list-group-active-bg: #0d6efd;
   --bs-list-group-active-border-color: #0d6efd;
   display: flex;
   flex-direction: column;
   padding-left: 0;
   margin-bottom: 0;
@@ -5052,174 +5242,178 @@
   border-width: 0 0 var(--bs-list-group-border-width);
 }
 .list-group-flush > .list-group-item:last-child {
   border-bottom-width: 0;
 }
 
 .list-group-item-primary {
-  color: #084298;
-  background-color: #cfe2ff;
-}
-.list-group-item-primary.list-group-item-action:hover, .list-group-item-primary.list-group-item-action:focus {
-  color: #084298;
-  background-color: #bacbe6;
-}
-.list-group-item-primary.list-group-item-action.active {
-  color: #fff;
-  background-color: #084298;
-  border-color: #084298;
+  --bs-list-group-color: var(--bs-primary-text-emphasis);
+  --bs-list-group-bg: var(--bs-primary-bg-subtle);
+  --bs-list-group-border-color: var(--bs-primary-border-subtle);
+  --bs-list-group-action-hover-color: var(--bs-emphasis-color);
+  --bs-list-group-action-hover-bg: var(--bs-primary-border-subtle);
+  --bs-list-group-action-active-color: var(--bs-emphasis-color);
+  --bs-list-group-action-active-bg: var(--bs-primary-border-subtle);
+  --bs-list-group-active-color: var(--bs-primary-bg-subtle);
+  --bs-list-group-active-bg: var(--bs-primary-text-emphasis);
+  --bs-list-group-active-border-color: var(--bs-primary-text-emphasis);
 }
 
 .list-group-item-secondary {
-  color: #41464b;
-  background-color: #e2e3e5;
-}
-.list-group-item-secondary.list-group-item-action:hover, .list-group-item-secondary.list-group-item-action:focus {
-  color: #41464b;
-  background-color: #cbccce;
-}
-.list-group-item-secondary.list-group-item-action.active {
-  color: #fff;
-  background-color: #41464b;
-  border-color: #41464b;
+  --bs-list-group-color: var(--bs-secondary-text-emphasis);
+  --bs-list-group-bg: var(--bs-secondary-bg-subtle);
+  --bs-list-group-border-color: var(--bs-secondary-border-subtle);
+  --bs-list-group-action-hover-color: var(--bs-emphasis-color);
+  --bs-list-group-action-hover-bg: var(--bs-secondary-border-subtle);
+  --bs-list-group-action-active-color: var(--bs-emphasis-color);
+  --bs-list-group-action-active-bg: var(--bs-secondary-border-subtle);
+  --bs-list-group-active-color: var(--bs-secondary-bg-subtle);
+  --bs-list-group-active-bg: var(--bs-secondary-text-emphasis);
+  --bs-list-group-active-border-color: var(--bs-secondary-text-emphasis);
 }
 
 .list-group-item-success {
-  color: #0f5132;
-  background-color: #d1e7dd;
-}
-.list-group-item-success.list-group-item-action:hover, .list-group-item-success.list-group-item-action:focus {
-  color: #0f5132;
-  background-color: #bcd0c7;
-}
-.list-group-item-success.list-group-item-action.active {
-  color: #fff;
-  background-color: #0f5132;
-  border-color: #0f5132;
+  --bs-list-group-color: var(--bs-success-text-emphasis);
+  --bs-list-group-bg: var(--bs-success-bg-subtle);
+  --bs-list-group-border-color: var(--bs-success-border-subtle);
+  --bs-list-group-action-hover-color: var(--bs-emphasis-color);
+  --bs-list-group-action-hover-bg: var(--bs-success-border-subtle);
+  --bs-list-group-action-active-color: var(--bs-emphasis-color);
+  --bs-list-group-action-active-bg: var(--bs-success-border-subtle);
+  --bs-list-group-active-color: var(--bs-success-bg-subtle);
+  --bs-list-group-active-bg: var(--bs-success-text-emphasis);
+  --bs-list-group-active-border-color: var(--bs-success-text-emphasis);
 }
 
 .list-group-item-info {
-  color: #055160;
-  background-color: #cff4fc;
-}
-.list-group-item-info.list-group-item-action:hover, .list-group-item-info.list-group-item-action:focus {
-  color: #055160;
-  background-color: #badce3;
-}
-.list-group-item-info.list-group-item-action.active {
-  color: #fff;
-  background-color: #055160;
-  border-color: #055160;
+  --bs-list-group-color: var(--bs-info-text-emphasis);
+  --bs-list-group-bg: var(--bs-info-bg-subtle);
+  --bs-list-group-border-color: var(--bs-info-border-subtle);
+  --bs-list-group-action-hover-color: var(--bs-emphasis-color);
+  --bs-list-group-action-hover-bg: var(--bs-info-border-subtle);
+  --bs-list-group-action-active-color: var(--bs-emphasis-color);
+  --bs-list-group-action-active-bg: var(--bs-info-border-subtle);
+  --bs-list-group-active-color: var(--bs-info-bg-subtle);
+  --bs-list-group-active-bg: var(--bs-info-text-emphasis);
+  --bs-list-group-active-border-color: var(--bs-info-text-emphasis);
 }
 
 .list-group-item-warning {
-  color: #664d03;
-  background-color: #fff3cd;
-}
-.list-group-item-warning.list-group-item-action:hover, .list-group-item-warning.list-group-item-action:focus {
-  color: #664d03;
-  background-color: #e6dbb9;
-}
-.list-group-item-warning.list-group-item-action.active {
-  color: #fff;
-  background-color: #664d03;
-  border-color: #664d03;
+  --bs-list-group-color: var(--bs-warning-text-emphasis);
+  --bs-list-group-bg: var(--bs-warning-bg-subtle);
+  --bs-list-group-border-color: var(--bs-warning-border-subtle);
+  --bs-list-group-action-hover-color: var(--bs-emphasis-color);
+  --bs-list-group-action-hover-bg: var(--bs-warning-border-subtle);
+  --bs-list-group-action-active-color: var(--bs-emphasis-color);
+  --bs-list-group-action-active-bg: var(--bs-warning-border-subtle);
+  --bs-list-group-active-color: var(--bs-warning-bg-subtle);
+  --bs-list-group-active-bg: var(--bs-warning-text-emphasis);
+  --bs-list-group-active-border-color: var(--bs-warning-text-emphasis);
 }
 
 .list-group-item-danger {
-  color: #842029;
-  background-color: #f8d7da;
-}
-.list-group-item-danger.list-group-item-action:hover, .list-group-item-danger.list-group-item-action:focus {
-  color: #842029;
-  background-color: #dfc2c4;
-}
-.list-group-item-danger.list-group-item-action.active {
-  color: #fff;
-  background-color: #842029;
-  border-color: #842029;
+  --bs-list-group-color: var(--bs-danger-text-emphasis);
+  --bs-list-group-bg: var(--bs-danger-bg-subtle);
+  --bs-list-group-border-color: var(--bs-danger-border-subtle);
+  --bs-list-group-action-hover-color: var(--bs-emphasis-color);
+  --bs-list-group-action-hover-bg: var(--bs-danger-border-subtle);
+  --bs-list-group-action-active-color: var(--bs-emphasis-color);
+  --bs-list-group-action-active-bg: var(--bs-danger-border-subtle);
+  --bs-list-group-active-color: var(--bs-danger-bg-subtle);
+  --bs-list-group-active-bg: var(--bs-danger-text-emphasis);
+  --bs-list-group-active-border-color: var(--bs-danger-text-emphasis);
 }
 
 .list-group-item-light {
-  color: #636464;
-  background-color: #fefefe;
-}
-.list-group-item-light.list-group-item-action:hover, .list-group-item-light.list-group-item-action:focus {
-  color: #636464;
-  background-color: #e5e5e5;
-}
-.list-group-item-light.list-group-item-action.active {
-  color: #fff;
-  background-color: #636464;
-  border-color: #636464;
+  --bs-list-group-color: var(--bs-light-text-emphasis);
+  --bs-list-group-bg: var(--bs-light-bg-subtle);
+  --bs-list-group-border-color: var(--bs-light-border-subtle);
+  --bs-list-group-action-hover-color: var(--bs-emphasis-color);
+  --bs-list-group-action-hover-bg: var(--bs-light-border-subtle);
+  --bs-list-group-action-active-color: var(--bs-emphasis-color);
+  --bs-list-group-action-active-bg: var(--bs-light-border-subtle);
+  --bs-list-group-active-color: var(--bs-light-bg-subtle);
+  --bs-list-group-active-bg: var(--bs-light-text-emphasis);
+  --bs-list-group-active-border-color: var(--bs-light-text-emphasis);
 }
 
 .list-group-item-dark {
-  color: #141619;
-  background-color: #d3d3d4;
-}
-.list-group-item-dark.list-group-item-action:hover, .list-group-item-dark.list-group-item-action:focus {
-  color: #141619;
-  background-color: #bebebf;
-}
-.list-group-item-dark.list-group-item-action.active {
-  color: #fff;
-  background-color: #141619;
-  border-color: #141619;
+  --bs-list-group-color: var(--bs-dark-text-emphasis);
+  --bs-list-group-bg: var(--bs-dark-bg-subtle);
+  --bs-list-group-border-color: var(--bs-dark-border-subtle);
+  --bs-list-group-action-hover-color: var(--bs-emphasis-color);
+  --bs-list-group-action-hover-bg: var(--bs-dark-border-subtle);
+  --bs-list-group-action-active-color: var(--bs-emphasis-color);
+  --bs-list-group-action-active-bg: var(--bs-dark-border-subtle);
+  --bs-list-group-active-color: var(--bs-dark-bg-subtle);
+  --bs-list-group-active-bg: var(--bs-dark-text-emphasis);
+  --bs-list-group-active-border-color: var(--bs-dark-text-emphasis);
 }
 
 .btn-close {
+  --bs-btn-close-color: #000;
+  --bs-btn-close-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%23000'%3e%3cpath d='M.293.293a1 1 0 0 1 1.414 0L8 6.586 14.293.293a1 1 0 1 1 1.414 1.414L9.414 8l6.293 6.293a1 1 0 0 1-1.414 1.414L8 9.414l-6.293 6.293a1 1 0 0 1-1.414-1.414L6.586 8 .293 1.707a1 1 0 0 1 0-1.414z'/%3e%3c/svg%3e");
+  --bs-btn-close-opacity: 0.5;
+  --bs-btn-close-hover-opacity: 0.75;
+  --bs-btn-close-focus-shadow: 0 0 0 0.25rem rgba(13, 110, 253, 0.25);
+  --bs-btn-close-focus-opacity: 1;
+  --bs-btn-close-disabled-opacity: 0.25;
+  --bs-btn-close-white-filter: invert(1) grayscale(100%) brightness(200%);
   box-sizing: content-box;
   width: 1em;
   height: 1em;
   padding: 0.25em 0.25em;
-  color: #000;
-  background: transparent url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%23000'%3e%3cpath d='M.293.293a1 1 0 0 1 1.414 0L8 6.586 14.293.293a1 1 0 1 1 1.414 1.414L9.414 8l6.293 6.293a1 1 0 0 1-1.414 1.414L8 9.414l-6.293 6.293a1 1 0 0 1-1.414-1.414L6.586 8 .293 1.707a1 1 0 0 1 0-1.414z'/%3e%3c/svg%3e") center/1em auto no-repeat;
+  color: var(--bs-btn-close-color);
+  background: transparent var(--bs-btn-close-bg) center/1em auto no-repeat;
   border: 0;
   border-radius: 0.375rem;
-  opacity: 0.5;
+  opacity: var(--bs-btn-close-opacity);
 }
 .btn-close:hover {
-  color: #000;
+  color: var(--bs-btn-close-color);
   text-decoration: none;
-  opacity: 0.75;
+  opacity: var(--bs-btn-close-hover-opacity);
 }
 .btn-close:focus {
   outline: 0;
-  box-shadow: 0 0 0 0.25rem rgba(13, 110, 253, 0.25);
-  opacity: 1;
+  box-shadow: var(--bs-btn-close-focus-shadow);
+  opacity: var(--bs-btn-close-focus-opacity);
 }
 .btn-close:disabled, .btn-close.disabled {
   pointer-events: none;
   -webkit-user-select: none;
   -moz-user-select: none;
   user-select: none;
-  opacity: 0.25;
+  opacity: var(--bs-btn-close-disabled-opacity);
 }
 
 .btn-close-white {
-  filter: invert(1) grayscale(100%) brightness(200%);
+  filter: var(--bs-btn-close-white-filter);
+}
+
+[data-bs-theme=dark] .btn-close {
+  filter: var(--bs-btn-close-white-filter);
 }
 
 .toast {
   --bs-toast-zindex: 1090;
   --bs-toast-padding-x: 0.75rem;
   --bs-toast-padding-y: 0.5rem;
   --bs-toast-spacing: 1.5rem;
   --bs-toast-max-width: 350px;
   --bs-toast-font-size: 0.875rem;
   --bs-toast-color: ;
-  --bs-toast-bg: rgba(255, 255, 255, 0.85);
-  --bs-toast-border-width: 1px;
+  --bs-toast-bg: rgba(var(--bs-body-bg-rgb), 0.85);
+  --bs-toast-border-width: var(--bs-border-width);
   --bs-toast-border-color: var(--bs-border-color-translucent);
-  --bs-toast-border-radius: 0.375rem;
-  --bs-toast-box-shadow: 0 0.5rem 1rem rgba(0, 0, 0, 0.15);
-  --bs-toast-header-color: #6c757d;
-  --bs-toast-header-bg: rgba(255, 255, 255, 0.85);
-  --bs-toast-header-border-color: rgba(0, 0, 0, 0.05);
+  --bs-toast-border-radius: var(--bs-border-radius);
+  --bs-toast-box-shadow: var(--bs-box-shadow);
+  --bs-toast-header-color: var(--bs-secondary-color);
+  --bs-toast-header-bg: rgba(var(--bs-body-bg-rgb), 0.85);
+  --bs-toast-header-border-color: var(--bs-border-color-translucent);
   width: var(--bs-toast-max-width);
   max-width: 100%;
   font-size: var(--bs-toast-font-size);
   color: var(--bs-toast-color);
   pointer-events: auto;
   background-color: var(--bs-toast-bg);
   background-clip: padding-box;
@@ -5271,30 +5465,30 @@
 
 .modal {
   --bs-modal-zindex: 1055;
   --bs-modal-width: 500px;
   --bs-modal-padding: 1rem;
   --bs-modal-margin: 0.5rem;
   --bs-modal-color: ;
-  --bs-modal-bg: #fff;
+  --bs-modal-bg: var(--bs-body-bg);
   --bs-modal-border-color: var(--bs-border-color-translucent);
-  --bs-modal-border-width: 1px;
-  --bs-modal-border-radius: 0.5rem;
+  --bs-modal-border-width: var(--bs-border-width);
+  --bs-modal-border-radius: var(--bs-border-radius-lg);
   --bs-modal-box-shadow: 0 0.125rem 0.25rem rgba(0, 0, 0, 0.075);
-  --bs-modal-inner-border-radius: calc(0.5rem - 1px);
+  --bs-modal-inner-border-radius: calc(var(--bs-border-radius-lg) - (var(--bs-border-width)));
   --bs-modal-header-padding-x: 1rem;
   --bs-modal-header-padding-y: 1rem;
   --bs-modal-header-padding: 1rem 1rem;
   --bs-modal-header-border-color: var(--bs-border-color);
-  --bs-modal-header-border-width: 1px;
+  --bs-modal-header-border-width: var(--bs-border-width);
   --bs-modal-title-line-height: 1.5;
   --bs-modal-footer-gap: 0.5rem;
   --bs-modal-footer-bg: ;
   --bs-modal-footer-border-color: var(--bs-border-color);
-  --bs-modal-footer-border-width: 1px;
+  --bs-modal-footer-border-width: var(--bs-border-width);
   position: fixed;
   top: 0;
   left: 0;
   z-index: var(--bs-modal-zindex);
   display: none;
   width: 100%;
   height: 100%;
@@ -5429,15 +5623,15 @@
   }
   .modal-sm {
     --bs-modal-width: 300px;
   }
 }
 @media (min-width: 992px) {
   .modal-lg,
-.modal-xl {
+  .modal-xl {
     --bs-modal-width: 800px;
   }
 }
 @media (min-width: 1200px) {
   .modal-xl {
     --bs-modal-width: 1140px;
   }
@@ -5470,15 +5664,15 @@
   }
   .modal-fullscreen-sm-down .modal-content {
     height: 100%;
     border: 0;
     border-radius: 0;
   }
   .modal-fullscreen-sm-down .modal-header,
-.modal-fullscreen-sm-down .modal-footer {
+  .modal-fullscreen-sm-down .modal-footer {
     border-radius: 0;
   }
   .modal-fullscreen-sm-down .modal-body {
     overflow-y: auto;
   }
 }
 @media (max-width: 767.98px) {
@@ -5490,15 +5684,15 @@
   }
   .modal-fullscreen-md-down .modal-content {
     height: 100%;
     border: 0;
     border-radius: 0;
   }
   .modal-fullscreen-md-down .modal-header,
-.modal-fullscreen-md-down .modal-footer {
+  .modal-fullscreen-md-down .modal-footer {
     border-radius: 0;
   }
   .modal-fullscreen-md-down .modal-body {
     overflow-y: auto;
   }
 }
 @media (max-width: 991.98px) {
@@ -5510,15 +5704,15 @@
   }
   .modal-fullscreen-lg-down .modal-content {
     height: 100%;
     border: 0;
     border-radius: 0;
   }
   .modal-fullscreen-lg-down .modal-header,
-.modal-fullscreen-lg-down .modal-footer {
+  .modal-fullscreen-lg-down .modal-footer {
     border-radius: 0;
   }
   .modal-fullscreen-lg-down .modal-body {
     overflow-y: auto;
   }
 }
 @media (max-width: 1199.98px) {
@@ -5530,15 +5724,15 @@
   }
   .modal-fullscreen-xl-down .modal-content {
     height: 100%;
     border: 0;
     border-radius: 0;
   }
   .modal-fullscreen-xl-down .modal-header,
-.modal-fullscreen-xl-down .modal-footer {
+  .modal-fullscreen-xl-down .modal-footer {
     border-radius: 0;
   }
   .modal-fullscreen-xl-down .modal-body {
     overflow-y: auto;
   }
 }
 @media (max-width: 1399.98px) {
@@ -5550,37 +5744,36 @@
   }
   .modal-fullscreen-xxl-down .modal-content {
     height: 100%;
     border: 0;
     border-radius: 0;
   }
   .modal-fullscreen-xxl-down .modal-header,
-.modal-fullscreen-xxl-down .modal-footer {
+  .modal-fullscreen-xxl-down .modal-footer {
     border-radius: 0;
   }
   .modal-fullscreen-xxl-down .modal-body {
     overflow-y: auto;
   }
 }
 .tooltip {
   --bs-tooltip-zindex: 1080;
   --bs-tooltip-max-width: 200px;
   --bs-tooltip-padding-x: 0.5rem;
   --bs-tooltip-padding-y: 0.25rem;
   --bs-tooltip-margin: ;
   --bs-tooltip-font-size: 0.875rem;
-  --bs-tooltip-color: #fff;
-  --bs-tooltip-bg: #000;
-  --bs-tooltip-border-radius: 0.375rem;
+  --bs-tooltip-color: var(--bs-body-bg);
+  --bs-tooltip-bg: var(--bs-emphasis-color);
+  --bs-tooltip-border-radius: var(--bs-border-radius);
   --bs-tooltip-opacity: 0.9;
   --bs-tooltip-arrow-width: 0.8rem;
   --bs-tooltip-arrow-height: 0.4rem;
   z-index: var(--bs-tooltip-zindex);
   display: block;
-  padding: var(--bs-tooltip-arrow-height);
   margin: var(--bs-tooltip-margin);
   font-family: var(--bs-font-sans-serif);
   font-style: normal;
   font-weight: 400;
   line-height: 1.5;
   text-align: left;
   text-align: start;
@@ -5608,47 +5801,47 @@
   position: absolute;
   content: "";
   border-color: transparent;
   border-style: solid;
 }
 
 .bs-tooltip-top .tooltip-arrow, .bs-tooltip-auto[data-popper-placement^=top] .tooltip-arrow {
-  bottom: 0;
+  bottom: calc(-1 * var(--bs-tooltip-arrow-height));
 }
 .bs-tooltip-top .tooltip-arrow::before, .bs-tooltip-auto[data-popper-placement^=top] .tooltip-arrow::before {
   top: -1px;
   border-width: var(--bs-tooltip-arrow-height) calc(var(--bs-tooltip-arrow-width) * 0.5) 0;
   border-top-color: var(--bs-tooltip-bg);
 }
 
 /* rtl:begin:ignore */
 .bs-tooltip-end .tooltip-arrow, .bs-tooltip-auto[data-popper-placement^=right] .tooltip-arrow {
-  left: 0;
+  left: calc(-1 * var(--bs-tooltip-arrow-height));
   width: var(--bs-tooltip-arrow-height);
   height: var(--bs-tooltip-arrow-width);
 }
 .bs-tooltip-end .tooltip-arrow::before, .bs-tooltip-auto[data-popper-placement^=right] .tooltip-arrow::before {
   right: -1px;
   border-width: calc(var(--bs-tooltip-arrow-width) * 0.5) var(--bs-tooltip-arrow-height) calc(var(--bs-tooltip-arrow-width) * 0.5) 0;
   border-right-color: var(--bs-tooltip-bg);
 }
 
 /* rtl:end:ignore */
 .bs-tooltip-bottom .tooltip-arrow, .bs-tooltip-auto[data-popper-placement^=bottom] .tooltip-arrow {
-  top: 0;
+  top: calc(-1 * var(--bs-tooltip-arrow-height));
 }
 .bs-tooltip-bottom .tooltip-arrow::before, .bs-tooltip-auto[data-popper-placement^=bottom] .tooltip-arrow::before {
   bottom: -1px;
   border-width: 0 calc(var(--bs-tooltip-arrow-width) * 0.5) var(--bs-tooltip-arrow-height);
   border-bottom-color: var(--bs-tooltip-bg);
 }
 
 /* rtl:begin:ignore */
 .bs-tooltip-start .tooltip-arrow, .bs-tooltip-auto[data-popper-placement^=left] .tooltip-arrow {
-  right: 0;
+  right: calc(-1 * var(--bs-tooltip-arrow-height));
   width: var(--bs-tooltip-arrow-height);
   height: var(--bs-tooltip-arrow-width);
 }
 .bs-tooltip-start .tooltip-arrow::before, .bs-tooltip-auto[data-popper-placement^=left] .tooltip-arrow::before {
   left: -1px;
   border-width: calc(var(--bs-tooltip-arrow-width) * 0.5) 0 calc(var(--bs-tooltip-arrow-width) * 0.5) var(--bs-tooltip-arrow-height);
   border-left-color: var(--bs-tooltip-bg);
@@ -5664,28 +5857,28 @@
   border-radius: var(--bs-tooltip-border-radius);
 }
 
 .popover {
   --bs-popover-zindex: 1070;
   --bs-popover-max-width: 276px;
   --bs-popover-font-size: 0.875rem;
-  --bs-popover-bg: #fff;
-  --bs-popover-border-width: 1px;
+  --bs-popover-bg: var(--bs-body-bg);
+  --bs-popover-border-width: var(--bs-border-width);
   --bs-popover-border-color: var(--bs-border-color-translucent);
-  --bs-popover-border-radius: 0.5rem;
-  --bs-popover-inner-border-radius: calc(0.5rem - 1px);
+  --bs-popover-border-radius: var(--bs-border-radius-lg);
+  --bs-popover-inner-border-radius: calc(var(--bs-border-radius-lg) - var(--bs-border-width));
   --bs-popover-box-shadow: 0 0.5rem 1rem rgba(0, 0, 0, 0.15);
   --bs-popover-header-padding-x: 1rem;
   --bs-popover-header-padding-y: 0.5rem;
   --bs-popover-header-font-size: 1rem;
-  --bs-popover-header-color: ;
-  --bs-popover-header-bg: #f0f0f0;
+  --bs-popover-header-color: inherit;
+  --bs-popover-header-bg: var(--bs-secondary-bg);
   --bs-popover-body-padding-x: 1rem;
   --bs-popover-body-padding-y: 1rem;
-  --bs-popover-body-color: #212529;
+  --bs-popover-body-color: var(--bs-body-color);
   --bs-popover-arrow-width: 1rem;
   --bs-popover-arrow-height: 0.5rem;
   --bs-popover-arrow-border: var(--bs-popover-border-color);
   z-index: var(--bs-popover-zindex);
   display: block;
   max-width: var(--bs-popover-max-width);
   font-family: var(--bs-font-sans-serif);
@@ -5886,15 +6079,15 @@
 .carousel-fade .active.carousel-item-end {
   z-index: 0;
   opacity: 0;
   transition: opacity 0s 0.6s;
 }
 @media (prefers-reduced-motion: reduce) {
   .carousel-fade .active.carousel-item-start,
-.carousel-fade .active.carousel-item-end {
+  .carousel-fade .active.carousel-item-end {
     transition: none;
   }
 }
 
 .carousel-control-prev,
 .carousel-control-next {
   position: absolute;
@@ -5911,15 +6104,15 @@
   background: none;
   border: 0;
   opacity: 0.5;
   transition: opacity 0.15s ease;
 }
 @media (prefers-reduced-motion: reduce) {
   .carousel-control-prev,
-.carousel-control-next {
+  .carousel-control-next {
     transition: none;
   }
 }
 .carousel-control-prev:hover, .carousel-control-prev:focus,
 .carousel-control-next:hover,
 .carousel-control-next:focus {
   color: #fff;
@@ -5970,15 +6163,14 @@
   z-index: 2;
   display: flex;
   justify-content: center;
   padding: 0;
   margin-right: 15%;
   margin-bottom: 1rem;
   margin-left: 15%;
-  list-style: none;
 }
 .carousel-indicators [data-bs-target] {
   box-sizing: content-box;
   flex: 0 1 auto;
   width: 30px;
   height: 3px;
   padding: 0;
@@ -6021,14 +6213,26 @@
 .carousel-dark .carousel-indicators [data-bs-target] {
   background-color: #000;
 }
 .carousel-dark .carousel-caption {
   color: #000;
 }
 
+[data-bs-theme=dark] .carousel .carousel-control-prev-icon,
+[data-bs-theme=dark] .carousel .carousel-control-next-icon, [data-bs-theme=dark].carousel .carousel-control-prev-icon,
+[data-bs-theme=dark].carousel .carousel-control-next-icon {
+  filter: invert(1) grayscale(100);
+}
+[data-bs-theme=dark] .carousel .carousel-indicators [data-bs-target], [data-bs-theme=dark].carousel .carousel-indicators [data-bs-target] {
+  background-color: #000;
+}
+[data-bs-theme=dark] .carousel .carousel-caption, [data-bs-theme=dark].carousel .carousel-caption {
+  color: #000;
+}
+
 .spinner-grow,
 .spinner-border {
   display: inline-block;
   width: var(--bs-spinner-width);
   height: var(--bs-spinner-height);
   vertical-align: var(--bs-spinner-vertical-align);
   border-radius: 50%;
@@ -6079,29 +6283,31 @@
 .spinner-grow-sm {
   --bs-spinner-width: 1rem;
   --bs-spinner-height: 1rem;
 }
 
 @media (prefers-reduced-motion: reduce) {
   .spinner-border,
-.spinner-grow {
+  .spinner-grow {
     --bs-spinner-animation-speed: 1.5s;
   }
 }
 .offcanvas, .offcanvas-xxl, .offcanvas-xl, .offcanvas-lg, .offcanvas-md, .offcanvas-sm {
   --bs-offcanvas-zindex: 1045;
   --bs-offcanvas-width: 400px;
   --bs-offcanvas-height: 30vh;
   --bs-offcanvas-padding-x: 1rem;
   --bs-offcanvas-padding-y: 1rem;
-  --bs-offcanvas-color: ;
-  --bs-offcanvas-bg: #fff;
-  --bs-offcanvas-border-width: 1px;
+  --bs-offcanvas-color: var(--bs-body-color);
+  --bs-offcanvas-bg: var(--bs-body-bg);
+  --bs-offcanvas-border-width: var(--bs-border-width);
   --bs-offcanvas-border-color: var(--bs-border-color-translucent);
   --bs-offcanvas-box-shadow: 0 0.125rem 0.25rem rgba(0, 0, 0, 0.075);
+  --bs-offcanvas-transition: transform 0.3s ease-in-out;
+  --bs-offcanvas-title-line-height: 1.5;
 }
 
 @media (max-width: 575.98px) {
   .offcanvas-sm {
     position: fixed;
     bottom: 0;
     z-index: var(--bs-offcanvas-zindex);
@@ -6109,15 +6315,15 @@
     flex-direction: column;
     max-width: 100%;
     color: var(--bs-offcanvas-color);
     visibility: hidden;
     background-color: var(--bs-offcanvas-bg);
     background-clip: padding-box;
     outline: 0;
-    transition: transform 0.3s ease-in-out;
+    transition: var(--bs-offcanvas-transition);
   }
 }
 @media (max-width: 575.98px) and (prefers-reduced-motion: reduce) {
   .offcanvas-sm {
     transition: none;
   }
 }
@@ -6125,51 +6331,41 @@
   .offcanvas-sm.offcanvas-start {
     top: 0;
     left: 0;
     width: var(--bs-offcanvas-width);
     border-right: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateX(-100%);
   }
-}
-@media (max-width: 575.98px) {
   .offcanvas-sm.offcanvas-end {
     top: 0;
     right: 0;
     width: var(--bs-offcanvas-width);
     border-left: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateX(100%);
   }
-}
-@media (max-width: 575.98px) {
   .offcanvas-sm.offcanvas-top {
     top: 0;
     right: 0;
     left: 0;
     height: var(--bs-offcanvas-height);
     max-height: 100%;
     border-bottom: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateY(-100%);
   }
-}
-@media (max-width: 575.98px) {
   .offcanvas-sm.offcanvas-bottom {
     right: 0;
     left: 0;
     height: var(--bs-offcanvas-height);
     max-height: 100%;
     border-top: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateY(100%);
   }
-}
-@media (max-width: 575.98px) {
   .offcanvas-sm.showing, .offcanvas-sm.show:not(.hiding) {
     transform: none;
   }
-}
-@media (max-width: 575.98px) {
   .offcanvas-sm.showing, .offcanvas-sm.hiding, .offcanvas-sm.show {
     visibility: visible;
   }
 }
 @media (min-width: 576px) {
   .offcanvas-sm {
     --bs-offcanvas-height: auto;
@@ -6197,15 +6393,15 @@
     flex-direction: column;
     max-width: 100%;
     color: var(--bs-offcanvas-color);
     visibility: hidden;
     background-color: var(--bs-offcanvas-bg);
     background-clip: padding-box;
     outline: 0;
-    transition: transform 0.3s ease-in-out;
+    transition: var(--bs-offcanvas-transition);
   }
 }
 @media (max-width: 767.98px) and (prefers-reduced-motion: reduce) {
   .offcanvas-md {
     transition: none;
   }
 }
@@ -6213,51 +6409,41 @@
   .offcanvas-md.offcanvas-start {
     top: 0;
     left: 0;
     width: var(--bs-offcanvas-width);
     border-right: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateX(-100%);
   }
-}
-@media (max-width: 767.98px) {
   .offcanvas-md.offcanvas-end {
     top: 0;
     right: 0;
     width: var(--bs-offcanvas-width);
     border-left: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateX(100%);
   }
-}
-@media (max-width: 767.98px) {
   .offcanvas-md.offcanvas-top {
     top: 0;
     right: 0;
     left: 0;
     height: var(--bs-offcanvas-height);
     max-height: 100%;
     border-bottom: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateY(-100%);
   }
-}
-@media (max-width: 767.98px) {
   .offcanvas-md.offcanvas-bottom {
     right: 0;
     left: 0;
     height: var(--bs-offcanvas-height);
     max-height: 100%;
     border-top: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateY(100%);
   }
-}
-@media (max-width: 767.98px) {
   .offcanvas-md.showing, .offcanvas-md.show:not(.hiding) {
     transform: none;
   }
-}
-@media (max-width: 767.98px) {
   .offcanvas-md.showing, .offcanvas-md.hiding, .offcanvas-md.show {
     visibility: visible;
   }
 }
 @media (min-width: 768px) {
   .offcanvas-md {
     --bs-offcanvas-height: auto;
@@ -6285,15 +6471,15 @@
     flex-direction: column;
     max-width: 100%;
     color: var(--bs-offcanvas-color);
     visibility: hidden;
     background-color: var(--bs-offcanvas-bg);
     background-clip: padding-box;
     outline: 0;
-    transition: transform 0.3s ease-in-out;
+    transition: var(--bs-offcanvas-transition);
   }
 }
 @media (max-width: 991.98px) and (prefers-reduced-motion: reduce) {
   .offcanvas-lg {
     transition: none;
   }
 }
@@ -6301,51 +6487,41 @@
   .offcanvas-lg.offcanvas-start {
     top: 0;
     left: 0;
     width: var(--bs-offcanvas-width);
     border-right: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateX(-100%);
   }
-}
-@media (max-width: 991.98px) {
   .offcanvas-lg.offcanvas-end {
     top: 0;
     right: 0;
     width: var(--bs-offcanvas-width);
     border-left: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateX(100%);
   }
-}
-@media (max-width: 991.98px) {
   .offcanvas-lg.offcanvas-top {
     top: 0;
     right: 0;
     left: 0;
     height: var(--bs-offcanvas-height);
     max-height: 100%;
     border-bottom: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateY(-100%);
   }
-}
-@media (max-width: 991.98px) {
   .offcanvas-lg.offcanvas-bottom {
     right: 0;
     left: 0;
     height: var(--bs-offcanvas-height);
     max-height: 100%;
     border-top: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateY(100%);
   }
-}
-@media (max-width: 991.98px) {
   .offcanvas-lg.showing, .offcanvas-lg.show:not(.hiding) {
     transform: none;
   }
-}
-@media (max-width: 991.98px) {
   .offcanvas-lg.showing, .offcanvas-lg.hiding, .offcanvas-lg.show {
     visibility: visible;
   }
 }
 @media (min-width: 992px) {
   .offcanvas-lg {
     --bs-offcanvas-height: auto;
@@ -6373,15 +6549,15 @@
     flex-direction: column;
     max-width: 100%;
     color: var(--bs-offcanvas-color);
     visibility: hidden;
     background-color: var(--bs-offcanvas-bg);
     background-clip: padding-box;
     outline: 0;
-    transition: transform 0.3s ease-in-out;
+    transition: var(--bs-offcanvas-transition);
   }
 }
 @media (max-width: 1199.98px) and (prefers-reduced-motion: reduce) {
   .offcanvas-xl {
     transition: none;
   }
 }
@@ -6389,51 +6565,41 @@
   .offcanvas-xl.offcanvas-start {
     top: 0;
     left: 0;
     width: var(--bs-offcanvas-width);
     border-right: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateX(-100%);
   }
-}
-@media (max-width: 1199.98px) {
   .offcanvas-xl.offcanvas-end {
     top: 0;
     right: 0;
     width: var(--bs-offcanvas-width);
     border-left: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateX(100%);
   }
-}
-@media (max-width: 1199.98px) {
   .offcanvas-xl.offcanvas-top {
     top: 0;
     right: 0;
     left: 0;
     height: var(--bs-offcanvas-height);
     max-height: 100%;
     border-bottom: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateY(-100%);
   }
-}
-@media (max-width: 1199.98px) {
   .offcanvas-xl.offcanvas-bottom {
     right: 0;
     left: 0;
     height: var(--bs-offcanvas-height);
     max-height: 100%;
     border-top: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateY(100%);
   }
-}
-@media (max-width: 1199.98px) {
   .offcanvas-xl.showing, .offcanvas-xl.show:not(.hiding) {
     transform: none;
   }
-}
-@media (max-width: 1199.98px) {
   .offcanvas-xl.showing, .offcanvas-xl.hiding, .offcanvas-xl.show {
     visibility: visible;
   }
 }
 @media (min-width: 1200px) {
   .offcanvas-xl {
     --bs-offcanvas-height: auto;
@@ -6461,15 +6627,15 @@
     flex-direction: column;
     max-width: 100%;
     color: var(--bs-offcanvas-color);
     visibility: hidden;
     background-color: var(--bs-offcanvas-bg);
     background-clip: padding-box;
     outline: 0;
-    transition: transform 0.3s ease-in-out;
+    transition: var(--bs-offcanvas-transition);
   }
 }
 @media (max-width: 1399.98px) and (prefers-reduced-motion: reduce) {
   .offcanvas-xxl {
     transition: none;
   }
 }
@@ -6477,51 +6643,41 @@
   .offcanvas-xxl.offcanvas-start {
     top: 0;
     left: 0;
     width: var(--bs-offcanvas-width);
     border-right: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateX(-100%);
   }
-}
-@media (max-width: 1399.98px) {
   .offcanvas-xxl.offcanvas-end {
     top: 0;
     right: 0;
     width: var(--bs-offcanvas-width);
     border-left: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateX(100%);
   }
-}
-@media (max-width: 1399.98px) {
   .offcanvas-xxl.offcanvas-top {
     top: 0;
     right: 0;
     left: 0;
     height: var(--bs-offcanvas-height);
     max-height: 100%;
     border-bottom: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateY(-100%);
   }
-}
-@media (max-width: 1399.98px) {
   .offcanvas-xxl.offcanvas-bottom {
     right: 0;
     left: 0;
     height: var(--bs-offcanvas-height);
     max-height: 100%;
     border-top: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateY(100%);
   }
-}
-@media (max-width: 1399.98px) {
   .offcanvas-xxl.showing, .offcanvas-xxl.show:not(.hiding) {
     transform: none;
   }
-}
-@media (max-width: 1399.98px) {
   .offcanvas-xxl.showing, .offcanvas-xxl.hiding, .offcanvas-xxl.show {
     visibility: visible;
   }
 }
 @media (min-width: 1400px) {
   .offcanvas-xxl {
     --bs-offcanvas-height: auto;
@@ -6548,15 +6704,15 @@
   flex-direction: column;
   max-width: 100%;
   color: var(--bs-offcanvas-color);
   visibility: hidden;
   background-color: var(--bs-offcanvas-bg);
   background-clip: padding-box;
   outline: 0;
-  transition: transform 0.3s ease-in-out;
+  transition: var(--bs-offcanvas-transition);
 }
 @media (prefers-reduced-motion: reduce) {
   .offcanvas {
     transition: none;
   }
 }
 .offcanvas.offcanvas-start {
@@ -6624,15 +6780,15 @@
   margin-top: calc(-0.5 * var(--bs-offcanvas-padding-y));
   margin-right: calc(-0.5 * var(--bs-offcanvas-padding-x));
   margin-bottom: calc(-0.5 * var(--bs-offcanvas-padding-y));
 }
 
 .offcanvas-title {
   margin-bottom: 0;
-  line-height: 1.5;
+  line-height: var(--bs-offcanvas-title-line-height);
 }
 
 .offcanvas-body {
   flex-grow: 1;
   padding: var(--bs-offcanvas-padding-y) var(--bs-offcanvas-padding-x);
   overflow-y: auto;
 }
@@ -6689,106 +6845,181 @@
   display: block;
   clear: both;
   content: "";
 }
 
 .text-bg-primary {
   color: #fff !important;
-  background-color: RGBA(13, 110, 253, var(--bs-bg-opacity, 1)) !important;
+  background-color: RGBA(var(--bs-primary-rgb), var(--bs-bg-opacity, 1)) !important;
 }
 
 .text-bg-secondary {
   color: #fff !important;
-  background-color: RGBA(108, 117, 125, var(--bs-bg-opacity, 1)) !important;
+  background-color: RGBA(var(--bs-secondary-rgb), var(--bs-bg-opacity, 1)) !important;
 }
 
 .text-bg-success {
   color: #fff !important;
-  background-color: RGBA(25, 135, 84, var(--bs-bg-opacity, 1)) !important;
+  background-color: RGBA(var(--bs-success-rgb), var(--bs-bg-opacity, 1)) !important;
 }
 
 .text-bg-info {
   color: #000 !important;
-  background-color: RGBA(13, 202, 240, var(--bs-bg-opacity, 1)) !important;
+  background-color: RGBA(var(--bs-info-rgb), var(--bs-bg-opacity, 1)) !important;
 }
 
 .text-bg-warning {
   color: #000 !important;
-  background-color: RGBA(255, 193, 7, var(--bs-bg-opacity, 1)) !important;
+  background-color: RGBA(var(--bs-warning-rgb), var(--bs-bg-opacity, 1)) !important;
 }
 
 .text-bg-danger {
   color: #fff !important;
-  background-color: RGBA(220, 53, 69, var(--bs-bg-opacity, 1)) !important;
+  background-color: RGBA(var(--bs-danger-rgb), var(--bs-bg-opacity, 1)) !important;
 }
 
 .text-bg-light {
   color: #000 !important;
-  background-color: RGBA(248, 249, 250, var(--bs-bg-opacity, 1)) !important;
+  background-color: RGBA(var(--bs-light-rgb), var(--bs-bg-opacity, 1)) !important;
 }
 
 .text-bg-dark {
   color: #fff !important;
-  background-color: RGBA(33, 37, 41, var(--bs-bg-opacity, 1)) !important;
+  background-color: RGBA(var(--bs-dark-rgb), var(--bs-bg-opacity, 1)) !important;
 }
 
 .link-primary {
-  color: #0d6efd !important;
+  color: RGBA(var(--bs-primary-rgb), var(--bs-link-opacity, 1)) !important;
+  -webkit-text-decoration-color: RGBA(var(--bs-primary-rgb), var(--bs-link-underline-opacity, 1)) !important;
+  text-decoration-color: RGBA(var(--bs-primary-rgb), var(--bs-link-underline-opacity, 1)) !important;
 }
 .link-primary:hover, .link-primary:focus {
-  color: #0a58ca !important;
+  color: RGBA(10, 88, 202, var(--bs-link-opacity, 1)) !important;
+  -webkit-text-decoration-color: RGBA(10, 88, 202, var(--bs-link-underline-opacity, 1)) !important;
+  text-decoration-color: RGBA(10, 88, 202, var(--bs-link-underline-opacity, 1)) !important;
 }
 
 .link-secondary {
-  color: #6c757d !important;
+  color: RGBA(var(--bs-secondary-rgb), var(--bs-link-opacity, 1)) !important;
+  -webkit-text-decoration-color: RGBA(var(--bs-secondary-rgb), var(--bs-link-underline-opacity, 1)) !important;
+  text-decoration-color: RGBA(var(--bs-secondary-rgb), var(--bs-link-underline-opacity, 1)) !important;
 }
 .link-secondary:hover, .link-secondary:focus {
-  color: #565e64 !important;
+  color: RGBA(86, 94, 100, var(--bs-link-opacity, 1)) !important;
+  -webkit-text-decoration-color: RGBA(86, 94, 100, var(--bs-link-underline-opacity, 1)) !important;
+  text-decoration-color: RGBA(86, 94, 100, var(--bs-link-underline-opacity, 1)) !important;
 }
 
 .link-success {
-  color: #198754 !important;
+  color: RGBA(var(--bs-success-rgb), var(--bs-link-opacity, 1)) !important;
+  -webkit-text-decoration-color: RGBA(var(--bs-success-rgb), var(--bs-link-underline-opacity, 1)) !important;
+  text-decoration-color: RGBA(var(--bs-success-rgb), var(--bs-link-underline-opacity, 1)) !important;
 }
 .link-success:hover, .link-success:focus {
-  color: #146c43 !important;
+  color: RGBA(20, 108, 67, var(--bs-link-opacity, 1)) !important;
+  -webkit-text-decoration-color: RGBA(20, 108, 67, var(--bs-link-underline-opacity, 1)) !important;
+  text-decoration-color: RGBA(20, 108, 67, var(--bs-link-underline-opacity, 1)) !important;
 }
 
 .link-info {
-  color: #0dcaf0 !important;
+  color: RGBA(var(--bs-info-rgb), var(--bs-link-opacity, 1)) !important;
+  -webkit-text-decoration-color: RGBA(var(--bs-info-rgb), var(--bs-link-underline-opacity, 1)) !important;
+  text-decoration-color: RGBA(var(--bs-info-rgb), var(--bs-link-underline-opacity, 1)) !important;
 }
 .link-info:hover, .link-info:focus {
-  color: #3dd5f3 !important;
+  color: RGBA(61, 213, 243, var(--bs-link-opacity, 1)) !important;
+  -webkit-text-decoration-color: RGBA(61, 213, 243, var(--bs-link-underline-opacity, 1)) !important;
+  text-decoration-color: RGBA(61, 213, 243, var(--bs-link-underline-opacity, 1)) !important;
 }
 
 .link-warning {
-  color: #ffc107 !important;
+  color: RGBA(var(--bs-warning-rgb), var(--bs-link-opacity, 1)) !important;
+  -webkit-text-decoration-color: RGBA(var(--bs-warning-rgb), var(--bs-link-underline-opacity, 1)) !important;
+  text-decoration-color: RGBA(var(--bs-warning-rgb), var(--bs-link-underline-opacity, 1)) !important;
 }
 .link-warning:hover, .link-warning:focus {
-  color: #ffcd39 !important;
+  color: RGBA(255, 205, 57, var(--bs-link-opacity, 1)) !important;
+  -webkit-text-decoration-color: RGBA(255, 205, 57, var(--bs-link-underline-opacity, 1)) !important;
+  text-decoration-color: RGBA(255, 205, 57, var(--bs-link-underline-opacity, 1)) !important;
 }
 
 .link-danger {
-  color: #dc3545 !important;
+  color: RGBA(var(--bs-danger-rgb), var(--bs-link-opacity, 1)) !important;
+  -webkit-text-decoration-color: RGBA(var(--bs-danger-rgb), var(--bs-link-underline-opacity, 1)) !important;
+  text-decoration-color: RGBA(var(--bs-danger-rgb), var(--bs-link-underline-opacity, 1)) !important;
 }
 .link-danger:hover, .link-danger:focus {
-  color: #b02a37 !important;
+  color: RGBA(176, 42, 55, var(--bs-link-opacity, 1)) !important;
+  -webkit-text-decoration-color: RGBA(176, 42, 55, var(--bs-link-underline-opacity, 1)) !important;
+  text-decoration-color: RGBA(176, 42, 55, var(--bs-link-underline-opacity, 1)) !important;
 }
 
 .link-light {
-  color: #f8f9fa !important;
+  color: RGBA(var(--bs-light-rgb), var(--bs-link-opacity, 1)) !important;
+  -webkit-text-decoration-color: RGBA(var(--bs-light-rgb), var(--bs-link-underline-opacity, 1)) !important;
+  text-decoration-color: RGBA(var(--bs-light-rgb), var(--bs-link-underline-opacity, 1)) !important;
 }
 .link-light:hover, .link-light:focus {
-  color: #f9fafb !important;
+  color: RGBA(249, 250, 251, var(--bs-link-opacity, 1)) !important;
+  -webkit-text-decoration-color: RGBA(249, 250, 251, var(--bs-link-underline-opacity, 1)) !important;
+  text-decoration-color: RGBA(249, 250, 251, var(--bs-link-underline-opacity, 1)) !important;
 }
 
 .link-dark {
-  color: #212529 !important;
+  color: RGBA(var(--bs-dark-rgb), var(--bs-link-opacity, 1)) !important;
+  -webkit-text-decoration-color: RGBA(var(--bs-dark-rgb), var(--bs-link-underline-opacity, 1)) !important;
+  text-decoration-color: RGBA(var(--bs-dark-rgb), var(--bs-link-underline-opacity, 1)) !important;
 }
 .link-dark:hover, .link-dark:focus {
-  color: #1a1e21 !important;
+  color: RGBA(26, 30, 33, var(--bs-link-opacity, 1)) !important;
+  -webkit-text-decoration-color: RGBA(26, 30, 33, var(--bs-link-underline-opacity, 1)) !important;
+  text-decoration-color: RGBA(26, 30, 33, var(--bs-link-underline-opacity, 1)) !important;
+}
+
+.link-body-emphasis {
+  color: RGBA(var(--bs-emphasis-color-rgb), var(--bs-link-opacity, 1)) !important;
+  -webkit-text-decoration-color: RGBA(var(--bs-emphasis-color-rgb), var(--bs-link-underline-opacity, 1)) !important;
+  text-decoration-color: RGBA(var(--bs-emphasis-color-rgb), var(--bs-link-underline-opacity, 1)) !important;
+}
+.link-body-emphasis:hover, .link-body-emphasis:focus {
+  color: RGBA(var(--bs-emphasis-color-rgb), var(--bs-link-opacity, 0.75)) !important;
+  -webkit-text-decoration-color: RGBA(var(--bs-emphasis-color-rgb), var(--bs-link-underline-opacity, 0.75)) !important;
+  text-decoration-color: RGBA(var(--bs-emphasis-color-rgb), var(--bs-link-underline-opacity, 0.75)) !important;
+}
+
+.focus-ring:focus {
+  outline: 0;
+  box-shadow: var(--bs-focus-ring-x, 0) var(--bs-focus-ring-y, 0) var(--bs-focus-ring-blur, 0) var(--bs-focus-ring-width) var(--bs-focus-ring-color);
+}
+
+.icon-link {
+  display: inline-flex;
+  gap: 0.375rem;
+  align-items: center;
+  -webkit-text-decoration-color: rgba(var(--bs-link-color-rgb), var(--bs-link-opacity, 0.5));
+  text-decoration-color: rgba(var(--bs-link-color-rgb), var(--bs-link-opacity, 0.5));
+  text-underline-offset: 0.25em;
+  -webkit-backface-visibility: hidden;
+  backface-visibility: hidden;
+}
+.icon-link > .bi {
+  flex-shrink: 0;
+  width: 1em;
+  height: 1em;
+  fill: currentcolor;
+  transition: 0.2s ease-in-out transform;
+}
+@media (prefers-reduced-motion: reduce) {
+  .icon-link > .bi {
+    transition: none;
+  }
+}
+
+.icon-link-hover:hover > .bi, .icon-link-hover:focus-visible > .bi {
+  transform: var(--bs-icon-link-transform, translate3d(0.25em, 0, 0));
 }
 
 .ratio {
   position: relative;
   width: 100%;
 }
 .ratio::before {
@@ -6932,24 +7163,27 @@
   flex: 1 1 auto;
   flex-direction: column;
   align-self: stretch;
 }
 
 .visually-hidden,
 .visually-hidden-focusable:not(:focus):not(:focus-within) {
-  position: absolute !important;
   width: 1px !important;
   height: 1px !important;
   padding: 0 !important;
   margin: -1px !important;
   overflow: hidden !important;
   clip: rect(0, 0, 0, 0) !important;
   white-space: nowrap !important;
   border: 0 !important;
 }
+.visually-hidden:not(caption),
+.visually-hidden-focusable:not(:focus):not(:focus-within):not(caption) {
+  position: absolute !important;
+}
 
 .stretched-link::after {
   position: absolute;
   top: 0;
   right: 0;
   bottom: 0;
   left: 0;
@@ -6962,15 +7196,15 @@
   text-overflow: ellipsis;
   white-space: nowrap;
 }
 
 .vr {
   display: inline-block;
   align-self: stretch;
-  width: 1px;
+  width: var(--bs-border-width);
   min-height: 1em;
   background-color: currentcolor;
   opacity: 0.25;
 }
 
 .align-baseline {
   vertical-align: baseline !important;
@@ -7004,14 +7238,39 @@
   float: right !important;
 }
 
 .float-none {
   float: none !important;
 }
 
+.object-fit-contain {
+  -o-object-fit: contain !important;
+  object-fit: contain !important;
+}
+
+.object-fit-cover {
+  -o-object-fit: cover !important;
+  object-fit: cover !important;
+}
+
+.object-fit-fill {
+  -o-object-fit: fill !important;
+  object-fit: fill !important;
+}
+
+.object-fit-scale {
+  -o-object-fit: scale-down !important;
+  object-fit: scale-down !important;
+}
+
+.object-fit-none {
+  -o-object-fit: none !important;
+  object-fit: none !important;
+}
+
 .opacity-0 {
   opacity: 0 !important;
 }
 
 .opacity-25 {
   opacity: 0.25 !important;
 }
@@ -7040,14 +7299,46 @@
   overflow: visible !important;
 }
 
 .overflow-scroll {
   overflow: scroll !important;
 }
 
+.overflow-x-auto {
+  overflow-x: auto !important;
+}
+
+.overflow-x-hidden {
+  overflow-x: hidden !important;
+}
+
+.overflow-x-visible {
+  overflow-x: visible !important;
+}
+
+.overflow-x-scroll {
+  overflow-x: scroll !important;
+}
+
+.overflow-y-auto {
+  overflow-y: auto !important;
+}
+
+.overflow-y-hidden {
+  overflow-y: hidden !important;
+}
+
+.overflow-y-visible {
+  overflow-y: visible !important;
+}
+
+.overflow-y-scroll {
+  overflow-y: scroll !important;
+}
+
 .d-inline {
   display: inline !important;
 }
 
 .d-inline-block {
   display: inline-block !important;
 }
@@ -7056,14 +7347,18 @@
   display: block !important;
 }
 
 .d-grid {
   display: grid !important;
 }
 
+.d-inline-grid {
+  display: inline-grid !important;
+}
+
 .d-table {
   display: table !important;
 }
 
 .d-table-row {
   display: table-row !important;
 }
@@ -7096,14 +7391,46 @@
   box-shadow: 0 1rem 3rem rgba(0, 0, 0, 0.175) !important;
 }
 
 .shadow-none {
   box-shadow: none !important;
 }
 
+.focus-ring-primary {
+  --bs-focus-ring-color: rgba(var(--bs-primary-rgb), var(--bs-focus-ring-opacity));
+}
+
+.focus-ring-secondary {
+  --bs-focus-ring-color: rgba(var(--bs-secondary-rgb), var(--bs-focus-ring-opacity));
+}
+
+.focus-ring-success {
+  --bs-focus-ring-color: rgba(var(--bs-success-rgb), var(--bs-focus-ring-opacity));
+}
+
+.focus-ring-info {
+  --bs-focus-ring-color: rgba(var(--bs-info-rgb), var(--bs-focus-ring-opacity));
+}
+
+.focus-ring-warning {
+  --bs-focus-ring-color: rgba(var(--bs-warning-rgb), var(--bs-focus-ring-opacity));
+}
+
+.focus-ring-danger {
+  --bs-focus-ring-color: rgba(var(--bs-danger-rgb), var(--bs-focus-ring-opacity));
+}
+
+.focus-ring-light {
+  --bs-focus-ring-color: rgba(var(--bs-light-rgb), var(--bs-focus-ring-opacity));
+}
+
+.focus-ring-dark {
+  --bs-focus-ring-color: rgba(var(--bs-dark-rgb), var(--bs-focus-ring-opacity));
+}
+
 .position-static {
   position: static !important;
 }
 
 .position-relative {
   position: relative !important;
 }
@@ -7257,37 +7584,74 @@
 }
 
 .border-dark {
   --bs-border-opacity: 1;
   border-color: rgba(var(--bs-dark-rgb), var(--bs-border-opacity)) !important;
 }
 
+.border-black {
+  --bs-border-opacity: 1;
+  border-color: rgba(var(--bs-black-rgb), var(--bs-border-opacity)) !important;
+}
+
 .border-white {
   --bs-border-opacity: 1;
   border-color: rgba(var(--bs-white-rgb), var(--bs-border-opacity)) !important;
 }
 
+.border-primary-subtle {
+  border-color: var(--bs-primary-border-subtle) !important;
+}
+
+.border-secondary-subtle {
+  border-color: var(--bs-secondary-border-subtle) !important;
+}
+
+.border-success-subtle {
+  border-color: var(--bs-success-border-subtle) !important;
+}
+
+.border-info-subtle {
+  border-color: var(--bs-info-border-subtle) !important;
+}
+
+.border-warning-subtle {
+  border-color: var(--bs-warning-border-subtle) !important;
+}
+
+.border-danger-subtle {
+  border-color: var(--bs-danger-border-subtle) !important;
+}
+
+.border-light-subtle {
+  border-color: var(--bs-light-border-subtle) !important;
+}
+
+.border-dark-subtle {
+  border-color: var(--bs-dark-border-subtle) !important;
+}
+
 .border-1 {
-  --bs-border-width: 1px;
+  border-width: 1px !important;
 }
 
 .border-2 {
-  --bs-border-width: 2px;
+  border-width: 2px !important;
 }
 
 .border-3 {
-  --bs-border-width: 3px;
+  border-width: 3px !important;
 }
 
 .border-4 {
-  --bs-border-width: 4px;
+  border-width: 4px !important;
 }
 
 .border-5 {
-  --bs-border-width: 5px;
+  border-width: 5px !important;
 }
 
 .border-opacity-10 {
   --bs-border-opacity: 0.1;
 }
 
 .border-opacity-25 {
@@ -7952,14 +8316,68 @@
   gap: 1.5rem !important;
 }
 
 .gap-5 {
   gap: 3rem !important;
 }
 
+.row-gap-0 {
+  row-gap: 0 !important;
+}
+
+.row-gap-1 {
+  row-gap: 0.25rem !important;
+}
+
+.row-gap-2 {
+  row-gap: 0.5rem !important;
+}
+
+.row-gap-3 {
+  row-gap: 1rem !important;
+}
+
+.row-gap-4 {
+  row-gap: 1.5rem !important;
+}
+
+.row-gap-5 {
+  row-gap: 3rem !important;
+}
+
+.column-gap-0 {
+  -moz-column-gap: 0 !important;
+  column-gap: 0 !important;
+}
+
+.column-gap-1 {
+  -moz-column-gap: 0.25rem !important;
+  column-gap: 0.25rem !important;
+}
+
+.column-gap-2 {
+  -moz-column-gap: 0.5rem !important;
+  column-gap: 0.5rem !important;
+}
+
+.column-gap-3 {
+  -moz-column-gap: 1rem !important;
+  column-gap: 1rem !important;
+}
+
+.column-gap-4 {
+  -moz-column-gap: 1.5rem !important;
+  column-gap: 1.5rem !important;
+}
+
+.column-gap-5 {
+  -moz-column-gap: 3rem !important;
+  column-gap: 3rem !important;
+}
+
 .font-monospace {
   font-family: var(--bs-font-monospace) !important;
 }
 
 .fs-1 {
   font-size: calc(1.375rem + 1.5vw) !important;
 }
@@ -7988,34 +8406,38 @@
   font-style: italic !important;
 }
 
 .fst-normal {
   font-style: normal !important;
 }
 
-.fw-light {
-  font-weight: 300 !important;
-}
-
 .fw-lighter {
   font-weight: lighter !important;
 }
 
+.fw-light {
+  font-weight: 300 !important;
+}
+
 .fw-normal {
   font-weight: 400 !important;
 }
 
-.fw-bold {
-  font-weight: 700 !important;
+.fw-medium {
+  font-weight: 500 !important;
 }
 
 .fw-semibold {
   font-weight: 600 !important;
 }
 
+.fw-bold {
+  font-weight: 700 !important;
+}
+
 .fw-bolder {
   font-weight: bolder !important;
 }
 
 .lh-1 {
   line-height: 1 !important;
 }
@@ -8136,27 +8558,42 @@
 .text-body {
   --bs-text-opacity: 1;
   color: rgba(var(--bs-body-color-rgb), var(--bs-text-opacity)) !important;
 }
 
 .text-muted {
   --bs-text-opacity: 1;
-  color: #6c757d !important;
+  color: var(--bs-secondary-color) !important;
 }
 
 .text-black-50 {
   --bs-text-opacity: 1;
   color: rgba(0, 0, 0, 0.5) !important;
 }
 
 .text-white-50 {
   --bs-text-opacity: 1;
   color: rgba(255, 255, 255, 0.5) !important;
 }
 
+.text-body-secondary {
+  --bs-text-opacity: 1;
+  color: var(--bs-secondary-color) !important;
+}
+
+.text-body-tertiary {
+  --bs-text-opacity: 1;
+  color: var(--bs-tertiary-color) !important;
+}
+
+.text-body-emphasis {
+  --bs-text-opacity: 1;
+  color: var(--bs-emphasis-color) !important;
+}
+
 .text-reset {
   --bs-text-opacity: 1;
   color: inherit !important;
 }
 
 .text-opacity-25 {
   --bs-text-opacity: 0.25;
@@ -8170,14 +8607,212 @@
   --bs-text-opacity: 0.75;
 }
 
 .text-opacity-100 {
   --bs-text-opacity: 1;
 }
 
+.text-primary-emphasis {
+  color: var(--bs-primary-text-emphasis) !important;
+}
+
+.text-secondary-emphasis {
+  color: var(--bs-secondary-text-emphasis) !important;
+}
+
+.text-success-emphasis {
+  color: var(--bs-success-text-emphasis) !important;
+}
+
+.text-info-emphasis {
+  color: var(--bs-info-text-emphasis) !important;
+}
+
+.text-warning-emphasis {
+  color: var(--bs-warning-text-emphasis) !important;
+}
+
+.text-danger-emphasis {
+  color: var(--bs-danger-text-emphasis) !important;
+}
+
+.text-light-emphasis {
+  color: var(--bs-light-text-emphasis) !important;
+}
+
+.text-dark-emphasis {
+  color: var(--bs-dark-text-emphasis) !important;
+}
+
+.link-opacity-10 {
+  --bs-link-opacity: 0.1;
+}
+
+.link-opacity-10-hover:hover {
+  --bs-link-opacity: 0.1;
+}
+
+.link-opacity-25 {
+  --bs-link-opacity: 0.25;
+}
+
+.link-opacity-25-hover:hover {
+  --bs-link-opacity: 0.25;
+}
+
+.link-opacity-50 {
+  --bs-link-opacity: 0.5;
+}
+
+.link-opacity-50-hover:hover {
+  --bs-link-opacity: 0.5;
+}
+
+.link-opacity-75 {
+  --bs-link-opacity: 0.75;
+}
+
+.link-opacity-75-hover:hover {
+  --bs-link-opacity: 0.75;
+}
+
+.link-opacity-100 {
+  --bs-link-opacity: 1;
+}
+
+.link-opacity-100-hover:hover {
+  --bs-link-opacity: 1;
+}
+
+.link-offset-1 {
+  text-underline-offset: 0.125em !important;
+}
+
+.link-offset-1-hover:hover {
+  text-underline-offset: 0.125em !important;
+}
+
+.link-offset-2 {
+  text-underline-offset: 0.25em !important;
+}
+
+.link-offset-2-hover:hover {
+  text-underline-offset: 0.25em !important;
+}
+
+.link-offset-3 {
+  text-underline-offset: 0.375em !important;
+}
+
+.link-offset-3-hover:hover {
+  text-underline-offset: 0.375em !important;
+}
+
+.link-underline-primary {
+  --bs-link-underline-opacity: 1;
+  -webkit-text-decoration-color: rgba(var(--bs-primary-rgb), var(--bs-link-underline-opacity)) !important;
+  text-decoration-color: rgba(var(--bs-primary-rgb), var(--bs-link-underline-opacity)) !important;
+}
+
+.link-underline-secondary {
+  --bs-link-underline-opacity: 1;
+  -webkit-text-decoration-color: rgba(var(--bs-secondary-rgb), var(--bs-link-underline-opacity)) !important;
+  text-decoration-color: rgba(var(--bs-secondary-rgb), var(--bs-link-underline-opacity)) !important;
+}
+
+.link-underline-success {
+  --bs-link-underline-opacity: 1;
+  -webkit-text-decoration-color: rgba(var(--bs-success-rgb), var(--bs-link-underline-opacity)) !important;
+  text-decoration-color: rgba(var(--bs-success-rgb), var(--bs-link-underline-opacity)) !important;
+}
+
+.link-underline-info {
+  --bs-link-underline-opacity: 1;
+  -webkit-text-decoration-color: rgba(var(--bs-info-rgb), var(--bs-link-underline-opacity)) !important;
+  text-decoration-color: rgba(var(--bs-info-rgb), var(--bs-link-underline-opacity)) !important;
+}
+
+.link-underline-warning {
+  --bs-link-underline-opacity: 1;
+  -webkit-text-decoration-color: rgba(var(--bs-warning-rgb), var(--bs-link-underline-opacity)) !important;
+  text-decoration-color: rgba(var(--bs-warning-rgb), var(--bs-link-underline-opacity)) !important;
+}
+
+.link-underline-danger {
+  --bs-link-underline-opacity: 1;
+  -webkit-text-decoration-color: rgba(var(--bs-danger-rgb), var(--bs-link-underline-opacity)) !important;
+  text-decoration-color: rgba(var(--bs-danger-rgb), var(--bs-link-underline-opacity)) !important;
+}
+
+.link-underline-light {
+  --bs-link-underline-opacity: 1;
+  -webkit-text-decoration-color: rgba(var(--bs-light-rgb), var(--bs-link-underline-opacity)) !important;
+  text-decoration-color: rgba(var(--bs-light-rgb), var(--bs-link-underline-opacity)) !important;
+}
+
+.link-underline-dark {
+  --bs-link-underline-opacity: 1;
+  -webkit-text-decoration-color: rgba(var(--bs-dark-rgb), var(--bs-link-underline-opacity)) !important;
+  text-decoration-color: rgba(var(--bs-dark-rgb), var(--bs-link-underline-opacity)) !important;
+}
+
+.link-underline {
+  --bs-link-underline-opacity: 1;
+  -webkit-text-decoration-color: rgba(var(--bs-link-color-rgb), var(--bs-link-underline-opacity, 1)) !important;
+  text-decoration-color: rgba(var(--bs-link-color-rgb), var(--bs-link-underline-opacity, 1)) !important;
+}
+
+.link-underline-opacity-0 {
+  --bs-link-underline-opacity: 0;
+}
+
+.link-underline-opacity-0-hover:hover {
+  --bs-link-underline-opacity: 0;
+}
+
+.link-underline-opacity-10 {
+  --bs-link-underline-opacity: 0.1;
+}
+
+.link-underline-opacity-10-hover:hover {
+  --bs-link-underline-opacity: 0.1;
+}
+
+.link-underline-opacity-25 {
+  --bs-link-underline-opacity: 0.25;
+}
+
+.link-underline-opacity-25-hover:hover {
+  --bs-link-underline-opacity: 0.25;
+}
+
+.link-underline-opacity-50 {
+  --bs-link-underline-opacity: 0.5;
+}
+
+.link-underline-opacity-50-hover:hover {
+  --bs-link-underline-opacity: 0.5;
+}
+
+.link-underline-opacity-75 {
+  --bs-link-underline-opacity: 0.75;
+}
+
+.link-underline-opacity-75-hover:hover {
+  --bs-link-underline-opacity: 0.75;
+}
+
+.link-underline-opacity-100 {
+  --bs-link-underline-opacity: 1;
+}
+
+.link-underline-opacity-100-hover:hover {
+  --bs-link-underline-opacity: 1;
+}
+
 .bg-primary {
   --bs-bg-opacity: 1;
   background-color: rgba(var(--bs-primary-rgb), var(--bs-bg-opacity)) !important;
 }
 
 .bg-secondary {
   --bs-bg-opacity: 1;
@@ -8230,14 +8865,24 @@
 }
 
 .bg-transparent {
   --bs-bg-opacity: 1;
   background-color: transparent !important;
 }
 
+.bg-body-secondary {
+  --bs-bg-opacity: 1;
+  background-color: rgba(var(--bs-secondary-bg-rgb), var(--bs-bg-opacity)) !important;
+}
+
+.bg-body-tertiary {
+  --bs-bg-opacity: 1;
+  background-color: rgba(var(--bs-tertiary-bg-rgb), var(--bs-bg-opacity)) !important;
+}
+
 .bg-opacity-10 {
   --bs-bg-opacity: 0.1;
 }
 
 .bg-opacity-25 {
   --bs-bg-opacity: 0.25;
 }
@@ -8250,14 +8895,46 @@
   --bs-bg-opacity: 0.75;
 }
 
 .bg-opacity-100 {
   --bs-bg-opacity: 1;
 }
 
+.bg-primary-subtle {
+  background-color: var(--bs-primary-bg-subtle) !important;
+}
+
+.bg-secondary-subtle {
+  background-color: var(--bs-secondary-bg-subtle) !important;
+}
+
+.bg-success-subtle {
+  background-color: var(--bs-success-bg-subtle) !important;
+}
+
+.bg-info-subtle {
+  background-color: var(--bs-info-bg-subtle) !important;
+}
+
+.bg-warning-subtle {
+  background-color: var(--bs-warning-bg-subtle) !important;
+}
+
+.bg-danger-subtle {
+  background-color: var(--bs-danger-bg-subtle) !important;
+}
+
+.bg-light-subtle {
+  background-color: var(--bs-light-bg-subtle) !important;
+}
+
+.bg-dark-subtle {
+  background-color: var(--bs-dark-bg-subtle) !important;
+}
+
 .bg-gradient {
   background-image: var(--bs-gradient) !important;
 }
 
 .user-select-all {
   -webkit-user-select: all !important;
   -moz-user-select: all !important;
@@ -8305,15 +8982,15 @@
 }
 
 .rounded-4 {
   border-radius: var(--bs-border-radius-xl) !important;
 }
 
 .rounded-5 {
-  border-radius: var(--bs-border-radius-2xl) !important;
+  border-radius: var(--bs-border-radius-xxl) !important;
 }
 
 .rounded-circle {
   border-radius: 50% !important;
 }
 
 .rounded-pill {
@@ -8321,59 +8998,262 @@
 }
 
 .rounded-top {
   border-top-left-radius: var(--bs-border-radius) !important;
   border-top-right-radius: var(--bs-border-radius) !important;
 }
 
+.rounded-top-0 {
+  border-top-left-radius: 0 !important;
+  border-top-right-radius: 0 !important;
+}
+
+.rounded-top-1 {
+  border-top-left-radius: var(--bs-border-radius-sm) !important;
+  border-top-right-radius: var(--bs-border-radius-sm) !important;
+}
+
+.rounded-top-2 {
+  border-top-left-radius: var(--bs-border-radius) !important;
+  border-top-right-radius: var(--bs-border-radius) !important;
+}
+
+.rounded-top-3 {
+  border-top-left-radius: var(--bs-border-radius-lg) !important;
+  border-top-right-radius: var(--bs-border-radius-lg) !important;
+}
+
+.rounded-top-4 {
+  border-top-left-radius: var(--bs-border-radius-xl) !important;
+  border-top-right-radius: var(--bs-border-radius-xl) !important;
+}
+
+.rounded-top-5 {
+  border-top-left-radius: var(--bs-border-radius-xxl) !important;
+  border-top-right-radius: var(--bs-border-radius-xxl) !important;
+}
+
+.rounded-top-circle {
+  border-top-left-radius: 50% !important;
+  border-top-right-radius: 50% !important;
+}
+
+.rounded-top-pill {
+  border-top-left-radius: var(--bs-border-radius-pill) !important;
+  border-top-right-radius: var(--bs-border-radius-pill) !important;
+}
+
 .rounded-end {
   border-top-right-radius: var(--bs-border-radius) !important;
   border-bottom-right-radius: var(--bs-border-radius) !important;
 }
 
+.rounded-end-0 {
+  border-top-right-radius: 0 !important;
+  border-bottom-right-radius: 0 !important;
+}
+
+.rounded-end-1 {
+  border-top-right-radius: var(--bs-border-radius-sm) !important;
+  border-bottom-right-radius: var(--bs-border-radius-sm) !important;
+}
+
+.rounded-end-2 {
+  border-top-right-radius: var(--bs-border-radius) !important;
+  border-bottom-right-radius: var(--bs-border-radius) !important;
+}
+
+.rounded-end-3 {
+  border-top-right-radius: var(--bs-border-radius-lg) !important;
+  border-bottom-right-radius: var(--bs-border-radius-lg) !important;
+}
+
+.rounded-end-4 {
+  border-top-right-radius: var(--bs-border-radius-xl) !important;
+  border-bottom-right-radius: var(--bs-border-radius-xl) !important;
+}
+
+.rounded-end-5 {
+  border-top-right-radius: var(--bs-border-radius-xxl) !important;
+  border-bottom-right-radius: var(--bs-border-radius-xxl) !important;
+}
+
+.rounded-end-circle {
+  border-top-right-radius: 50% !important;
+  border-bottom-right-radius: 50% !important;
+}
+
+.rounded-end-pill {
+  border-top-right-radius: var(--bs-border-radius-pill) !important;
+  border-bottom-right-radius: var(--bs-border-radius-pill) !important;
+}
+
 .rounded-bottom {
   border-bottom-right-radius: var(--bs-border-radius) !important;
   border-bottom-left-radius: var(--bs-border-radius) !important;
 }
 
+.rounded-bottom-0 {
+  border-bottom-right-radius: 0 !important;
+  border-bottom-left-radius: 0 !important;
+}
+
+.rounded-bottom-1 {
+  border-bottom-right-radius: var(--bs-border-radius-sm) !important;
+  border-bottom-left-radius: var(--bs-border-radius-sm) !important;
+}
+
+.rounded-bottom-2 {
+  border-bottom-right-radius: var(--bs-border-radius) !important;
+  border-bottom-left-radius: var(--bs-border-radius) !important;
+}
+
+.rounded-bottom-3 {
+  border-bottom-right-radius: var(--bs-border-radius-lg) !important;
+  border-bottom-left-radius: var(--bs-border-radius-lg) !important;
+}
+
+.rounded-bottom-4 {
+  border-bottom-right-radius: var(--bs-border-radius-xl) !important;
+  border-bottom-left-radius: var(--bs-border-radius-xl) !important;
+}
+
+.rounded-bottom-5 {
+  border-bottom-right-radius: var(--bs-border-radius-xxl) !important;
+  border-bottom-left-radius: var(--bs-border-radius-xxl) !important;
+}
+
+.rounded-bottom-circle {
+  border-bottom-right-radius: 50% !important;
+  border-bottom-left-radius: 50% !important;
+}
+
+.rounded-bottom-pill {
+  border-bottom-right-radius: var(--bs-border-radius-pill) !important;
+  border-bottom-left-radius: var(--bs-border-radius-pill) !important;
+}
+
 .rounded-start {
   border-bottom-left-radius: var(--bs-border-radius) !important;
   border-top-left-radius: var(--bs-border-radius) !important;
 }
 
+.rounded-start-0 {
+  border-bottom-left-radius: 0 !important;
+  border-top-left-radius: 0 !important;
+}
+
+.rounded-start-1 {
+  border-bottom-left-radius: var(--bs-border-radius-sm) !important;
+  border-top-left-radius: var(--bs-border-radius-sm) !important;
+}
+
+.rounded-start-2 {
+  border-bottom-left-radius: var(--bs-border-radius) !important;
+  border-top-left-radius: var(--bs-border-radius) !important;
+}
+
+.rounded-start-3 {
+  border-bottom-left-radius: var(--bs-border-radius-lg) !important;
+  border-top-left-radius: var(--bs-border-radius-lg) !important;
+}
+
+.rounded-start-4 {
+  border-bottom-left-radius: var(--bs-border-radius-xl) !important;
+  border-top-left-radius: var(--bs-border-radius-xl) !important;
+}
+
+.rounded-start-5 {
+  border-bottom-left-radius: var(--bs-border-radius-xxl) !important;
+  border-top-left-radius: var(--bs-border-radius-xxl) !important;
+}
+
+.rounded-start-circle {
+  border-bottom-left-radius: 50% !important;
+  border-top-left-radius: 50% !important;
+}
+
+.rounded-start-pill {
+  border-bottom-left-radius: var(--bs-border-radius-pill) !important;
+  border-top-left-radius: var(--bs-border-radius-pill) !important;
+}
+
 .visible {
   visibility: visible !important;
 }
 
 .invisible {
   visibility: hidden !important;
 }
 
+.z-n1 {
+  z-index: -1 !important;
+}
+
+.z-0 {
+  z-index: 0 !important;
+}
+
+.z-1 {
+  z-index: 1 !important;
+}
+
+.z-2 {
+  z-index: 2 !important;
+}
+
+.z-3 {
+  z-index: 3 !important;
+}
+
 @media (min-width: 576px) {
   .float-sm-start {
     float: left !important;
   }
   .float-sm-end {
     float: right !important;
   }
   .float-sm-none {
     float: none !important;
   }
+  .object-fit-sm-contain {
+    -o-object-fit: contain !important;
+    object-fit: contain !important;
+  }
+  .object-fit-sm-cover {
+    -o-object-fit: cover !important;
+    object-fit: cover !important;
+  }
+  .object-fit-sm-fill {
+    -o-object-fit: fill !important;
+    object-fit: fill !important;
+  }
+  .object-fit-sm-scale {
+    -o-object-fit: scale-down !important;
+    object-fit: scale-down !important;
+  }
+  .object-fit-sm-none {
+    -o-object-fit: none !important;
+    object-fit: none !important;
+  }
   .d-sm-inline {
     display: inline !important;
   }
   .d-sm-inline-block {
     display: inline-block !important;
   }
   .d-sm-block {
     display: block !important;
   }
   .d-sm-grid {
     display: grid !important;
   }
+  .d-sm-inline-grid {
+    display: inline-grid !important;
+  }
   .d-sm-table {
     display: table !important;
   }
   .d-sm-table-row {
     display: table-row !important;
   }
   .d-sm-table-cell {
@@ -8830,14 +9710,56 @@
   }
   .gap-sm-4 {
     gap: 1.5rem !important;
   }
   .gap-sm-5 {
     gap: 3rem !important;
   }
+  .row-gap-sm-0 {
+    row-gap: 0 !important;
+  }
+  .row-gap-sm-1 {
+    row-gap: 0.25rem !important;
+  }
+  .row-gap-sm-2 {
+    row-gap: 0.5rem !important;
+  }
+  .row-gap-sm-3 {
+    row-gap: 1rem !important;
+  }
+  .row-gap-sm-4 {
+    row-gap: 1.5rem !important;
+  }
+  .row-gap-sm-5 {
+    row-gap: 3rem !important;
+  }
+  .column-gap-sm-0 {
+    -moz-column-gap: 0 !important;
+    column-gap: 0 !important;
+  }
+  .column-gap-sm-1 {
+    -moz-column-gap: 0.25rem !important;
+    column-gap: 0.25rem !important;
+  }
+  .column-gap-sm-2 {
+    -moz-column-gap: 0.5rem !important;
+    column-gap: 0.5rem !important;
+  }
+  .column-gap-sm-3 {
+    -moz-column-gap: 1rem !important;
+    column-gap: 1rem !important;
+  }
+  .column-gap-sm-4 {
+    -moz-column-gap: 1.5rem !important;
+    column-gap: 1.5rem !important;
+  }
+  .column-gap-sm-5 {
+    -moz-column-gap: 3rem !important;
+    column-gap: 3rem !important;
+  }
   .text-sm-start {
     text-align: left !important;
   }
   .text-sm-end {
     text-align: right !important;
   }
   .text-sm-center {
@@ -8850,26 +9772,49 @@
   }
   .float-md-end {
     float: right !important;
   }
   .float-md-none {
     float: none !important;
   }
+  .object-fit-md-contain {
+    -o-object-fit: contain !important;
+    object-fit: contain !important;
+  }
+  .object-fit-md-cover {
+    -o-object-fit: cover !important;
+    object-fit: cover !important;
+  }
+  .object-fit-md-fill {
+    -o-object-fit: fill !important;
+    object-fit: fill !important;
+  }
+  .object-fit-md-scale {
+    -o-object-fit: scale-down !important;
+    object-fit: scale-down !important;
+  }
+  .object-fit-md-none {
+    -o-object-fit: none !important;
+    object-fit: none !important;
+  }
   .d-md-inline {
     display: inline !important;
   }
   .d-md-inline-block {
     display: inline-block !important;
   }
   .d-md-block {
     display: block !important;
   }
   .d-md-grid {
     display: grid !important;
   }
+  .d-md-inline-grid {
+    display: inline-grid !important;
+  }
   .d-md-table {
     display: table !important;
   }
   .d-md-table-row {
     display: table-row !important;
   }
   .d-md-table-cell {
@@ -9326,14 +10271,56 @@
   }
   .gap-md-4 {
     gap: 1.5rem !important;
   }
   .gap-md-5 {
     gap: 3rem !important;
   }
+  .row-gap-md-0 {
+    row-gap: 0 !important;
+  }
+  .row-gap-md-1 {
+    row-gap: 0.25rem !important;
+  }
+  .row-gap-md-2 {
+    row-gap: 0.5rem !important;
+  }
+  .row-gap-md-3 {
+    row-gap: 1rem !important;
+  }
+  .row-gap-md-4 {
+    row-gap: 1.5rem !important;
+  }
+  .row-gap-md-5 {
+    row-gap: 3rem !important;
+  }
+  .column-gap-md-0 {
+    -moz-column-gap: 0 !important;
+    column-gap: 0 !important;
+  }
+  .column-gap-md-1 {
+    -moz-column-gap: 0.25rem !important;
+    column-gap: 0.25rem !important;
+  }
+  .column-gap-md-2 {
+    -moz-column-gap: 0.5rem !important;
+    column-gap: 0.5rem !important;
+  }
+  .column-gap-md-3 {
+    -moz-column-gap: 1rem !important;
+    column-gap: 1rem !important;
+  }
+  .column-gap-md-4 {
+    -moz-column-gap: 1.5rem !important;
+    column-gap: 1.5rem !important;
+  }
+  .column-gap-md-5 {
+    -moz-column-gap: 3rem !important;
+    column-gap: 3rem !important;
+  }
   .text-md-start {
     text-align: left !important;
   }
   .text-md-end {
     text-align: right !important;
   }
   .text-md-center {
@@ -9346,26 +10333,49 @@
   }
   .float-lg-end {
     float: right !important;
   }
   .float-lg-none {
     float: none !important;
   }
+  .object-fit-lg-contain {
+    -o-object-fit: contain !important;
+    object-fit: contain !important;
+  }
+  .object-fit-lg-cover {
+    -o-object-fit: cover !important;
+    object-fit: cover !important;
+  }
+  .object-fit-lg-fill {
+    -o-object-fit: fill !important;
+    object-fit: fill !important;
+  }
+  .object-fit-lg-scale {
+    -o-object-fit: scale-down !important;
+    object-fit: scale-down !important;
+  }
+  .object-fit-lg-none {
+    -o-object-fit: none !important;
+    object-fit: none !important;
+  }
   .d-lg-inline {
     display: inline !important;
   }
   .d-lg-inline-block {
     display: inline-block !important;
   }
   .d-lg-block {
     display: block !important;
   }
   .d-lg-grid {
     display: grid !important;
   }
+  .d-lg-inline-grid {
+    display: inline-grid !important;
+  }
   .d-lg-table {
     display: table !important;
   }
   .d-lg-table-row {
     display: table-row !important;
   }
   .d-lg-table-cell {
@@ -9822,14 +10832,56 @@
   }
   .gap-lg-4 {
     gap: 1.5rem !important;
   }
   .gap-lg-5 {
     gap: 3rem !important;
   }
+  .row-gap-lg-0 {
+    row-gap: 0 !important;
+  }
+  .row-gap-lg-1 {
+    row-gap: 0.25rem !important;
+  }
+  .row-gap-lg-2 {
+    row-gap: 0.5rem !important;
+  }
+  .row-gap-lg-3 {
+    row-gap: 1rem !important;
+  }
+  .row-gap-lg-4 {
+    row-gap: 1.5rem !important;
+  }
+  .row-gap-lg-5 {
+    row-gap: 3rem !important;
+  }
+  .column-gap-lg-0 {
+    -moz-column-gap: 0 !important;
+    column-gap: 0 !important;
+  }
+  .column-gap-lg-1 {
+    -moz-column-gap: 0.25rem !important;
+    column-gap: 0.25rem !important;
+  }
+  .column-gap-lg-2 {
+    -moz-column-gap: 0.5rem !important;
+    column-gap: 0.5rem !important;
+  }
+  .column-gap-lg-3 {
+    -moz-column-gap: 1rem !important;
+    column-gap: 1rem !important;
+  }
+  .column-gap-lg-4 {
+    -moz-column-gap: 1.5rem !important;
+    column-gap: 1.5rem !important;
+  }
+  .column-gap-lg-5 {
+    -moz-column-gap: 3rem !important;
+    column-gap: 3rem !important;
+  }
   .text-lg-start {
     text-align: left !important;
   }
   .text-lg-end {
     text-align: right !important;
   }
   .text-lg-center {
@@ -9842,26 +10894,49 @@
   }
   .float-xl-end {
     float: right !important;
   }
   .float-xl-none {
     float: none !important;
   }
+  .object-fit-xl-contain {
+    -o-object-fit: contain !important;
+    object-fit: contain !important;
+  }
+  .object-fit-xl-cover {
+    -o-object-fit: cover !important;
+    object-fit: cover !important;
+  }
+  .object-fit-xl-fill {
+    -o-object-fit: fill !important;
+    object-fit: fill !important;
+  }
+  .object-fit-xl-scale {
+    -o-object-fit: scale-down !important;
+    object-fit: scale-down !important;
+  }
+  .object-fit-xl-none {
+    -o-object-fit: none !important;
+    object-fit: none !important;
+  }
   .d-xl-inline {
     display: inline !important;
   }
   .d-xl-inline-block {
     display: inline-block !important;
   }
   .d-xl-block {
     display: block !important;
   }
   .d-xl-grid {
     display: grid !important;
   }
+  .d-xl-inline-grid {
+    display: inline-grid !important;
+  }
   .d-xl-table {
     display: table !important;
   }
   .d-xl-table-row {
     display: table-row !important;
   }
   .d-xl-table-cell {
@@ -10318,14 +11393,56 @@
   }
   .gap-xl-4 {
     gap: 1.5rem !important;
   }
   .gap-xl-5 {
     gap: 3rem !important;
   }
+  .row-gap-xl-0 {
+    row-gap: 0 !important;
+  }
+  .row-gap-xl-1 {
+    row-gap: 0.25rem !important;
+  }
+  .row-gap-xl-2 {
+    row-gap: 0.5rem !important;
+  }
+  .row-gap-xl-3 {
+    row-gap: 1rem !important;
+  }
+  .row-gap-xl-4 {
+    row-gap: 1.5rem !important;
+  }
+  .row-gap-xl-5 {
+    row-gap: 3rem !important;
+  }
+  .column-gap-xl-0 {
+    -moz-column-gap: 0 !important;
+    column-gap: 0 !important;
+  }
+  .column-gap-xl-1 {
+    -moz-column-gap: 0.25rem !important;
+    column-gap: 0.25rem !important;
+  }
+  .column-gap-xl-2 {
+    -moz-column-gap: 0.5rem !important;
+    column-gap: 0.5rem !important;
+  }
+  .column-gap-xl-3 {
+    -moz-column-gap: 1rem !important;
+    column-gap: 1rem !important;
+  }
+  .column-gap-xl-4 {
+    -moz-column-gap: 1.5rem !important;
+    column-gap: 1.5rem !important;
+  }
+  .column-gap-xl-5 {
+    -moz-column-gap: 3rem !important;
+    column-gap: 3rem !important;
+  }
   .text-xl-start {
     text-align: left !important;
   }
   .text-xl-end {
     text-align: right !important;
   }
   .text-xl-center {
@@ -10338,26 +11455,49 @@
   }
   .float-xxl-end {
     float: right !important;
   }
   .float-xxl-none {
     float: none !important;
   }
+  .object-fit-xxl-contain {
+    -o-object-fit: contain !important;
+    object-fit: contain !important;
+  }
+  .object-fit-xxl-cover {
+    -o-object-fit: cover !important;
+    object-fit: cover !important;
+  }
+  .object-fit-xxl-fill {
+    -o-object-fit: fill !important;
+    object-fit: fill !important;
+  }
+  .object-fit-xxl-scale {
+    -o-object-fit: scale-down !important;
+    object-fit: scale-down !important;
+  }
+  .object-fit-xxl-none {
+    -o-object-fit: none !important;
+    object-fit: none !important;
+  }
   .d-xxl-inline {
     display: inline !important;
   }
   .d-xxl-inline-block {
     display: inline-block !important;
   }
   .d-xxl-block {
     display: block !important;
   }
   .d-xxl-grid {
     display: grid !important;
   }
+  .d-xxl-inline-grid {
+    display: inline-grid !important;
+  }
   .d-xxl-table {
     display: table !important;
   }
   .d-xxl-table-row {
     display: table-row !important;
   }
   .d-xxl-table-cell {
@@ -10814,14 +11954,56 @@
   }
   .gap-xxl-4 {
     gap: 1.5rem !important;
   }
   .gap-xxl-5 {
     gap: 3rem !important;
   }
+  .row-gap-xxl-0 {
+    row-gap: 0 !important;
+  }
+  .row-gap-xxl-1 {
+    row-gap: 0.25rem !important;
+  }
+  .row-gap-xxl-2 {
+    row-gap: 0.5rem !important;
+  }
+  .row-gap-xxl-3 {
+    row-gap: 1rem !important;
+  }
+  .row-gap-xxl-4 {
+    row-gap: 1.5rem !important;
+  }
+  .row-gap-xxl-5 {
+    row-gap: 3rem !important;
+  }
+  .column-gap-xxl-0 {
+    -moz-column-gap: 0 !important;
+    column-gap: 0 !important;
+  }
+  .column-gap-xxl-1 {
+    -moz-column-gap: 0.25rem !important;
+    column-gap: 0.25rem !important;
+  }
+  .column-gap-xxl-2 {
+    -moz-column-gap: 0.5rem !important;
+    column-gap: 0.5rem !important;
+  }
+  .column-gap-xxl-3 {
+    -moz-column-gap: 1rem !important;
+    column-gap: 1rem !important;
+  }
+  .column-gap-xxl-4 {
+    -moz-column-gap: 1.5rem !important;
+    column-gap: 1.5rem !important;
+  }
+  .column-gap-xxl-5 {
+    -moz-column-gap: 3rem !important;
+    column-gap: 3rem !important;
+  }
   .text-xxl-start {
     text-align: left !important;
   }
   .text-xxl-end {
     text-align: right !important;
   }
   .text-xxl-center {
@@ -10851,14 +12033,17 @@
   }
   .d-print-block {
     display: block !important;
   }
   .d-print-grid {
     display: grid !important;
   }
+  .d-print-inline-grid {
+    display: inline-grid !important;
+  }
   .d-print-table {
     display: table !important;
   }
   .d-print-table-row {
     display: table-row !important;
   }
   .d-print-table-cell {
```

### Comparing `fietsboek-0.8.0/fietsboek/static/favicon.png` & `fietsboek-0.9.0/fietsboek/static/favicon.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fietsboek.js` & `fietsboek-0.9.0/fietsboek/static/fietsboek.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,57 @@
 "use strict";
 // Make eslint happy about the Window redefinition
 (_) => null;
 /**
+ * Gets the value of a single cookie.
+ *
+ * @param name - Name of the cookie.
+ * @return The cookie value, or null.
+ */
+function getCookie(name) {
+    var _a;
+    return (_a = document.cookie.split("; ")
+        .find((row) => row.startsWith(`${name}=`))) === null || _a === void 0 ? void 0 : _a.split("=")[1];
+}
+/**
+ * Builds a URL with the correct application URL as base.
+ *
+ * Do not add the leading slash, otherwise the resolution will be wrong!
+ *
+ * @param path - Path to append to the base.
+ * @return The correct URL in regards to the application URL.
+ */
+function makeUrl(name) {
+    return new URL(name, BASE_URL);
+}
+/**
  * Installs a listener to the given DOM objects.
  *
  * @param selector - The query selector to find the DOM objects.
  * @param event - The event name to listen to.
  * @param handler - The handler function.
  */
 function addHandler(selector, event, handler) {
     document.querySelectorAll(selector).
     forEach((obj) => obj.addEventListener(event, handler));
 }
 /**
+ * Handler for when a language is clicked. Sets the cookie to the correct locale.
+ *
+ * @param event - The triggering event.
+ */
+function languageClicked(event) {
+    const path = new URL(BASE_URL).pathname;
+    const language = event.target.getAttribute("data-langcode");
+    document.cookie = `fietsboek_locale=${language}; Path=${path}`;
+    window.location.reload();
+    event.preventDefault();
+}
+addHandler(".language-choice", "click", languageClicked);
+/**
  * Handler for when a tag is clicked. Removes the tag from the tag list.
  *
  * @param event - The triggering event.
  */
 function tagClicked(event) {
     const span = event.target.closest('span');
     span.parentNode.removeChild(span);
@@ -98,39 +133,56 @@
     if (nameField.value.length == 0) {
         nameField.setCustomValidity('Needs a name');
     }
 }
 // This function is used via a HTML onchange= handler, so make eslint happy
 checkNameValidity;
 /**
+ * Check whether the given friend is already tagged.
+ *
+ * Note that this uses the "HTML list", so it uses the tags that the user is
+ * currently editing - not the ones from the database!
+ *
+ * @param friendId - ID of the friend to check.
+ * @return Whether the friend is in the list of tagged people.
+ */
+function friendIsTagged(friendId) {
+    return Array.from(document.querySelectorAll("[name='tagged-friend[]']"))
+        .map((obj) => obj)
+        .filter((obj) => !obj.disabled)
+        .map((obj) => obj.value)
+        .includes(friendId.toString());
+}
+/**
  * Hit the endpoint to search for friends. This populates the friend selector
  * when tagging friends.
  */
 function searchFriends() {
     const searchPattern = document.querySelector("#friendSearchQuery").
     value.toLowerCase();
     const friendSearch = document.querySelector("#friendSearch");
     friendSearch.innerHTML = "";
     fetch(FRIENDS_URL)
         .then((response) => response.json())
         .then((response) => {
-            const blueprint = document.querySelector("#friendSearchBlueprint");
+            const blueprint = document.querySelector("#friendSearchBlueprint").content;
             // Only show friends with a matching name
-            const friends = response.filter((obj) => obj.name.toLowerCase().indexOf(searchPattern) != -1);
+            let friends = response.filter((obj) => obj.name.toLowerCase().indexOf(searchPattern) != -1);
+            // Only show friends that are not yet existing
+            friends = friends.filter((obj) => !friendIsTagged(obj.id));
             friends.forEach((friend) => {
                 var _a;
                 const copy = blueprint.cloneNode(true);
-                copy.removeAttribute("id");
                 copy.querySelector(".friend-name").textContent = friend.name;
                 (_a = copy.querySelector("button")) === null || _a === void 0 ? void 0 : _a.addEventListener("click", (event) => {
                     const button = event.target.closest("button");
                     button.parentNode.parentNode.removeChild(button.parentNode);
-                    const added = document.querySelector("#friendAddedBlueprint").
-                    cloneNode(true);
-                    added.removeAttribute("id");
+                    const added = document.querySelector("#friendAddedBlueprint")
+                        .content
+                        .cloneNode(true);
                     added.querySelector(".friend-name").
                     textContent = friend.name;
                     added.querySelector("input").value = friend.id.toString();
                     added.querySelector("input").removeAttribute("disabled");
                     added.querySelector("button").addEventListener("click", removeFriendClicked);
                     document.querySelector('#taggedFriends').appendChild(added);
                 });
@@ -163,36 +215,35 @@
  * that each one can be removed individually. It also adds preview images, and
  * adds the button to delete and edit the image's description.
  *
  * @param event - The triggering event.
  */
 function imageSelectorChanged(event) {
     var _a;
-    console.log(event);
     const target = event.target;
     for (const file of Array.from((_a = target.files) !== null && _a !== void 0 ? _a : [])) {
         window.fietsboekImageIndex++;
         const input = document.createElement("input");
         input.type = "file";
         input.hidden = true;
         input.name = `image[${window.fietsboekImageIndex}]`;
         const transfer = new DataTransfer();
         transfer.items.add(file);
         input.files = transfer.files;
         const preview = document.querySelector("#trackImagePreviewBlueprint").
+        content.
         cloneNode(true);
-        preview.removeAttribute("id");
         preview.querySelector("img").src = URL.createObjectURL(file);
         preview.querySelector("button.delete-image").
         addEventListener("click", deleteImageButtonClicked);
         preview.querySelector("button.edit-image-description").
         addEventListener("click", editImageDescriptionClicked);
         preview.querySelector("input.image-description-input").
         name = `image-description[${window.fietsboekImageIndex}]`;
-        preview.appendChild(input);
+        preview.querySelector("div").appendChild(input);
         document.querySelector("#trackImageList").appendChild(preview);
     }
     target.value = "";
 }
 addHandler("#imageSelector", "change", imageSelectorChanged);
 /**
  * Handler to remove a picture from a track.
@@ -268,15 +319,15 @@
 }
 addHandler(".summary-toggler", "click", toggleSummary);
 /*
  * Handler to enable the "Download archive button" ...
  */
 addHandler("#archiveDownloadButton", "click", () => {
     const checked = document.querySelectorAll(".archive-checkbox:checked");
-    const url = new URL("/track/archive", window.location.href);
+    const url = makeUrl("track/archive");
     checked.forEach((c) => {
         url.searchParams.append("track_id[]", c.value);
     });
     window.location.assign(url);
 });
 /*
  * ... and the listeners on the checkboxes to disable and enable the button.
@@ -303,23 +354,99 @@
  * Handler to change the sorting of the home page.
  *
  * This basically sets the cookie to signal that the home page should be
  * returned reversed, and then reloads the page.
  *
  * @param event - The triggering event.
  */
-function changeHomeSorting(event) {
-    var _a, _b;
-    const currentSorting = (_b = (_a = document.cookie.split("; ")
-        .find((row) => row.startsWith("home_sorting="))) === null || _a === void 0 ? void 0 : _a.split("=")[1]) !== null && _b !== void 0 ? _b : "asc";
+function changeHomeSorting(_event) {
+    var _a;
+    const currentSorting = (_a = getCookie("home_sorting")) !== null && _a !== void 0 ? _a : "asc";
     const newSorting = currentSorting == "asc" ? "desc" : "asc";
     document.cookie = `home_sorting=${newSorting}; SameSite=Lax`;
     window.location.reload();
 }
 addHandler("#changeHomeSorting", "click", changeHomeSorting);
+/**
+ * Handler to toggle the favourite status of a track.
+ *
+ * This is applied to .favourite-star elements and expects the track ID in
+ * data-track-id.
+ *
+ * @param event - The triggering event.
+ */
+function toggleTrackFavourite(event) {
+    var _a;
+    const target = event.target;
+    const trackId = target.getAttribute("data-track-id");
+    if (trackId === null) {
+        return;
+    }
+    const url = makeUrl("me/toggle-favourite");
+    const formData = new URLSearchParams();
+    formData.append("track-id", trackId);
+    formData.append("csrf_token", (_a = getCookie("csrf_token")) !== null && _a !== void 0 ? _a : "");
+    fetch(url, {
+        "method": "POST",
+        "body": formData,
+    }).then(response => response.json().then(data => {
+        const isNowFavourite = data["favourite"];
+        if (isNowFavourite) {
+            target.classList.replace("bi-star", "bi-star-fill");
+        } else {
+            target.classList.replace("bi-star-fill", "bi-star");
+        }
+    }));
+}
+addHandler(".favourite-star", "click", toggleTrackFavourite);
+/**
+ * Returns an array of localized month names (Jan-Dec).
+ */
+function getLocalizedMonthNames() {
+    const monthNames = [];
+    const date = new Date(2000, 0);
+    for (let i = 0; i < 12; i++) {
+        monthNames.push(date.toLocaleString(LOCALE, {
+            month: 'long'
+        }));
+        date.setMonth(i + 1);
+    }
+    return monthNames;
+}
+/**
+ * Load and plot the user's summary.
+ */
+function loadProfileStats() {
+    const monthNames = getLocalizedMonthNames();
+    const url = makeUrl("me/summary.json");
+    fetch(url)
+        .then(response => response.json())
+        .then((response) => {
+            const datasets = [];
+            for (const [year, months] of Object.entries(response)) {
+                const data = [];
+                for (let i = 1; i <= 12; ++i) {
+                    data.push((i in months) ? (months[i] / 1000) : 0);
+                }
+                datasets.push({
+                    data: data,
+                    label: year,
+                });
+            }
+            new Chart("graph-month-summary", {
+                type: "bar",
+                data: {
+                    datasets: datasets,
+                    labels: monthNames,
+                },
+            });
+        });
+}
+/* Used via in-page scripts, so make eslint happy */
+loadProfileStats;
 document.addEventListener('DOMContentLoaded', function() {
     window.fietsboekImageIndex = 0;
     /* Enable tooltips */
     const tooltipTriggerList = [].slice.call(document.querySelectorAll('[data-bs-toggle="tooltip"]'));
     tooltipTriggerList.map((tooltipTriggerEl) => {
         return new bootstrap.Tooltip(tooltipTriggerEl, {
             sanitize: false
```

### Comparing `fietsboek-0.8.0/fietsboek/static/fietsboek.js.map` & `fietsboek-0.9.0/fietsboek/static/fietsboek.js.map`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'mappings'": "';AAqBA,kDAAkD;AAClD,CAAC,CAAS,EAAE,EAAE,CAAC,IAAI,CAAC;AAQpB;;;;;GAKG;AACH,SAAS,SAAS,CAAC,IAAY;;IAC3B,OAAO,MAAA,QAAQ,CAAC,MAAM,CAAC,KAAK,CAAC,IAAI,CAAC;SAC7B,IAAI,CAAC,CAAC,GAAG,EAAE,EAAE,CAAC,GAAG,CAAC,UAAU,CAAC,GAAG,IAAI,GAAG,CAAC,CAAC,0CACxC,KAAK,CAAC,GAAG,EAAE,CAAC,CAAC,CAAC;AACxB,CAAC;AAGD;;;;;;;GAOG;AACH,SAAS,OAAO,CAAC,IAAY;IACzB,OAAO,IAAI,GAAG,CAAC,IAAI,EAAE,QAAQ,CAAC,CAAC;AACnC,CAAC;AAED;;;;;;GAMG;AACH,SAAS,UAAU,CACf,QAAkB,EAClB,KAAQ,EACR,OAAoD;IAEpD,QAAQ,CAAC,gBAAgB,CAAC,QAAQ,CAAC; […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "fietsboek.js",
-    "mappings": "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",
+    "mappings": "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",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "../../asset-sources/fietsboek.ts"
     ],
     "version": 3
 }
```

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/bootstrap-icons.woff` & `fietsboek-0.9.0/fietsboek/static/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/bootstrap-icons.woff2` & `fietsboek-0.9.0/fietsboek/static/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-300.woff` & `fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-300.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-300.woff2` & `fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-300.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-300italic.woff` & `fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-300italic.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-300italic.woff2` & `fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-300italic.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-500.woff` & `fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-500.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-500.woff2` & `fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-500.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-500italic.woff` & `fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-500italic.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-500italic.woff2` & `fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-500italic.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-600.woff` & `fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-600.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-600.woff2` & `fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-600.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-600italic.woff` & `fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-600italic.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-600italic.woff2` & `fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-600italic.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-700.woff` & `fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-700.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-700.woff2` & `fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-700italic.woff` & `fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-700italic.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-700italic.woff2` & `fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-700italic.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-800.woff` & `fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-800.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-800.woff2` & `fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-800.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-800italic.woff` & `fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-800italic.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-800italic.woff2` & `fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-800italic.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-italic.woff` & `fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-italic.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-italic.woff2` & `fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-regular.woff` & `fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-regular.woff2` & `fietsboek-0.9.0/fietsboek/static/fonts/open-sans-v29-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/fonts.css` & `fietsboek-0.9.0/fietsboek/static/fonts.css`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/osm-monkeypatch.js` & `fietsboek-0.9.0/fietsboek/static/osm-monkeypatch.js`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/static/theme.css.map` & `fietsboek-0.9.0/fietsboek/static/theme.css.map`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'mappings'": "'AAAA;EACE;;;AAGF;EACE;EACA;EACA;EACA;EACA;EACA;EACA;;;AAGF;EACE;;;AAGF;EACE;;;AAGF;EACE;;;AAGF;EACE;;AAEA;EACE;EACA;EACA;;;AAIJ;EACE;;;AAGF;EACE;EACA;EACA;EACA;EACA;EACA;;;AAGF;EACE;EACA;;;AAGF;EACE;;;AAGF;EACE;EACA;;;AAGF;EAqCE;EACA;EACA;EACA;EACA;EACA;;AAzCA;EACE;EACA;EACA;EACA;;AAGF;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;AAGF;EACE;EACA;;AAGF;EACE;EACA;EACA;EACA;EACA;EACA;;;AAWJ;EACI;;;AAGJ;EACE;;;AAGF;EACE;EACA;;;AAGF;EACE;EACA;;;AAGF;EACE;;;AAGF;EACE;EACA;EACA;;AAE […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "theme.css",
-    "mappings": "AAAA;EACE;EACA;EACA;EACA;;;AAGF;EACE;;;AAGF;EACE;;;AAGF;EACE;EACA;EACA;EACA;EACA;EACA;;;AAGF;EACE;EACA;;;AAGF;EACE;;;AAGF;EACE;EACA;;;AAGF;EAqCE;EACA;EACA;EACA;EACA;EACA;;AAzCA;EACE;EACA;EACA;EACA;;AAGF;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;AAGF;EACE;EACA;;AAGF;EACE;EACA;EACA;EACA;EACA;EACA;;;AAWJ;EACI;;;AAGJ;EACE;;;AAGF;EACE;EACA;;;AAGF;EACE;EACA;;;AAGF;EACE;;;AAGF;EACE;EACA;EACA;;AAEA;EACE;EACA;;AAGF;EACE;;;AAIJ;AACA;EACE;;;AAGF;EACE;EACA;;;AAGF;EACE;;;AAGF;EACE;EACA;;;AAGF;EACE;;;AAGF;EACE;;;AAGF;EACE",
+    "mappings": "AAAA;EACE;;;AAGF;EACE;EACA;EACA;EACA;EACA;EACA;EACA;;;AAGF;EACE;;;AAGF;EACE;;;AAGF;EACE;;;AAGF;EACE;;AAEA;EACE;EACA;EACA;;;AAIJ;EACE;;;AAGF;EACE;EACA;EACA;EACA;EACA;EACA;;;AAGF;EACE;EACA;;;AAGF;EACE;;;AAGF;EACE;EACA;;;AAGF;EAqCE;EACA;EACA;EACA;EACA;EACA;;AAzCA;EACE;EACA;EACA;EACA;;AAGF;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;AAGF;EACE;EACA;;AAGF;EACE;EACA;EACA;EACA;EACA;EACA;;;AAWJ;EACI;;;AAGJ;EACE;;;AAGF;EACE;EACA;;;AAGF;EACE;EACA;;;AAGF;EACE;;;AAGF;EACE;EACA;EACA;;AAEA;EACE;EACA;;AAGF;EACE;;;AAIJ;EACE;;;AAGF;EACE;;;AAGF;AACA;EACE;;;AAGF;EACE;;;AAGF;EACE;EACA;;;AAGF;EACE;;;AAGF;EACE;EACA;;;AAGF;EACE;;;AAGF;EACE;;;AAGF;EACE",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "../../asset-sources/theme.scss"
     ],
     "version": 3
 }
```

### Comparing `fietsboek-0.8.0/fietsboek/summaries.py` & `fietsboek-0.9.0/fietsboek/summaries.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module for a yearly/monthly track summary."""
+
 from typing import Dict, List
 
 from fietsboek.models.track import TrackWithMetadata
 
 
 class Summary:
     """A summary of a user's tracks.
```

### Comparing `fietsboek-0.8.0/fietsboek/templates/admin.jinja2` & `fietsboek-0.9.0/fietsboek/templates/admin.jinja2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/templates/browse.jinja2` & `fietsboek-0.9.0/fietsboek/templates/browse.jinja2`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,25 @@
         <div class="input-group">
           <button type="button" class="btn btn-outline-secondary button-clear-input"><i class="bi bi-eraser-fill"></i></button>
           <select class="form-select" size="2" name="type[]" multiple>
             <option value="ORGANIC"{% if "ORGANIC" in request.params.getall("type[]") %} selected{% endif %}>{{ _("page.browse.filter.type.organic") }}</option>
             <option value="SYNTHETIC"{% if "SYNTHETIC" in request.params.getall("type[]") %} selected{% endif %}>{{ _("page.browse.filter.type.synthetic") }}</option>
           </select>
         </div>
+
+        {% if request.identity %}
+        <div class="input-group mt-2">
+          <button type="button" class="btn btn-outline-secondary button-clear-input"><i class="bi bi-eraser-fill"></i></button>
+          <select class="form-select" name="favourite">
+            <option value="">{{ _("page.browse.filter.favourite.all") }}</option>
+            <option value="true"{% if request.params.get("favourite") == "true" %} selected{% endif %}>{{ _("page.browse.filter.favourite.yes") }}</option>
+            <option value="false"{% if request.params.get("favourite") == "false" %} selected{% endif %}>{{ _("page.browse.filter.favourite.no") }}</option>
+          </select>
+        </div>
+        {% endif %}
       </div>
       <div class="col-md-6">
         {% if request.identity %}
         {% macro render_switch(id, name, value, text) %}
         <div class="form-check form-switch">
           <input class="form-check-input" type="checkbox" role="switch" id="{{ id }}" name="{{ name }}" value="{{ value }}" {% if value in request.params.getall(name) %}checked{% endif %}>
           <label class="form-check-label" for="{{ id }}">{{ text }}</label>
@@ -119,14 +130,19 @@
     </form>
   </div>
   {% if tracks %}
   {% for track in tracks %}
   <div class="card mb-3">
     <h5 class="card-header">
       <input type="checkbox" class="form-check-input archive-checkbox" name="track_id[]" value="{{ track.id }}">
+      {% if request.identity and request.identity in track.favourees %}
+      <i class="bi bi-star-fill favourite-star" data-track-id="{{ track.id }}"></i>
+      {% else %}
+      <i class="bi bi-star favourite-star" data-track-id="{{ track.id }}"></i>
+      {% endif %}
       <a href="{{ request.route_url('details', track_id=track.id) }}">{{ track.title | default(track.date, true) }}</a>
       {% if track.text_tags() %}
       {% for tag in track.tags %}<span class="badge bg-info text-dark">{{ tag.tag }}</span> {% endfor %}
       {% endif %}
       <span class="float-end">
         {% if track.show_organic_data() %}
         <i class="bi bi-cassette" title="{{ _("page.browse.organic_tooltip") }}"></i>
```

### Comparing `fietsboek-0.8.0/fietsboek/templates/create_account.jinja2` & `fietsboek-0.9.0/fietsboek/templates/create_account.jinja2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/templates/details.jinja2` & `fietsboek-0.9.0/fietsboek/templates/details.jinja2`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 {% extends "layout.jinja2" %}
 {% import "util.jinja2" as util with context %}
 
 {% block content %}
 <div class="container">
-  <h1>{{ track.title | default(_("page.details.title"), true) }}</h1>
+  <h1>
+    {{ track.title | default(_("page.details.title"), true) }}
+    {% if request.identity %}
+    <span style="display: inline-flex; vertical-align: middle;">
+    {% if request.identity in track.favourees %}
+    <i class="bi bi-star-fill favourite-star" data-track-id="{{ track.id }}"></i>
+    {% else %}
+    <i class="bi bi-star favourite-star" data-track-id="{{ track.id }}"></i>
+    {% endif %}
+    </span>
+    {% endif %}
+  </h1>
   {% if show_edit_link %}
   <div class="btn-group" role="group">
     <a class="btn btn-success" href="{{ request.route_path('edit', track_id=track.id) }}"><i class="bi-pencil-square"></i> {{ _("page.details.edit") }}</a>
     <button type="button" class="btn btn-info" id="showShareLink" data-bs-toggle="modal" data-bs-target="#shareLinkModal"><i class="bi-share"></i> {{ _("page.details.share") }}</button>
     <button type="button" class="btn btn-danger" id="deleteLink" data-bs-toggle="modal" data-bs-target="#deleteModal"><i class="bi bi-trash"></i> {{ _("page.details.delete") }}</button>
   </div>
   <div class="modal fade" id="shareLinkModal" tabindex="-1" aria-hidden="true">
@@ -78,15 +89,17 @@
   {% endif %}
   <div id="mainmap" class="gpxview:{{ gpx_url }}:OSM" style="width:100%;height:600px">
     <noscript><p>{{ _("page.noscript") }}<p></noscript>
   </div>
   <div id="mainmap_hp" style="width:100%;height:300px">
   </div>
 
-  <a class="btn btn-primary" href="{{ gpx_url }}"><i class="bi bi-download"></i> {{ _("page.details.download") }}</a>
+  <div class="mb-3">
+    <a class="btn btn-primary" href="{{ gpx_url }}"><i class="bi bi-download"></i> {{ _("page.details.download") }}</a>
+  </div>
 
   <table class="table table-hover table-sm">
     <tbody>
       <tr>
         <th scope="row">{{ _("page.details.date") }}</th>
         <td id="detailsDate">{{ track.date | format_datetime }}</td>
       </tr>
```

#### html2text {}

```diff
@@ -1,10 +1,12 @@
 {% extends "layout.jinja2" %} {% import "util.jinja2" as util with context %}
 {% block content %}
-************ {{{{ ttrraacckk..ttiittllee || ddeeffaauulltt((__((""ppaaggee..ddeettaaiillss..ttiittllee"")),, ttrruuee)) }}}} ************
+{{{{ ttrraacckk..ttiittllee || ddeeffaauulltt((__((""ppaaggee..ddeettaaiillss..ttiittllee"")),, ttrruuee)) }}}} {{%% iiff
+rreeqquueesstt..iiddeennttiittyy %%}} {{%% iiff rreeqquueesstt..iiddeennttiittyy iinn ttrraacckk..ffaavvoouurreeeess %%}} {{%% eellssee %%}} {{%%
+eennddiiff %%}} {{%% eennddiiff %%}}
 {% if show_edit_link %}
 _{_{_ ___(_"_p_a_g_e_._d_e_t_a_i_l_s_._e_d_i_t_"_)_ _}_}
  {{ _("page.details.share") }} {{ _("page.details.delete") }}
 **** {{{{ __((""ppaaggee..ddeettaaiillss..sshhaarreelliinnkk..ttiittllee"")) }}}} ****
 {{ _("page.details.sharelink.info") }}
 {% set share_link = request.route_url('details', track_id=track.id, _query=[
 ("secret", track.link_secret)]) %} _{_{_ _s_h_a_r_e___l_i_n_k_ _}_}
```

### Comparing `fietsboek-0.8.0/fietsboek/templates/edit.jinja2` & `fietsboek-0.9.0/fietsboek/templates/edit.jinja2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/templates/edit_form.jinja2` & `fietsboek-0.9.0/fietsboek/templates/edit_form.jinja2`

 * *Files 4% similar despite different names*

```diff
@@ -67,25 +67,27 @@
       <input type="text" id="friendSearchQuery" class="form-control">
     </div>
     <div class="col-lg-3">
       <button type="button" class="btn btn-primary" id="add-friend-btn"><i class="bi bi-search"></i> {{ _("page.track.form.add_friend") }}</buttton>
     </div>
   </div>
   <!-- Hidden templates for Javascript to use -->
-  <div style="display: none;">
-    <li class="list-group-item friendlist-control" id="friendSearchBlueprint">
+  <template id="friendSearchBlueprint">
+    <li class="list-group-item friendlist-control">
       <button type="button" class="btn btn-success"><i class="bi bi-plus-square-fill"></i></button>
       <span class="friend-name"></span>
     </li>
-    <li class="list-group-item friendlist-control" id="friendAddedBlueprint">
+  </template>
+  <template id="friendAddedBlueprint">
+    <li class="list-group-item friendlist-control">
       <button type="button" class="btn btn-danger remove-friend-button"><i class="bi bi-x-square-fill"></i></button>
       <input name="tagged-friend[]" type="hidden" disabled>
       <span class="friend-name"></span>
     </li>
-  </div>
+  </template>
   <!-- End of templates -->
   <ul class="list-group" id="friendSearch">
   </ul>
 </div>
 <div class="mb-3">
   <div>{{ _("page.track.form.badges") }}</div>
   {% for (state, badge) in badges %}
@@ -110,25 +112,32 @@
       <input type="hidden" class="image-description-input" name="image-description[{{ image.name }}]" value="{{ image.description }}">
       <input type="hidden" class="image-deleter-input" name="delete-image[]" value="{{ image.name }}" disabled>
       <img src="{{ image.url }}" title="{{ image.description }}">
     </div>
     {% endfor %}
   </div>
   <input type="file" name="image[]" id="imageSelector" class="form-control" accept="image/*" style="display:none;" multiple>
-  <button type="button" onclick="document.querySelector('#imageSelector').click()" class="btn btn-primary"><i class="bi bi-images"></i> {{ _("page.track.form.select_images") }}</button>
+  <button type="button" onclick="document.querySelector('#imageSelector').click()" class="btn btn-primary" id="selectImagesButton" {% if not request.config.enable_image_uploads %}disabled{% endif %}>
+      <i class="bi bi-images"></i> {{ _("page.track.form.select_images") }}
+  </button>
+  {% if not request.config.enable_image_uploads %}
+  <span class="text-info">
+      <i class="bi bi-info-circle-fill"></i> {{ _("page.track.form.image_uploads_disabled") }}
+  </span>
+  {% endif %}
 </div>
 <!-- Mode hidden templates -->
-<div style="display:none;">
-  <div id="trackImagePreviewBlueprint" class="track-image-preview">
+<template id="trackImagePreviewBlueprint">
+  <div class="track-image-preview">
     <button type="button" class="btn-close delete-image" aria-label="{{ _("page.track.form.remove_image") }}"></button>
     <button type="button" class="edit-image-description"><i class="bi bi-cursor-text"></i></button>
     <input type="hidden" class="image-description-input" name="image-description[]" value="">
     <img>
   </div>
-</div>
+</template>
 <!-- Edit image description modal -->
 <div class="modal" tabindex="-1" id="imageDescriptionModal">
   <div class="modal-dialog">
     <div class="modal-content">
       <div class="modal-header">
         <h5 class="modal-title">{{ _("page.track.form.image_description_modal") }}</h5>
         <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
```

### Comparing `fietsboek-0.8.0/fietsboek/templates/finish_upload.jinja2` & `fietsboek-0.9.0/fietsboek/templates/finish_upload.jinja2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/templates/home.jinja2` & `fietsboek-0.9.0/fietsboek/templates/home.jinja2`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,25 @@
       <div class="list-group collapse show">
         {% for track in month %}
         <span class="list-group-item">
           {{ track.date.day }}:
           <a href="{{ request.route_url('details', track_id=track.id) }}" data-bs-toggle="tooltip" data-bs-container="body" data-bs-html="true" title="{{ track.html_tooltip(request.localizer) }}">
             {{ track.title | default(track.date, true) }}
           </a>
-          <span class="float-end">{{ (track.length / 1000) | round(2) | format_decimal }} km</span>
+          {% if request.identity in track.favourees %}
+          <i class="bi bi-star-fill favourite-star-ni"></i>
+          {% endif %}
+          <span class="float-end">
+              {% if track.tagged_people %}
+              <span data-bs-toggle="tooltip" data-bs-container="body" data-bs-html="true" title="{{ track.html_tooltip_tagged_people() }}">
+                  {{ track.tagged_people | length + 1 }} <i class="bi bi-people-fill"></i> &nbsp;
+              </span>
+              {% endif %}
+              {{ (track.length / 1000) | round(2) | format_decimal }} km
+          </span>
         </span>
         {% endfor %}
       </div>
       {% endfor %}
     </div>
     {% endfor %}
   </div>
```

#### html2text {}

```diff
@@ -14,16 +14,17 @@
 "page.home.summary.tracks", year|length) }} — {{ (year.total_length / 1000) |
 round(2) | format_decimal }} km
 {% for month in year %}
 {{ month_name(request, month.month) }} {{ ngettext("page.home.summary.track",
 "page.home.summary.tracks", month|length) }} — {{ (month.total_length / 1000) |
 round(2) | format_decimal }} km
 {% for track in month %} {{ track.date.day }}: _{_{_ _t_r_a_c_k_._t_i_t_l_e_ _|_ _d_e_f_a_u_l_t
-_(_t_r_a_c_k_._d_a_t_e_,_ _t_r_u_e_)_ _}_}_ {{ (track.length / 1000) | round(2) | format_decimal }}
-km {% endfor %}
+_(_t_r_a_c_k_._d_a_t_e_,_ _t_r_u_e_)_ _}_}_ {% if request.identity in track.favourees %} {% endif %}
+{% if track.tagged_people %} {{ track.tagged_people | length + 1 }}   {% endif
+%} {{ (track.length / 1000) | round(2) | format_decimal }} km {% endfor %}
 {% endfor %}
 {% endfor %}
 {{ _("page.home.total") }}: {{ ngettext("page.home.summary.track",
 "page.home.summary.tracks", summary|length) }}, {{ (summary.total_length /
 1000) | round(2) | format_decimal }} km
 {% elif home_content %} {{ home_content | safe }} {% endif %}
 {% endblock %}
```

### Comparing `fietsboek-0.8.0/fietsboek/templates/layout.jinja2` & `fietsboek-0.9.0/fietsboek/templates/layout.jinja2`

 * *Files 4% similar despite different names*

```diff
@@ -108,24 +108,41 @@
 
     {% for message in request.session.pop_flash() %}
     <div class="alert alert-primary" role="alert">
       {{message}}
     </div>
     {% endfor %}
 
+    <div id="mainContent">
     {% block content %}
     {% endblock %}
+    </div>
+
+    <footer id="siteFooter">
+      <div class="container">
+        <hr>
+        <div id="languageChooser">
+          {% for lang_code, display_name in list_languages(request) %}
+          <a href="#" class="language-choice" data-langcode="{{ lang_code }}">{{ display_name }}</a>
+          {% endfor %}
+        </div>
+      </div>
+    </footer>
+
     <!-- Bootstrap core JavaScript
     ================================================== -->
     <!-- Placed at the end of the document so the pages load faster -->
     <script src="{{request.static_url('fietsboek:static/bootstrap.bundle.min.js')}}"></script>
     <!-- Pre-load leaflet Javascript. This lets us use Leaflet on any page, without relying on GPXViewer to load it -->
     <script src="{{request.static_url('fietsboek:static/GM_Utils/leaflet/leaflet.js')}}"></script>
     <!-- Our patch to the GPX viewer, load before the actual GPX viewer -->
     <script src="{{request.static_url('fietsboek:static/osm-monkeypatch.js')}}"></script>
     <!-- Jürgen Berkemeier's GPX viewer -->
     <script src="{{request.static_url('fietsboek:static/GM_Utils/GPX2GM.js')}}"></script>
+    <!-- Chart.JS -->
+    <script src="{{request.static_url('fietsboek:static/chart.umd.js')}}"></script>
+
     <script src="{{request.static_url('fietsboek:static/fietsboek.js')}}"></script>
     {% block latescripts %}
     {% endblock %}
   </body>
 </html>
```

#### html2text {}

```diff
@@ -22,9 +22,13 @@
           o {% endif %} {% else %} {# Items shown to not-logged-in users #}
           o _{_{_ ___(_"_p_a_g_e_._n_a_v_b_a_r_._l_o_g_i_n_"_)_ _}_}
           o {% if request.config.enable_account_registration %}
           o _{_{_ ___(_"_p_a_g_e_._n_a_v_b_a_r_._c_r_e_a_t_e___a_c_c_o_u_n_t_"_)_ _}_}
           o {% endif %} {% endif %}
 {% for message in request.session.pop_flash() %}
 {{message}}
-{% endfor %} {% block content %} {% endblock %}
+{% endfor %}
+{% block content %} {% endblock %}
+===============================================================================
+{% for lang_code, display_name in list_languages(request) %} _{_{_ _d_i_s_p_l_a_y___n_a_m_e_ _}_}
+{% endfor %}
 {% block latescripts %} {% endblock %}
```

### Comparing `fietsboek-0.8.0/fietsboek/templates/login.jinja2` & `fietsboek-0.9.0/fietsboek/templates/login.jinja2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/templates/password_reset.jinja2` & `fietsboek-0.9.0/fietsboek/templates/password_reset.jinja2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/templates/profile.jinja2` & `fietsboek-0.9.0/fietsboek/templates/profile.jinja2`

 * *Files 20% similar despite different names*

```diff
@@ -54,77 +54,113 @@
   </div>
 {% endmacro %}
 
 {% block content %}
 <div class="container">
   <h1>{{ user.name }}</h1>
 
-  {% if heatmap_url or tilehunt_url %}
-  <div id="userMap" style="height: 600px; width: 100%;"></div>
-  {% endif %}
-
-  <table class="table table-hover table-sm">
-    <th scope="row">{{ _("page.profile.length") }}</th>
-      <td id="profileLength">{{ (total.length / 1000) | round(2) | format_decimal }} km</td>
-    </tr>
-    <tr>
-      <th scope="row">{{ _("page.profile.uphill") }}</th>
-      <td id="profileUphill">{{ total.uphill | round(2) | format_decimal }} m</td>
-    </tr>
-    <tr>
-      <th scope="row">{{ _("page.profile.downhill") }}</th>
-      <td id="profileDownhill">{{ total.downhill | round(2) | format_decimal }} m</td>
-    </tr>
-    <tr>
-      <th scope="row">{{ _("page.profile.moving_time") }}</th>
-      <td id="profileMovingTime">{{ total.moving_time }}</td>
-    </tr>
-    <tr>
-      <th scope="row">{{ _("page.profile.stopped_time") }}</th>
-      <td id="profileStoppedTime">{{ total.stopped_time }}</td>
-    </tr>
-    <tr>
-      <th scope="row">{{ _("page.profile.max_speed") }}</th>
-      <td id="profileMaxSpeed">{{ mps_to_kph(total.max_speed) | round(2) | format_decimal }} km/h</td>
-    </tr>
-    <tr>
-      <th scope="row">{{ _("page.profile.avg_speed") }}</th>
-      <td id="profileAvgSpeed">{{ mps_to_kph(total.avg_speed) | round(2) | format_decimal }} km/h</td>
-    </tr>
-    <tr>
-      <th scope="row">{{ _("page.profile.number_of_tracks") }}</th>
-      <td id="profileNumberOfTracks">{{ total.count }}</td>
-    </tr>
-  </table>
-
-  {% if total.longest_distance_track %}
-  <h2>{{ _("page.profile.longest_distance_track") }}</h2>
-  {{ render_track_card(total.longest_distance_track) }}
-  {% endif %}
-
-  {% if total.shortest_distance_track %}
-  <h2>{{ _("page.profile.shortest_distance_track") }}</h2>
-  {{ render_track_card(total.shortest_distance_track) }}
-  {% endif %}
-
-  {% if total.longest_duration_track %}
-  <h2>{{ _("page.profile.longest_duration_track") }}</h2>
-  {{ render_track_card(total.longest_duration_track) }}
-  {% endif %}
-
-  {% if total.shortest_duration_track %}
-  <h2>{{ _("page.profile.shortest_duration_track") }}</h2>
-  {{ render_track_card(total.shortest_duration_track) }}
-  {% endif %}
+  <ul class="nav nav-tabs" id="profileTabbar" role="tablist">
+    <li class="nav-item" role="presentation">
+      <button class="nav-link active" id="tabOverviewButton" data-bs-toggle="tab" data-bs-target="#tabOverviewPane" type="button" role="tab" aria-controls="tabOverviewPane" aria-selected="true">
+        {{ _("page.profile.tabbar.overview") }}
+      </button>
+    </li>
+    <li class="nav-item" role="presentation">
+      <button class="nav-link" id="tabGraphsButton" data-bs-toggle="tab" data-bs-target="#tabGraphsPane" type="button" role="tab" aria-controls="tabGraphsPane" aria-selected="false">
+        {{ _("page.profile.tabbar.graphs") }}
+      </button>
+    </li>
+  </ul>
+
+  <div class="tab-content">
+    <!-- First tab -->
+    <div class="tab-pane fade show active" id="tabOverviewPane" role="tabpanel" aria-labelledby="tabOverviewButton">
+      {% if heatmap_url or tilehunt_url %}
+      <div id="userMap" style="height: 600px; width: 100%;"></div>
+      {% endif %}
+
+      <table class="table table-hover table-sm">
+        <tr>
+          <th scope="row">{{ _("page.profile.length") }}</th>
+          <td id="profileLength">{{ (total.length / 1000) | round(2) | format_decimal }} km</td>
+        </tr>
+        <tr>
+          <th scope="row">{{ _("page.profile.avg_length") }}</th>
+          <td id="profileAvgLength">{{ (total.avg_length / 1000) | round(2) | format_decimal }} km</td>
+        </tr>
+        <tr>
+          <th scope="row">{{ _("page.profile.uphill") }}</th>
+          <td id="profileUphill">{{ total.uphill | round(2) | format_decimal }} m</td>
+        </tr>
+        <tr>
+          <th scope="row">{{ _("page.profile.downhill") }}</th>
+          <td id="profileDownhill">{{ total.downhill | round(2) | format_decimal }} m</td>
+        </tr>
+        <tr>
+          <th scope="row">{{ _("page.profile.moving_time") }}</th>
+          <td id="profileMovingTime">{{ total.moving_time }}</td>
+        </tr>
+        <tr>
+          <th scope="row">{{ _("page.profile.stopped_time") }}</th>
+          <td id="profileStoppedTime">{{ total.stopped_time }}</td>
+        </tr>
+        <tr>
+          <th scope="row">{{ _("page.profile.avg_duration") }}</th>
+          <td id="profileAvgDuration">{{ total.avg_duration }}</td>
+        </tr>
+        <tr>
+          <th scope="row">{{ _("page.profile.max_speed") }}</th>
+          <td id="profileMaxSpeed">{{ mps_to_kph(total.max_speed) | round(2) | format_decimal }} km/h</td>
+        </tr>
+        <tr>
+          <th scope="row">{{ _("page.profile.avg_speed") }}</th>
+          <td id="profileAvgSpeed">{{ mps_to_kph(total.avg_speed) | round(2) | format_decimal }} km/h</td>
+        </tr>
+        <tr>
+          <th scope="row">{{ _("page.profile.number_of_tracks") }}</th>
+          <td id="profileNumberOfTracks">{{ total.count }}</td>
+        </tr>
+      </table>
+
+      {% if total.longest_distance_track %}
+      <h2>{{ _("page.profile.longest_distance_track") }}</h2>
+      {{ render_track_card(total.longest_distance_track) }}
+      {% endif %}
+
+      {% if total.shortest_distance_track %}
+      <h2>{{ _("page.profile.shortest_distance_track") }}</h2>
+      {{ render_track_card(total.shortest_distance_track) }}
+      {% endif %}
+
+      {% if total.longest_duration_track %}
+      <h2>{{ _("page.profile.longest_duration_track") }}</h2>
+      {{ render_track_card(total.longest_duration_track) }}
+      {% endif %}
+
+      {% if total.shortest_duration_track %}
+      <h2>{{ _("page.profile.shortest_duration_track") }}</h2>
+      {{ render_track_card(total.shortest_duration_track) }}
+      {% endif %}
+    </div>
+
+    <!-- Second tab -->
+    <div class="tab-pane fade" id="tabGraphsPane" role="tabpanel" aria-labelledby="tabGraphsButton">
+      <h2 class="chart-title">{{ _("page.profile.graph.km_per_month") }}</h2>
+      <div style="position: relative; height: 500px; width: 75%; margin: auto;"><canvas id="graph-month-summary"></canvas></div>
+    </div>
+  </div>
+
 </div>
 {% endblock %}
 
 {% block latescripts %}
 <script>
   (function() {
+    loadProfileStats();
+
     const renderMap = document.getElementById("userMap") !== null;
     if (!renderMap) {
       return;
     }
 
     const map = L.map("userMap").setView([52.520008, 13.404954], 2);
```

### Comparing `fietsboek-0.8.0/fietsboek/templates/request_password.jinja2` & `fietsboek-0.9.0/fietsboek/templates/request_password.jinja2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/templates/resend_verification.jinja2` & `fietsboek-0.9.0/fietsboek/templates/resend_verification.jinja2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/templates/upload.jinja2` & `fietsboek-0.9.0/fietsboek/templates/upload.jinja2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/templates/user_data.jinja2` & `fietsboek-0.9.0/fietsboek/templates/user_data.jinja2`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,25 @@
     </div>
     {{ util.hidden_csrf_input() }}
     <button type="submit" class="btn btn-primary"><i class="bi bi-save"></i> {{ _("page.my_profile.personal_data.save") }}</button>
   </form>
 
   <hr>
 
+  <h2>{{ _("page.my_profile.session_logout.title") }}</h2>
+
+  <p>{{ _("page.my_profile.session_logout.explanation") }}</p>
+
+  <form method="POST" action="{{ request.route_path('force-logout') }}">
+    {{ util.hidden_csrf_input() }}
+    <button type="submit" class="btn btn-danger"><i class="bi bi-shield-lock-fill"></i> {{ _("page.my_profile.session_logout.button") }}</button>
+  </form>
+
+  <hr>
+
   <h2>{{ _("page.my_profile.friends") }}</h2>
 
   <ul class="list-group">
     {% for friend in user.get_friends() %}
     <li class="list-group-item d-flex align-items-center">
       <form action="{{ request.route_url('delete-friend') }}" method="POST">
         <input type="hidden" name="friend-id" value="{{ friend.id }}">
```

### Comparing `fietsboek-0.8.0/fietsboek/transformers/__init__.py` & `fietsboek-0.9.0/fietsboek/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.8.0/fietsboek/transformers/breaks.py` & `fietsboek-0.9.0/fietsboek/transformers/breaks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Transformers that deal with breaks in the track."""
+
 import datetime
 
 from gpxpy.gpx import GPX, GPXTrack
 from pyramid.i18n import TranslationString
 
 from . import Parameters, Transformer
```

### Comparing `fietsboek-0.8.0/fietsboek/transformers/elevation.py` & `fietsboek-0.9.0/fietsboek/transformers/elevation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Transformers that deal with elevation changes in the track."""
+
 from collections.abc import Callable, Iterable
 from itertools import islice, zip_longest
 
 from gpxpy.gpx import GPX, GPXTrackPoint
 from pyramid.i18n import TranslationString
 
 from . import Parameters, Transformer
```

### Comparing `fietsboek-0.8.0/fietsboek/updater/__init__.py` & `fietsboek-0.9.0/fietsboek/updater/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Updating (data migration) logic for fietsboek."""
+
 import datetime
 import enum
 import importlib.resources
 import importlib.util
 import logging
 import random
 import string
```

### Comparing `fietsboek-0.8.0/fietsboek/updater/cli.py` & `fietsboek-0.9.0/fietsboek/updater/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 While this script does not download and install the latest Fietsboek version
 itself (as this step depends on where you got Fietsboek from), it takes care of
 managing migrations between Fietsboek versions. In particular, the updater
 takes care of running the database migrations, migrating the data directory and
 migrating the configuration.
 """
+
 import logging.config
 
 import click
 
 from ..scripts import config_option
 from . import Updater
```

### Comparing `fietsboek-0.8.0/fietsboek/updater/script.py` & `fietsboek-0.9.0/fietsboek/updater/script.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base class definition for update scripts."""
+
 # Placed in a separate file to avoid cyclic dependencies
 
 
 class UpdateScript:
     """Base class for update scripts.
 
     This class provides stub methods for the update script hooks as well as
```

### Comparing `fietsboek-0.8.0/fietsboek/updater/scripts/upd_20230103_lu8w3rwlz4ddcpms.py` & `fietsboek-0.9.0/fietsboek/updater/scripts/upd_20230103_lu8w3rwlz4ddcpms.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 """
 import datetime
 from pathlib import Path
 
 import brotli
 import gpxpy
 from sqlalchemy import create_engine
+from sqlalchemy.sql import text
 
 from fietsboek.updater.script import UpdateScript
 
 update_id = 'lu8w3rwlz4ddcpms'
 previous = [
     '30ppwg8zi4ujb46f',
 ]
@@ -33,15 +34,15 @@
 
         sql = (
             "SELECT tracks.id, tracks.title, tracks.description, tracks.date_raw, "
             "tracks.date_tz, users.name "
             "FROM tracks, users "
             "WHERE tracks.owner_id = users.id;"
         )
-        for row in connection.execute(sql):
+        for row in connection.execute(text(sql)):
             track_id, title, description, date_raw, date_tz, author_name = row
             if isinstance(date_raw, str):
                 date_raw = datetime.datetime.strptime(date_raw, "%Y-%m-%d %H:%M:%S.%f")
             if date_tz is None:
                 timezone = datetime.timezone.utc
             else:
                 timezone = datetime.timezone(datetime.timedelta(minutes=date_tz))
```

### Comparing `fietsboek-0.8.0/fietsboek/updater/scripts/upd_30ppwg8zi4ujb46f.py` & `fietsboek-0.9.0/fietsboek/updater/scripts/upd_30ppwg8zi4ujb46f.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 class Up(UpdateScript):
     def pre_alembic(self, config):
         engine = create_engine(config["sqlalchemy.url"])
         connection = engine.connect()
         data_dir = Path(config["fietsboek.data_dir"])
 
-        for row in connection.execute("SELECT id, gpx FROM tracks;"):
+        for row in connection.execute(text("SELECT id, gpx FROM tracks;")):
             self.tell(f"Moving GPX data for track {row.id} from database to disk")
             track_dir = data_dir / "tracks" / str(row.id)
             track_dir.mkdir(parents=True, exist_ok=True)
 
             raw_gpx = gzip.decompress(row.gpx)
             gpx_path = track_dir / "track.gpx.br"
             gpx_path.write_bytes(brotli.compress(raw_gpx, quality=5))
```

### Comparing `fietsboek-0.8.0/fietsboek/util.py` & `fietsboek-0.9.0/fietsboek/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Various utility functions."""
+
 import datetime
 import html
 import importlib.resources
 import os
 import re
 import secrets
 import unicodedata
@@ -38,14 +39,17 @@
     "img": {"alt", "src"},
 }
 
 # Arbitrarily chosen, just make sure they are representable
 DEFAULT_START_TIME = datetime.datetime(1977, 5, 25, 8, 0)
 DEFAULT_END_TIME = datetime.datetime(1985, 7, 3, 8, 0)
 
+DISPLAY_NAME_PATH = "DISPLAY_NAME"
+"""Path of the file in a locale resource folder which contains the display name."""
+
 
 _filename_ascii_strip_re = re.compile(r"[^A-Za-z0-9_.-]")
 _windows_device_files = (
     "CON",
     "AUX",
     "COM1",
     "COM2",
@@ -304,14 +308,23 @@
     if repeat_password is not None:
         if repeat_password != password:
             raise ValueError(_("password_constraint.mismatch"))
     if len(password) < 8:
         raise ValueError(_("password_constraint.length"))
 
 
+def _locale_packages(locale_packages: Optional[list[str]] = None) -> list[str]:
+    # We expect this to be "fietsboek", but we are open to forks.
+    my_package = __name__.split(".", 1)[0]
+    packages = [my_package]
+    if locale_packages:
+        packages.extend(locale_packages)
+    return packages
+
+
 def read_localized_resource(
     locale_name: str,
     path: str,
     locale_packages: Optional[List[str]] = None,
     raise_on_error: bool = False,
 ) -> str:
     """Reads a localized resource.
@@ -332,31 +345,57 @@
     """
     locales = [locale_name]
     # Second chance: If the locale is a specific form of a more general
     # locale, try the general locale as well.
     if "_" in locale_name:
         locales.append(locale_name.split("_", 1)[0])
 
-    if locale_packages is None:
-        locale_packages = []
-    locale_packages.insert(0, "fietsboek")
+    locale_packages = _locale_packages(locale_packages)
 
     for locale in locales:
         for package in locale_packages:
             locale_dir = importlib.resources.files(package) / "locale" / locale
             resource_path = locale_dir / path
             try:
                 return resource_path.read_text(encoding="utf-8")
             except (FileNotFoundError, ModuleNotFoundError, NotADirectoryError):
                 pass
     if raise_on_error:
         raise FileNotFoundError(f"Resource {path!r} not found")
     return f"{locale_name}:{path}"
 
 
+def locale_display_name(locale_name: str, locale_packages: Optional[list[str]] = None) -> str:
+    """Reads the display name for the given locale.
+
+    If the name cannot be found, simply returns ``locale_name``.
+
+    :param locale_name: Name of the locale.
+    :param locale_packages: Names of packages in which locale data is searched.
+    """
+    try:
+        return read_localized_resource(locale_name, DISPLAY_NAME_PATH, locale_packages, True)
+    except FileNotFoundError:
+        return locale_name
+
+
+def list_locales(request: Request) -> list[tuple[str, str]]:
+    """Lists all available locales.
+
+    Returns a list of locale name and display name tuples.
+
+    :param request: The Pyramid request for which to list the locales.
+    """
+    locales = []
+    for locale_name in request.config.available_locales:
+        display_name = locale_display_name(locale_name, request.config.language_packs)
+        locales.append((locale_name, display_name))
+    return locales
+
+
 def tile_url(request: Request, route_name: str, **kwargs: str) -> str:
     """Generates a URL for tiles.
 
     This is basically :meth:`request.route_url`, but it keeps the
     ``{x}``/``{y}``/``{z}`` placeholders intact for consumption by Leaflet.
 
     Expects that the URL takes a ``x``, ``y`` and ``z`` parameter.
```

### Comparing `fietsboek-0.8.0/fietsboek/views/account.py` & `fietsboek-0.9.0/fietsboek/views/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Account related endpoints."""
+
 from pyramid.httpexceptions import HTTPForbidden, HTTPFound
 from pyramid.i18n import TranslationString as _
 from pyramid.view import view_config
 
 from .. import actions, models, util
 
 
@@ -56,13 +57,14 @@
     email_addr = request.params["email"]
     if not email_addr:
         request.session.flash(request.localizer.translate(_("flash.invalid_email")))
         return HTTPFound(request.route_url("create-account"))
 
     user = models.User(name=name, email=email_addr)
     user.set_password(password)
+    user.roll_session_secret()
     request.dbsession.add(user)
 
     actions.send_verification_token(request, user)
 
     request.session.flash(request.localizer.translate(_("flash.a_confirmation_link_has_been_sent")))
     return HTTPFound(request.route_url("login"))
```

### Comparing `fietsboek-0.8.0/fietsboek/views/admin.py` & `fietsboek-0.9.0/fietsboek/views/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Admin views."""
+
 from pyramid.httpexceptions import HTTPFound
 from pyramid.i18n import TranslationString as _
 from pyramid.view import view_config
 from sqlalchemy import select
 
 from .. import models
```

### Comparing `fietsboek-0.8.0/fietsboek/views/browse.py` & `fietsboek-0.9.0/fietsboek/views/browse.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Views for browsing all tracks."""
+
 import datetime
 from collections.abc import Callable, Iterable
 from enum import Enum
 from io import RawIOBase
 from typing import TypeVar
 from zipfile import ZIP_DEFLATED, ZipFile
 
 from pyramid.httpexceptions import HTTPBadRequest, HTTPForbidden, HTTPNotFound
 from pyramid.request import Request
 from pyramid.response import Response
 from pyramid.view import view_config
-from sqlalchemy import func, or_, select
+from sqlalchemy import func, not_, or_, select
 from sqlalchemy.orm import aliased
 from sqlalchemy.sql import Select
 
 from .. import models, util
 from ..models.track import TrackType, TrackWithMetadata
 
 T = TypeVar("T", bound=Enum)
@@ -222,14 +223,46 @@
             )
         )
 
     def apply(self, track: TrackWithMetadata) -> bool:
         return track.owner == self.user or self.user in track.tagged_people
 
 
+class FavouriteFilter(Filter):
+    """A :class:`Filter` that accepts only favoured or non-favoured tracks."""
+
+    def __init__(self, user: models.User, favourite: bool):
+        """Sets up the filter.
+
+        :param user: The user for which the favourite status should be checked.
+        :param favourite: ``True`` if only favourites should be returned,
+            ``False`` otherwise.
+        """
+        self.user = user
+        self.favourite = favourite
+
+    def compile(self, query: Select, track: AliasedTrack) -> Select:
+        tfa = models.track.track_favourite_assoc
+        if self.favourite:
+            invert = lambda x: x
+        else:
+            invert = not_
+        return query.where(
+            invert(
+                select(tfa)
+                .where(tfa.c.track_id == track.id)
+                .where(tfa.c.user_id == self.user.id)
+                .exists()
+            )
+        )
+
+    def apply(self, track: TrackWithMetadata) -> bool:
+        return (self.user in track.favourees) == self.favourite
+
+
 class FilterCollection(Filter):
     """A class that applies multiple :class:`Filter`."""
 
     def __init__(self, filters: Iterable[Filter]):
         self._filters = filters
 
     def __bool__(self):
@@ -341,14 +374,18 @@
             filters.append(
                 LambdaFilter(
                     lambda query, track: query.where(track.type.in_(types)),
                     lambda track: track.type in types,
                 )
             )
 
+        if request.identity and request.params.get("favourite"):
+            favourite = request.params.get("favourite") == "true"
+            filters.append(FavouriteFilter(request.identity, favourite))
+
         return cls(filters)
 
 
 def apply_order(query: Select, track: AliasedTrack, order: ResultOrder) -> Select:
     """Applies a ``ORDER BY`` clause to the query.
 
     :raises ValueError: If the given order does not exist.
```

### Comparing `fietsboek-0.8.0/fietsboek/views/default.py` & `fietsboek-0.9.0/fietsboek/views/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Home views."""
+
 from markupsafe import Markup
 from pyramid.httpexceptions import HTTPFound, HTTPNotFound
 from pyramid.i18n import TranslationString as _
 from pyramid.interfaces import ISecurityPolicy
 from pyramid.renderers import render_to_response
 from pyramid.request import Request
 from pyramid.response import Response
@@ -116,21 +117,22 @@
         return HTTPFound(request.route_url("login"))
 
     if not user.is_verified:
         request.session.flash(request.localizer.translate(_("flash.account_not_verified")))
         return HTTPFound(request.route_url("login"))
 
     request.session.flash(request.localizer.translate(_("flash.logged_in")))
-    headers = remember(request, str(user.id))
+    user_id = user.authenticated_user_id()
+    headers = remember(request, user_id)
 
     if request.params.get("remember-me") == "on":
         # We don't want this logic to be the default in
         # SecurityPolicy.remember, so we manually fake it here:
         policy = request.registry.getUtility(ISecurityPolicy)
-        headers += policy.remember_cookie(request, str(user.id))
+        headers += policy.remember_cookie(request, user_id)
 
     response = HTTPFound("/", headers=headers)
     return response
 
 
 @view_config(route_name="logout")
 def logout(request: Request) -> Response:
```

### Comparing `fietsboek-0.8.0/fietsboek/views/detail.py` & `fietsboek-0.9.0/fietsboek/views/detail.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Track detail views."""
+
 import datetime
 import gzip
 import logging
 
 from pyramid.httpexceptions import (
     HTTPFound,
     HTTPInternalServerError,
@@ -11,15 +12,15 @@
 )
 from pyramid.i18n import TranslationString as _
 from pyramid.response import FileResponse, Response
 from pyramid.view import view_config
 from sqlalchemy import select
 
 from .. import models, util
-from ..models.track import TrackWithMetadata
+from ..models.track import Track, TrackWithMetadata
 
 LOGGER = logging.getLogger(__name__)
 
 
 def _sort_key(image_name: str) -> str:
     """Returns the "key" by which the image should be sorted.
 
@@ -87,20 +88,25 @@
     """Returns the actual GPX data from the stored track.
 
     :param request: The Pyramid request.
     :type request: pyramid.request.Request
     :return: The HTTP response.
     :rtype: pyramid.response.Response
     """
-    track = request.context
+    track: Track = request.context
     try:
         manager = request.data_manager.open(track.id)
     except FileNotFoundError:
         LOGGER.error("Track exists in database, but not on disk: %d", track.id)
         return HTTPInternalServerError()
+    if track.title:
+        wanted_filename = f"{track.id} - {util.secure_filename(track.title)}.gpx"
+    else:
+        wanted_filename = f"{track.id}.gpx"
+    content_disposition = f'attachment; filename="{wanted_filename}"'
     # We can be nice to the client if they support it, and deliver the gzipped
     # data straight. This saves decompression time on the server and saves a
     # lot of bandwidth.
     accepted = request.accept_encoding.acceptable_offers(["br", "gzip", "identity"])
     for encoding, _qvalue in accepted:
         if encoding == "br":
             response = FileResponse(
@@ -118,14 +124,15 @@
             break
         if encoding == "identity":
             response = Response(manager.decompress_gpx(), content_type="application/gpx+xml")
             break
     else:
         return HTTPNotAcceptable("No data with acceptable encoding found")
     response.md5_etag()
+    response.content_disposition = content_disposition
     return response
 
 
 @view_config(route_name="invalidate-share", request_method="POST", permission="track.unshare")
 def invalidate_share(request):
     """Endpoint to invalidate the share link.
```

### Comparing `fietsboek-0.8.0/fietsboek/views/edit.py` & `fietsboek-0.9.0/fietsboek/views/edit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Views for editing a track."""
+
 import datetime
 import logging
 from collections import namedtuple
 
 from pyramid.httpexceptions import HTTPBadRequest, HTTPFound
 from pyramid.view import view_config
 from sqlalchemy import select
```

### Comparing `fietsboek-0.8.0/fietsboek/views/profile.py` & `fietsboek-0.9.0/fietsboek/views/profile.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Endpoints for the user profile pages."""
+
 import datetime
+import logging
 import sqlite3
 import urllib.parse
 from dataclasses import dataclass
 from typing import Optional
 
 from pyramid.httpexceptions import HTTPNotFound
 from pyramid.request import Request
@@ -11,14 +13,15 @@
 from pyramid.view import view_config
 from sqlalchemy import select
 from sqlalchemy.orm import aliased
 
 from .. import models, util
 from ..data import UserDataDir
 from ..models.track import TrackType, TrackWithMetadata
+from ..summaries import Summary
 
 # A well-made transparent tile is actually pretty small (only 116 bytes), which
 # is even smaller than our HTTP 404 page. So not only is it more efficient
 # (bandwidth-wise) to transfer the transparent PNG, it also means that we can
 # set cache headers, which the client will honor.
 #
 # Since the tile is so small, we've embedded it right here in the source.
@@ -37,14 +40,16 @@
     0xc1, 0x01, 0x0d, 0x00, 0x00, 0x00, 0xc2, 0xa0, 0xf7, 0x4f, 0x6d, 0x0e,
     0x37, 0xa0, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0xbe, 0x0d,
     0x21, 0x00, 0x00, 0x01, 0x9a, 0x60, 0xe1, 0xd5, 0x00, 0x00, 0x00, 0x00,
     0x49, 0x45, 0x4e, 0x44, 0xae, 0x42, 0x60, 0x82,
 ])
 # fmt: on
 
+LOGGER = logging.getLogger(__name__)
+
 
 @dataclass
 class CumulativeStats:
     """Cumulative user stats.
 
     The values start out with default values, and tracks can be merged in via
     :meth:`add`.
@@ -122,14 +127,31 @@
     @property
     def avg_speed(self) -> float:
         """Average speed, in m/s."""
         if not self.moving_time:
             return 0.0
         return self.length / self.moving_time.total_seconds()
 
+    @property
+    def avg_length(self) -> float:
+        """Average length, in m."""
+        if not self.count:
+            return 0
+        return self.length / self.count
+
+    @property
+    def avg_duration(self) -> datetime.timedelta:
+        """Average duration of a track.
+
+        Note that this property is automatically rounded to seconds.
+        """
+        if not self.count:
+            return datetime.timedelta()
+        return round_to_seconds((self.moving_time + self.stopped_time) / self.count)
+
 
 def round_to_seconds(value: datetime.timedelta) -> datetime.timedelta:
     """Round a timedelta to full seconds.
 
     :param value: The input value.
     :return: The rounded value.
     """
@@ -225,8 +247,30 @@
     result = result.fetchone()
     if result is None:
         return Response(EMPTY_TILE, content_type="image/png")
 
     return Response(result[0], content_type="image/png")
 
 
-__all__ = ["profile", "user_tile"]
+@view_config(
+    route_name="json-summary", request_method="GET", permission="profile.view", renderer="json"
+)
+def json_summary(request: Request) -> Response:
+    """Returns the per-month summary as JSON.
+
+    :param request: The pyramid request.
+    :return: The response, rendered as JSON.
+    """
+    query = request.identity.all_tracks_query()
+    query = select(aliased(models.Track, query)).where(query.c.type == TrackType.ORGANIC)
+    summary = Summary()
+
+    for track in request.dbsession.execute(query).scalars():
+        if track.cache is None:
+            LOGGER.debug("Skipping track %d as it has no cached metadata", track.id)
+            continue
+        summary.add(TrackWithMetadata(track, request.data_manager))
+
+    return {y.year: {m.month: m.total_length for m in y} for y in summary}
+
+
+__all__ = ["profile", "user_tile", "json_summary"]
```

### Comparing `fietsboek-0.8.0/fietsboek/views/tileproxy.py` & `fietsboek-0.9.0/fietsboek/views/tileproxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 While this might slow down the initial load (as we now load everything through
 fietsboek), we can cache the OSM tiles per instance, and we can provide better
 access control for services like thunderforest.com.
 
 Additionally, this protects the users' IP, as only fietsboek can see it.
 """
+
 import datetime
 import logging
-import random
 import threading
 from itertools import chain
 from typing import List, Optional
+from urllib.parse import quote
 
-import pydantic.tools
 import requests
-from pydantic import AnyUrl
+from pydantic import AnyUrl, TypeAdapter
 from pyramid.httpexceptions import HTTPBadRequest, HTTPGatewayTimeout
 from pyramid.request import Request
 from pyramid.response import Response
 from pyramid.view import view_config
 from requests.exceptions import ReadTimeout
 from zope.interface import Interface, implementer
 
@@ -33,15 +33,15 @@
     return f'<a href="{url}" target="_blank">{text}</a>'
 
 
 _jb_copy = _href("https://www.j-berkemeier.de/GPXViewer", "GPXViewer")
 
 
 def _url(value: str) -> AnyUrl:
-    return pydantic.tools.parse_obj_as(AnyUrl, value)
+    return TypeAdapter(AnyUrl).validate_python(value)
 
 
 DEFAULT_TILE_LAYERS = [
     # Main base layers
     TileLayerConfig(
         layer_id="osm",
         name="OSM",
@@ -328,15 +328,25 @@
     timeout_tracker = f"provider-timeout:{provider}"
     if int(request.redis.get(timeout_tracker) or "0") > PUNISHMENT_THRESHOLD:
         # We've gotten too many timeouts from this provider recently, so avoid
         # contacting it in the first place.
         LOGGER.debug("Aborted attempt to contact %s due to previous timeouts", provider)
         raise HTTPGatewayTimeout(f"Avoiding request to {provider}")
 
-    url = tile_sources[provider].url.format(x=x, y=y, z=z, s=random.choice("abc"))
+    url = (
+        tile_sources[provider]
+        .url.unicode_string()
+        .replace(quote("{x}"), str(x))
+        .replace(quote("{y}"), str(y))
+        .replace(quote("{z}"), str(z))
+    )
+    # Avoid doing actual requests during tests
+    if url.startswith("http://localhost:0"):
+        LOGGER.debug("Skipping tile proxy request for testing URL")
+        return Response(b"", content_type="image/png")
     headers = {
         "user-agent": f"Fietsboek-Tile-Proxy/{__VERSION__}",
     }
     from_mail = request.config.email_from
     if from_mail:
         headers["from"] = from_mail
 
@@ -346,15 +356,18 @@
     except ReadTimeout:
         LOGGER.debug("Proxy timeout when accessing %r", url)
         request.redis.incr(timeout_tracker)
         request.redis.expire(timeout_tracker, PUNISHMENT_TTL)
         raise HTTPGatewayTimeout(f"No response in time from {provider}") from None
     except requests.HTTPError as exc:
         LOGGER.info("Proxy request failed for %s: %s", provider, exc)
-        return Response(f"Failed to get tile from {provider}", status_code=exc.response.status_code)
+        status_code = 400
+        if exc.response:
+            status_code = exc.response.status_code
+        return Response(f"Failed to get tile from {provider}", status_code=status_code)
     else:
         request.redis.set(cache_key, resp.content, ex=TTL)
         return Response(resp.content, content_type=resp.headers.get("Content-type", content_type))
 
 
 def sources_for(request: Request) -> List[TileLayerConfig]:
     """Returns all eligible tile sources for the given request.
```

### Comparing `fietsboek-0.8.0/fietsboek/views/upload.py` & `fietsboek-0.9.0/fietsboek/views/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Upload functionality."""
+
 import datetime
 import logging
 
 import gpxpy
 from pyramid.httpexceptions import HTTPBadRequest, HTTPFound
 from pyramid.i18n import TranslationString as _
 from pyramid.response import Response
```

### Comparing `fietsboek-0.8.0/fietsboek/views/user_data.py` & `fietsboek-0.9.0/fietsboek/views/user_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 """Views corresponding to the user profile."""
+
 import datetime
 
 from pyramid.httpexceptions import HTTPForbidden, HTTPFound, HTTPNotFound
 from pyramid.i18n import TranslationString as _
+from pyramid.request import Request
+from pyramid.response import Response
+from pyramid.security import remember
 from pyramid.view import view_config
 from sqlalchemy import select
 
 from .. import models, util
 
 
 @view_config(
@@ -43,26 +47,30 @@
 
     :param request: The Pyramid request.
     :type request: pyramid.request.Request
     :return: The HTTP response.
     :rtype: pyramid.response.Response
     """
     password = request.params["password"]
+    # Save the identity as request.identity will be None after changing the
+    # password.
+    identity = request.identity
     if password:
         try:
             util.check_password_constraints(password, request.params["repeat-password"])
         except ValueError as exc:
             request.session.flash(request.localizer.translate(exc.args[0]))
             return HTTPFound(request.route_url("user-data"))
-        request.identity.set_password(request.params["password"])
+        identity.set_password(request.params["password"])
     name = request.params["name"]
-    if request.identity.name != name:
-        request.identity.name = name
+    if identity.name != name:
+        identity.name = name
     request.session.flash(request.localizer.translate(_("flash.personal_data_updated")))
-    return HTTPFound(request.route_url("user-data"))
+    headers = remember(request, identity.authenticated_user_id())
+    return HTTPFound(request.route_url("user-data"), headers=headers)
 
 
 @view_config(route_name="add-friend", permission="user", request_method="POST")
 def do_add_friend(request):
     """Sends a friend request.
 
     This is the endpoint of a form on the profile overview.
@@ -153,7 +161,37 @@
     :param request: The Pyramid request.
     :type request: pyramid.request.Request
     :return: The HTTP response.
     :rtype: pyramid.response.Response
     """
     friends = [{"name": friend.name, "id": friend.id} for friend in request.identity.get_friends()]
     return friends
+
+
+@view_config(
+    route_name="toggle-favourite", renderer="json", permission="user", request_method="POST"
+)
+def do_toggle_favourite(request: Request) -> dict:
+    """Toggles the favourite status for the given track.
+
+    :param request: The Pyramid request.
+    :return: The data to return to the client.
+    """
+    track = request.dbsession.execute(
+        select(models.Track).filter_by(id=request.params["track-id"])
+    ).scalar_one_or_none()
+    if track is None:
+        return HTTPNotFound()
+    request.identity.toggle_favourite(track)
+    return {"favourite": request.identity in track.favourees}
+
+
+@view_config(route_name="force-logout", permission="user", request_method="POST")
+def do_force_logout(request: Request) -> Response:
+    """Forces all sessions to be logged out.
+
+    :param request: The Pyramid request.
+    :return: The HTTP response.
+    """
+    request.identity.roll_session_secret()
+    request.session.flash(request.localizer.translate(_("flash.sessions_logged_out")))
+    return HTTPFound(request.route_url("login"))
```

### Comparing `fietsboek-0.8.0/pyproject.toml` & `fietsboek-0.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fietsboek"
 description = "GPX file sharing website"
-version = "0.8.0"
+version = "0.9.0"
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 authors = [
     "Daniel Schadt <fietsboek@kingdread.de>",
 ]
 classifiers = [
     'Development Status :: 3 - Alpha',
@@ -28,31 +28,31 @@
 python = "^3.9"
 
 pyramid = "^2"
 pyramid_jinja2 = "^2.10"
 pyramid_debugtoolbar = "^4.9"
 pyramid_retry = "^2.1"
 pyramid_tm = "^2.5"
-waitress = "^2.1"
+waitress = "^3"
 
 SQLAlchemy = { version = "^2.0.15", extras = ["mypy"] }
 alembic = "^1.8"
-transaction = "^3"
+transaction = "^4"
 "zope.sqlalchemy" = "^3.0"
-redis = "^4.3.4"
+redis = "^5"
 
 Babel = "^2.11"
-cryptography = "^41.0.1"
+cryptography = "^42"
 gpxpy = "^1.5"
 markdown = "^3.4"
 nh3 = "^0.2.9"
 Click = "^8.1"
 requests = "^2.28.1"
 
-pydantic = "^1.10.2"
+pydantic = "^2"
 termcolor = "^2.1.1"
 filelock = "^3.8.2"
 brotli = "^1.0.9"
 click-option-group = "^0.5.5"
 fitparse = "^1.2.0"
 
 [tool.poetry.group.docs]
@@ -62,25 +62,25 @@
 Sphinx = "^7.0"
 sphinx-autodoc-typehints = "^1.19.5"
 
 [tool.poetry.group.testing]
 optional = true
 
 [tool.poetry.group.testing.dependencies]
-pytest = "^7.2.0"
+pytest = "^8.0.0"
 webtest = "^3.0.0"
-pytest-cov = "^4.0.0"
-pytest-playwright = "^0.3.0"
+pytest-cov = "^5.0.0"
+pytest-playwright = "^0.4.0"
 
 [tool.poetry.group.linters]
 optional = true
 
 [tool.poetry.group.linters.dependencies]
-pylint = "^2.15.8"
-black = "^23.1.0"
+pylint = "^3"
+black = "^24.0.0"
 
 [tool.poetry.group.types]
 optional = true
 
 [tool.poetry.group.types.dependencies]
 mypy = "^1.1"
 types-markdown = "^3.4.2.1"
```

### Comparing `fietsboek-0.8.0/PKG-INFO` & `fietsboek-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fietsboek
-Version: 0.8.0
+Version: 0.9.0
 Summary: GPX file sharing website
 Home-page: https://fietsboek.org/
 License: AGPL-3.0-or-later
 Keywords: web,gpx
 Author: Daniel Schadt
 Author-email: fietsboek@kingdread.de
 Requires-Python: >=3.9,<4.0
@@ -12,40 +12,41 @@
 Classifier: Framework :: Pyramid
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Requires-Dist: Babel (>=2.11,<3.0)
 Requires-Dist: Click (>=8.1,<9.0)
 Requires-Dist: SQLAlchemy[mypy] (>=2.0.15,<3.0.0)
 Requires-Dist: alembic (>=1.8,<2.0)
 Requires-Dist: brotli (>=1.0.9,<2.0.0)
 Requires-Dist: click-option-group (>=0.5.5,<0.6.0)
-Requires-Dist: cryptography (>=41.0.1,<42.0.0)
+Requires-Dist: cryptography (>=42,<43)
 Requires-Dist: filelock (>=3.8.2,<4.0.0)
 Requires-Dist: fitparse (>=1.2.0,<2.0.0)
 Requires-Dist: gpxpy (>=1.5,<2.0)
 Requires-Dist: markdown (>=3.4,<4.0)
 Requires-Dist: nh3 (>=0.2.9,<0.3.0)
-Requires-Dist: pydantic (>=1.10.2,<2.0.0)
+Requires-Dist: pydantic (>=2,<3)
 Requires-Dist: pyramid (>=2,<3)
 Requires-Dist: pyramid_debugtoolbar (>=4.9,<5.0)
 Requires-Dist: pyramid_jinja2 (>=2.10,<3.0)
 Requires-Dist: pyramid_retry (>=2.1,<3.0)
 Requires-Dist: pyramid_tm (>=2.5,<3.0)
-Requires-Dist: redis (>=4.3.4,<5.0.0)
+Requires-Dist: redis (>=5,<6)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: termcolor (>=2.1.1,<3.0.0)
-Requires-Dist: transaction (>=3,<4)
-Requires-Dist: waitress (>=2.1,<3.0)
+Requires-Dist: transaction (>=4,<5)
+Requires-Dist: waitress (>=3,<4)
 Requires-Dist: zope.sqlalchemy (>=3.0,<4.0)
 Project-URL: Documentation, https://docs.fietsboek.org/
 Project-URL: Repository, https://gitlab.com/dunj3/fietsboek
 Description-Content-Type: text/markdown
 
 Fietsboek
 =========
```

#### html2text {}

```diff
@@ -1,53 +1,53 @@
-Metadata-Version: 2.1 Name: fietsboek Version: 0.8.0 Summary: GPX file sharing
+Metadata-Version: 2.1 Name: fietsboek Version: 0.9.0 Summary: GPX file sharing
 website Home-page: https://fietsboek.org/ License: AGPL-3.0-or-later Keywords:
 web,gpx Author: Daniel Schadt Author-email: fietsboek@kingdread.de Requires-
 Python: >=3.9,<4.0 Classifier: Development Status :: 3 - Alpha Classifier:
 Framework :: Pyramid Classifier: License :: OSI Approved :: GNU Affero General
 Public License v3 or later (AGPLv3+) Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
-Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic
-Content Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
-Requires-Dist: Babel (>=2.11,<3.0) Requires-Dist: Click (>=8.1,<9.0) Requires-
-Dist: SQLAlchemy[mypy] (>=2.0.15,<3.0.0) Requires-Dist: alembic (>=1.8,<2.0)
-Requires-Dist: brotli (>=1.0.9,<2.0.0) Requires-Dist: click-option-group
-(>=0.5.5,<0.6.0) Requires-Dist: cryptography (>=41.0.1,<42.0.0) Requires-Dist:
-filelock (>=3.8.2,<4.0.0) Requires-Dist: fitparse (>=1.2.0,<2.0.0) Requires-
-Dist: gpxpy (>=1.5,<2.0) Requires-Dist: markdown (>=3.4,<4.0) Requires-Dist:
-nh3 (>=0.2.9,<0.3.0) Requires-Dist: pydantic (>=1.10.2,<2.0.0) Requires-Dist:
-pyramid (>=2,<3) Requires-Dist: pyramid_debugtoolbar (>=4.9,<5.0) Requires-
-Dist: pyramid_jinja2 (>=2.10,<3.0) Requires-Dist: pyramid_retry (>=2.1,<3.0)
-Requires-Dist: pyramid_tm (>=2.5,<3.0) Requires-Dist: redis (>=4.3.4,<5.0.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0) Requires-Dist: termcolor
-(>=2.1.1,<3.0.0) Requires-Dist: transaction (>=3,<4) Requires-Dist: waitress
-(>=2.1,<3.0) Requires-Dist: zope.sqlalchemy (>=3.0,<4.0) Project-URL:
-Documentation, https://docs.fietsboek.org/ Project-URL: Repository, https://
-gitlab.com/dunj3/fietsboek Description-Content-Type: text/markdown Fietsboek
-========= _[_P_i_p_e_l_i_n_e_ _s_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _s_t_a_t_u_s_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n
-_v_e_r_s_i_o_n_s_][Website](https://fietsboek.org) â [Documentation](https://
-docs.fietsboek.org) Fietsboek is a self-hostable sharing site for GPX track
-recordings with social features. The goal is to have an application like
-[MyTourbook][MyTourbook] that runs as a web-service and allows sharing and
-discovering of new tracks. Note that Fietsboek is early in development and a
-hobby project, as such many features are still lacking. [MyTourbook]: https://
-mytourbook.sourceforge.io/mytourbook/ Installation ------------ Setup
-instructions are in the [documentation](https://docs.fietsboek.org/
-administration/installation.html) ([mirror](https://fietsboek.readthedocs.io/
-en/latest/administration/installation.html)). Development ----------- - Setup
-the environment: virtualenv .venv .venv/bin/pip install poetry .venv/bin/poetry
-install - Adjust `development.ini` to your needs. Explanations of the
-configuration options are in the [documentation](https://docs.fietsboek.org/
-administration/configuration.html). - Initialize the database: .venv/bin/
-alembic -c development.ini upgrade head - Serve the code: .venv/bin/pserve
-development.ini --reload - Hack away! License ------- Fietsboek, the GPX web
-sharing project Copyright (C) 2022 Daniel Schadt This program is free software:
-you can redistribute it and/or modify it under the terms of the GNU Affero
-General Public License as published by the Free Software Foundation, either
-version 3 of the License, or (at your option) any later version. This program
-is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
-without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
-PARTICULAR PURPOSE. See the GNU Affero General Public License for more details.
-You should have received a copy of the GNU Affero General Public License along
-with this program. If not, see
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content Classifier: Topic
+:: Internet :: WWW/HTTP :: WSGI :: Application Requires-Dist: Babel
+(>=2.11,<3.0) Requires-Dist: Click (>=8.1,<9.0) Requires-Dist: SQLAlchemy[mypy]
+(>=2.0.15,<3.0.0) Requires-Dist: alembic (>=1.8,<2.0) Requires-Dist: brotli
+(>=1.0.9,<2.0.0) Requires-Dist: click-option-group (>=0.5.5,<0.6.0) Requires-
+Dist: cryptography (>=42,<43) Requires-Dist: filelock (>=3.8.2,<4.0.0)
+Requires-Dist: fitparse (>=1.2.0,<2.0.0) Requires-Dist: gpxpy (>=1.5,<2.0)
+Requires-Dist: markdown (>=3.4,<4.0) Requires-Dist: nh3 (>=0.2.9,<0.3.0)
+Requires-Dist: pydantic (>=2,<3) Requires-Dist: pyramid (>=2,<3) Requires-Dist:
+pyramid_debugtoolbar (>=4.9,<5.0) Requires-Dist: pyramid_jinja2 (>=2.10,<3.0)
+Requires-Dist: pyramid_retry (>=2.1,<3.0) Requires-Dist: pyramid_tm
+(>=2.5,<3.0) Requires-Dist: redis (>=5,<6) Requires-Dist: requests
+(>=2.28.1,<3.0.0) Requires-Dist: termcolor (>=2.1.1,<3.0.0) Requires-Dist:
+transaction (>=4,<5) Requires-Dist: waitress (>=3,<4) Requires-Dist:
+zope.sqlalchemy (>=3.0,<4.0) Project-URL: Documentation, https://
+docs.fietsboek.org/ Project-URL: Repository, https://gitlab.com/dunj3/fietsboek
+Description-Content-Type: text/markdown Fietsboek ========= _[_P_i_p_e_l_i_n_e_ _s_t_a_t_u_s_]
+_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _s_t_a_t_u_s_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_][Website](https:/
+/fietsboek.org) â [Documentation](https://docs.fietsboek.org) Fietsboek is a
+self-hostable sharing site for GPX track recordings with social features. The
+goal is to have an application like [MyTourbook][MyTourbook] that runs as a
+web-service and allows sharing and discovering of new tracks. Note that
+Fietsboek is early in development and a hobby project, as such many features
+are still lacking. [MyTourbook]: https://mytourbook.sourceforge.io/mytourbook/
+Installation ------------ Setup instructions are in the [documentation](https:/
+/docs.fietsboek.org/administration/installation.html) ([mirror](https://
+fietsboek.readthedocs.io/en/latest/administration/installation.html)).
+Development ----------- - Setup the environment: virtualenv .venv .venv/bin/pip
+install poetry .venv/bin/poetry install - Adjust `development.ini` to your
+needs. Explanations of the configuration options are in the [documentation]
+(https://docs.fietsboek.org/administration/configuration.html). - Initialize
+the database: .venv/bin/alembic -c development.ini upgrade head - Serve the
+code: .venv/bin/pserve development.ini --reload - Hack away! License ------
+- Fietsboek, the GPX web sharing project Copyright (C) 2022 Daniel Schadt This
+program is free software: you can redistribute it and/or modify it under the
+terms of the GNU Affero General Public License as published by the Free
+Software Foundation, either version 3 of the License, or (at your option) any
+later version. This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
+or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General Public License
+for more details. You should have received a copy of the GNU Affero General
+Public License along with this program. If not, see
 www.gnu.org/licenses/>.
```

