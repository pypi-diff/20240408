# Comparing `tmp/emo_market_base-0.0.1.tar.gz` & `tmp/emo_market_base-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emo_market_base-0.0.1.tar", last modified: Mon Apr  8 20:58:56 2024, max compression
+gzip compressed data, was "emo_market_base-0.0.3.tar", last modified: Mon Apr  8 21:20:38 2024, max compression
```

## Comparing `emo_market_base-0.0.1.tar` & `emo_market_base-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 20:58:56.817008 emo_market_base-0.0.1/
--rw-rw-rw-   0        0        0     1096 2024-03-23 18:43:28.000000 emo_market_base-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      606 2024-04-08 20:58:56.815006 emo_market_base-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       82 2024-03-23 21:50:04.000000 emo_market_base-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-08 20:58:56.817008 emo_market_base-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      768 2024-04-08 20:58:17.000000 emo_market_base-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 20:58:56.780783 emo_market_base-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-08 20:58:56.814003 emo_market_base-0.0.1/src/emo_market_base.egg-info/
--rw-rw-rw-   0        0        0      606 2024-04-08 20:58:56.000000 emo_market_base-0.0.1/src/emo_market_base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2024-04-08 20:58:56.000000 emo_market_base-0.0.1/src/emo_market_base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 20:58:56.000000 emo_market_base-0.0.1/src/emo_market_base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-04-08 20:58:56.000000 emo_market_base-0.0.1/src/emo_market_base.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-08 20:58:56.000000 emo_market_base-0.0.1/src/emo_market_base.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-08 20:58:56.812003 emo_market_base-0.0.1/src/market_base/
--rw-rw-rw-   0        0        0        0 2024-03-23 21:53:27.000000 emo_market_base-0.0.1/src/market_base/__init__.py
--rw-rw-rw-   0        0        0     4746 2024-03-31 03:51:46.000000 emo_market_base-0.0.1/src/market_base/date.py
--rw-rw-rw-   0        0        0      767 2024-03-24 20:02:42.000000 emo_market_base-0.0.1/src/market_base/db.py
--rw-rw-rw-   0        0        0     2630 2024-04-05 12:37:20.000000 emo_market_base-0.0.1/src/market_base/filesytem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:20:38.694719 emo_market_base-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-08 21:20:38.694719 emo_market_base-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 21:20:38.694719 emo_market_base-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:20:38.686720 emo_market_base-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:20:38.690719 emo_market_base-0.0.3/src/emo_market_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-08 21:20:38.000000 emo_market_base-0.0.3/src/emo_market_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-08 21:20:38.000000 emo_market_base-0.0.3/src/emo_market_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 21:20:38.000000 emo_market_base-0.0.3/src/emo_market_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-08 21:20:38.000000 emo_market_base-0.0.3/src/emo_market_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 21:20:38.000000 emo_market_base-0.0.3/src/emo_market_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:20:38.690719 emo_market_base-0.0.3/src/market_base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/src/market_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/src/market_base/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/src/market_base/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/src/market_base/filesytem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:20:38.690719 emo_market_base-0.0.3/src/market_base/webdriver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/src/market_base/webdriver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/src/market_base/webdriver/category_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/src/market_base/webdriver/list_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/src/market_base/webdriver/market.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/src/market_base/webdriver/product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/src/market_base/webdriver/product_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/src/market_base/webdriver/url.py
```

### Comparing `emo_market_base-0.0.1/LICENSE` & `emo_market_base-0.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Eren Mustafa ÖZDAL
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2024 Eren Mustafa ÖZDAL
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `emo_market_base-0.0.1/src/market_base/date.py` & `emo_market_base-0.0.3/src/market_base/date.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-import logging
-from datetime import datetime
-from typing import Dict, List, Union
-from selenium.webdriver.remote.webelement import WebElement
-
-
-logger = logging.getLogger("MarketBaseDate")
-
-
-class Date:
-
-    @staticmethod
-    def to_str(
-        date: Union[datetime, None] = None,
-        date_format: str = "%Y-%m-%d"
-    ) -> str:
-        if date is None:
-            date = datetime.today()
-
-        return date.strftime(date_format)
-
-    @staticmethod
-    def timestamp(date: Union[datetime, None] = None) -> int:
-        if date:
-            return date.timestamp()
-
-        return datetime.now().timestamp()
-
-    @classmethod
-    def parse(cls, txt: str, _format: str = "%d %B %A") -> datetime:
-        """Gelen tarih string verisini datetime nesnesine döndürür.
-        Yılı hesaplar.
-
-        Args:
-            txt (str): tarih metin değeri
-            _format (str): metinden çıkarılacak tarih formatı
-
-        Returns:
-            datetime: oluşturulan tarih nesnesi
-        """
-        if "-" in txt:
-            return cls._parse_range(txt)
-
-        return cls._parse_single(txt, _format)
-
-    @classmethod
-    def _parse_range(cls, txt: str, _format: str = "%d %B"):
-        finish = txt.split('-')[1].strip()
-        return cls._parse_single(finish, _format)
-
-    @classmethod
-    def _parse_single(cls, txt: str, _format: str) -> datetime:
-        # Ay adı alınır
-        month_name = cls.get_month_name(txt, _format)
-
-        # Bulunduğumuz yıl alınır
-        year = datetime.today().year
-
-        # Bulunduğumuz ay Aralık ise ve
-        # gelen tarih Ocak ayı ise yılı 1 arttır
-        if datetime.today().month == 12 and month_name == "Ocak":
-            year += 1
-
-        # Belirlenen yıla göre tarih nesnesi oluştur
-        _format += " %Y"
-        return datetime.strptime(f"{txt} {year}", _format)
-
-    @staticmethod
-    def get_month_name(txt: str, _format: str):
-        """Gelen tarih metni ve formatına göre ayın adını alır.
-        Bunun için formattaki %B ile ay adının konumunu bulur 
-        ve metinden döndürür.
-
-        Args:
-            txt (str): Tarih metni
-            _format (str): Tarih formatı
-
-        Returns:
-            str: ay adı
-        """
-        format_parts = _format.split()
-        i = format_parts.index("%B")
-        return txt.split()[i]
-
-    @classmethod
-    def get_dates(
-        cls,
-        els: List[WebElement],
-        excludes: Union[List, None]
-    ) -> List:
-        dates = []
-
-        for el in els:
-            # eğer tarih alınamadı ise geç
-            try:
-                date = cls.get_date(el, excludes)
-                if date:
-                    dates.append(date)
-            except:
-                continue
-
-        logger.info(f"{len(dates)} adet tarih bilgisi alındı")
-
-        return dates
-
-    @classmethod
-    def get_date(
-        cls,
-        el: WebElement,
-        excludes: Union[List, None]
-    ) -> Union[Dict, None]:
-        if excludes and el.text in excludes:
-            return
-
-        return cls.date_dict(el)
-
-    @classmethod
-    def date_dict(cls, el: WebElement) -> Dict:
-        return {
-            "element": el,
-            "text": el.text,
-            "object": cls.parse(el.text)
-        }
-
-    @staticmethod
-    def next_date(dates: List[Dict]) -> Dict:
-        # Bugünün tarih ve saat bilgisini al
-        today = datetime.today()
-
-        # Saat ve dakikayı sıfırla
-        today = today.replace(hour=0, minute=0, second=0, microsecond=0)
-
-        return next((d for d in dates if d["object"] >= today), None)
-
-    @staticmethod
-    def day_difference(
-        start_date: Union[str, datetime],
-        finish_date: Union[str, datetime, None] = None
-    ) -> int:
-        """İki tarih arasındaki gün farkını bulur
-
-        Args:
-            start_date (str): son kazıma tarihi. Format: "%Y-%m-%d"
-            threshold_days (int, optional): Geçmesi gereken süre. Defaults to 7.
-
-        Returns:
-            bool: "Kazıma zamanı geldi mi" sonucu
-        """
-
-        # String tarihini datetime nesnesine dönüştür
-        if isinstance(start_date, str):
-            start_date = datetime.strptime(start_date, "%Y-%m-%d")
-
-        if finish_date is None:
-            finish_date = datetime.today()
-        elif isinstance(finish_date, str):
-            finish_date = datetime.strptime(finish_date, "%Y-%m-%d")
-
-        # Tarih farkını hesapla
-        difference = finish_date - start_date
-
-        # Farkı gün cinsine dönüştür ve threshold_days ile karşılaştır
-        return difference.days
+import logging
+from datetime import datetime
+from typing import Dict, List, Union
+from selenium.webdriver.remote.webelement import WebElement
+
+
+logger = logging.getLogger("MarketBaseDate")
+
+
+class Date:
+
+    @staticmethod
+    def to_str(
+        date: Union[datetime, None] = None,
+        date_format: str = "%Y-%m-%d"
+    ) -> str:
+        if date is None:
+            date = datetime.today()
+
+        return date.strftime(date_format)
+
+    @staticmethod
+    def timestamp(date: Union[datetime, None] = None) -> int:
+        if date:
+            return date.timestamp()
+
+        return datetime.now().timestamp()
+
+    @classmethod
+    def parse(cls, txt: str, _format: str = "%d %B %A") -> datetime:
+        """Gelen tarih string verisini datetime nesnesine döndürür.
+        Yılı hesaplar.
+
+        Args:
+            txt (str): tarih metin değeri
+            _format (str): metinden çıkarılacak tarih formatı
+
+        Returns:
+            datetime: oluşturulan tarih nesnesi
+        """
+        if "-" in txt:
+            return cls._parse_range(txt)
+
+        return cls._parse_single(txt, _format)
+
+    @classmethod
+    def _parse_range(cls, txt: str, _format: str = "%d %B"):
+        finish = txt.split('-')[1].strip()
+        return cls._parse_single(finish, _format)
+
+    @classmethod
+    def _parse_single(cls, txt: str, _format: str) -> datetime:
+        # Ay adı alınır
+        month_name = cls.get_month_name(txt, _format)
+
+        # Bulunduğumuz yıl alınır
+        year = datetime.today().year
+
+        # Bulunduğumuz ay Aralık ise ve
+        # gelen tarih Ocak ayı ise yılı 1 arttır
+        if datetime.today().month == 12 and month_name == "Ocak":
+            year += 1
+
+        # Belirlenen yıla göre tarih nesnesi oluştur
+        _format += " %Y"
+        return datetime.strptime(f"{txt} {year}", _format)
+
+    @staticmethod
+    def get_month_name(txt: str, _format: str):
+        """Gelen tarih metni ve formatına göre ayın adını alır.
+        Bunun için formattaki %B ile ay adının konumunu bulur 
+        ve metinden döndürür.
+
+        Args:
+            txt (str): Tarih metni
+            _format (str): Tarih formatı
+
+        Returns:
+            str: ay adı
+        """
+        format_parts = _format.split()
+        i = format_parts.index("%B")
+        return txt.split()[i]
+
+    @classmethod
+    def get_dates(
+        cls,
+        els: List[WebElement],
+        excludes: Union[List, None]
+    ) -> List:
+        dates = []
+
+        for el in els:
+            # eğer tarih alınamadı ise geç
+            try:
+                date = cls.get_date(el, excludes)
+                if date:
+                    dates.append(date)
+            except:
+                continue
+
+        logger.info(f"{len(dates)} adet tarih bilgisi alındı")
+
+        return dates
+
+    @classmethod
+    def get_date(
+        cls,
+        el: WebElement,
+        excludes: Union[List, None]
+    ) -> Union[Dict, None]:
+        if excludes and el.text in excludes:
+            return
+
+        return cls.date_dict(el)
+
+    @classmethod
+    def date_dict(cls, el: WebElement) -> Dict:
+        return {
+            "element": el,
+            "text": el.text,
+            "object": cls.parse(el.text)
+        }
+
+    @staticmethod
+    def next_date(dates: List[Dict]) -> Dict:
+        # Bugünün tarih ve saat bilgisini al
+        today = datetime.today()
+
+        # Saat ve dakikayı sıfırla
+        today = today.replace(hour=0, minute=0, second=0, microsecond=0)
+
+        return next((d for d in dates if d["object"] >= today), None)
+
+    @staticmethod
+    def day_difference(
+        start_date: Union[str, datetime],
+        finish_date: Union[str, datetime, None] = None
+    ) -> int:
+        """İki tarih arasındaki gün farkını bulur
+
+        Args:
+            start_date (str): son kazıma tarihi. Format: "%Y-%m-%d"
+            threshold_days (int, optional): Geçmesi gereken süre. Defaults to 7.
+
+        Returns:
+            bool: "Kazıma zamanı geldi mi" sonucu
+        """
+
+        # String tarihini datetime nesnesine dönüştür
+        if isinstance(start_date, str):
+            start_date = datetime.strptime(start_date, "%Y-%m-%d")
+
+        if finish_date is None:
+            finish_date = datetime.today()
+        elif isinstance(finish_date, str):
+            finish_date = datetime.strptime(finish_date, "%Y-%m-%d")
+
+        # Tarih farkını hesapla
+        difference = finish_date - start_date
+
+        # Farkı gün cinsine dönüştür ve threshold_days ile karşılaştır
+        return difference.days
```

### Comparing `emo_market_base-0.0.1/src/market_base/db.py` & `emo_market_base-0.0.3/src/market_base/db.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import logging
-from typing import Any, Union
-from cache_db.cache_db import CacheDB
-
-
-class DB:
-
-    def __init__(self, path: str) -> None:
-        self.db = CacheDB(path)
-        self.db.load_cache()
-
-        self.logger = logging.getLogger("MarketBaseDB")
-
-    def get(self, key: str, default: Union[Any, None] = None) -> Any:
-        result = self.db.get(key, default)
-        self.logger.info(f"Veri alındı. '{key}': '{result}'")
-        return result
-
-    def set(self, key: str, value, with_save: bool = True):
-        self.db.cache[key] = value
-        self.logger.info(f"Veri eklendi. '{key}': '{value}'")
-
-        if with_save:
-            self.db.save_cache()
-            self.logger.info(f"Dosya kaydedildi: {self.db.file_path}")
+import logging
+from typing import Any, Union
+from cache_db.cache_db import CacheDB
+
+
+class DB:
+
+    def __init__(self, path: str) -> None:
+        self.db = CacheDB(path)
+        self.db.load_cache()
+
+        self.logger = logging.getLogger("MarketBaseDB")
+
+    def get(self, key: str, default: Union[Any, None] = None) -> Any:
+        result = self.db.get(key, default)
+        self.logger.info(f"Veri alındı. '{key}': '{result}'")
+        return result
+
+    def set(self, key: str, value, with_save: bool = True):
+        self.db.cache[key] = value
+        self.logger.info(f"Veri eklendi. '{key}': '{value}'")
+
+        if with_save:
+            self.db.save_cache()
+            self.logger.info(f"Dosya kaydedildi: {self.db.file_path}")
```

### Comparing `emo_market_base-0.0.1/src/market_base/filesytem.py` & `emo_market_base-0.0.3/src/market_base/filesytem.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-import logging
-import requests
-from typing import List, Union
-from pdf2image import convert_from_path
-from file_system.file import File as FileCore
-
-
-logger = logging.getLogger("MarketBaseFile")
-
-
-class File:
-
-    @staticmethod
-    def mk_dir(base_path: str, **kwargs) -> str:
-        path = base_path.format(**kwargs)
-        if not FileCore.exists(path):
-            FileCore.create_directory(path)
-            logger.info(f"'{path}' dizini oluşturuldu.")
-
-        return path
-
-    @staticmethod
-    def clean_filename(filename: str):
-        # İstenmeyen karakterlerin bulunduğu bir karakter kümesi oluşturun
-        invalid_chars = '<>:"/\\|?*'
-
-        # İstenmeyen karakterleri temizleyin
-        chars = [c for c in filename if c not in invalid_chars]
-        cleaned_filename = ''.join(chars)
-        logger.info("Dosya adı temizlendi. "
-                    f"'{filename}' -> '{cleaned_filename}'")
-
-        return cleaned_filename
-
-    @staticmethod
-    def download(src: str, dest: str) -> Union[str, None]:
-        """
-        İnternetten bir kaynağın indirilmesini ve hedefe kaydedilmesini sağlar
-
-        Args:
-            src (str): kaynak adresi
-            dest (str): yerel hedef yolu
-
-        Returns:
-            str: _description_
-        """
-        # dosya adı belirlenir
-        filename = FileCore.get_filename(src)
-
-        try:
-            response = requests.get(src)
-            if response.status_code == 200:
-                file_path = f"{dest}/{filename}"
-                with open(f"{dest}/{filename}", "wb") as file:
-                    file.write(response.content)
-
-                return file_path
-            else:
-                logger.error(f"----- {src} adresinden dosya indirilemedi.")
-                return None
-        except Exception as e:
-            logger.error(f"----- Dosya indirilirken hata oluştu: {e}")
-            return None
-
-    @staticmethod
-    def pdf_to_images(pdf_path: str, dest: str) -> List:
-        image_paths = []
-
-        # PDF dosyasını görüntü dosyalarına dönüştür
-        images = convert_from_path(pdf_path)
-
-        # dosya adını al
-        filename = FileCore.get_filename(pdf_path, without_extentsion=True)
-
-        for i, image in enumerate(images, start=1):
-            # görüntü dosyasının adını oluştur
-            image_path = f"{dest}/{filename}_page_{i}.jpg"
-            image.save(image_path)
-            image_paths.append(image_path)
-            logger.info(f"'{image_path}' görseli oluşturuldu.")
-
-        return image_paths
+import logging
+import requests
+from typing import List, Union
+from pdf2image import convert_from_path
+from file_system.file import File as FileCore
+
+
+logger = logging.getLogger("MarketBaseFile")
+
+
+class File:
+
+    @staticmethod
+    def mk_dir(base_path: str, **kwargs) -> str:
+        path = base_path.format(**kwargs)
+        if not FileCore.exists(path):
+            FileCore.create_directory(path)
+            logger.info(f"'{path}' dizini oluşturuldu.")
+
+        return path
+
+    @staticmethod
+    def clean_filename(filename: str):
+        # İstenmeyen karakterlerin bulunduğu bir karakter kümesi oluşturun
+        invalid_chars = '<>:"/\\|?*'
+
+        # İstenmeyen karakterleri temizleyin
+        chars = [c for c in filename if c not in invalid_chars]
+        cleaned_filename = ''.join(chars)
+        logger.info("Dosya adı temizlendi. "
+                    f"'{filename}' -> '{cleaned_filename}'")
+
+        return cleaned_filename
+
+    @staticmethod
+    def download(src: str, dest: str) -> Union[str, None]:
+        """
+        İnternetten bir kaynağın indirilmesini ve hedefe kaydedilmesini sağlar
+
+        Args:
+            src (str): kaynak adresi
+            dest (str): yerel hedef yolu
+
+        Returns:
+            str: _description_
+        """
+        # dosya adı belirlenir
+        filename = FileCore.get_filename(src)
+
+        try:
+            response = requests.get(src)
+            if response.status_code == 200:
+                file_path = f"{dest}/{filename}"
+                with open(f"{dest}/{filename}", "wb") as file:
+                    file.write(response.content)
+
+                return file_path
+            else:
+                logger.error(f"----- {src} adresinden dosya indirilemedi.")
+                return None
+        except Exception as e:
+            logger.error(f"----- Dosya indirilirken hata oluştu: {e}")
+            return None
+
+    @staticmethod
+    def pdf_to_images(pdf_path: str, dest: str) -> List:
+        image_paths = []
+
+        # PDF dosyasını görüntü dosyalarına dönüştür
+        images = convert_from_path(pdf_path)
+
+        # dosya adını al
+        filename = FileCore.get_filename(pdf_path, without_extentsion=True)
+
+        for i, image in enumerate(images, start=1):
+            # görüntü dosyasının adını oluştur
+            image_path = f"{dest}/{filename}_page_{i}.jpg"
+            image.save(image_path)
+            image_paths.append(image_path)
+            logger.info(f"'{image_path}' görseli oluşturuldu.")
+
+        return image_paths
```

