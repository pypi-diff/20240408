# Comparing `tmp/webinarru-0.0.52.tar.gz` & `tmp/webinarru-0.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webinarru-0.0.52.tar", max compression
+gzip compressed data, was "webinarru-0.0.53.tar", max compression
```

## Comparing `webinarru-0.0.52.tar` & `webinarru-0.0.53.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      935 2023-09-23 05:40:20.990000 webinarru-0.0.52/README.md
--rw-r--r--   0        0        0       58 2023-09-23 09:37:15.780000 webinarru-0.0.52/WebinarRu/__init__.py
--rw-r--r--   0        0        0     5656 2024-03-22 08:25:55.281533 webinarru-0.0.52/WebinarRu/base_api.py
--rw-r--r--   0        0        0    31539 2024-03-25 18:43:37.167585 webinarru-0.0.52/WebinarRu/models.py
--rw-r--r--   0        0        0    60778 2024-03-25 18:43:08.454618 webinarru-0.0.52/WebinarRu/webinar_api.py
--rw-r--r--   0        0        0      515 2024-03-25 18:46:57.323643 webinarru-0.0.52/pyproject.toml
--rw-r--r--   0        0        0     1454 1970-01-01 00:00:00.000000 webinarru-0.0.52/PKG-INFO
+-rw-r--r--   0        0        0      935 2023-09-23 05:40:20.990000 webinarru-0.0.53/README.md
+-rw-r--r--   0        0        0       58 2023-09-23 09:37:15.780000 webinarru-0.0.53/WebinarRu/__init__.py
+-rw-r--r--   0        0        0     5656 2024-03-22 08:25:55.281533 webinarru-0.0.53/WebinarRu/base_api.py
+-rw-r--r--   0        0        0    31539 2024-03-25 18:43:37.167585 webinarru-0.0.53/WebinarRu/models.py
+-rw-r--r--   0        0        0    60799 2024-04-08 16:00:36.071910 webinarru-0.0.53/WebinarRu/webinar_api.py
+-rw-r--r--   0        0        0      515 2024-04-08 16:00:36.020706 webinarru-0.0.53/pyproject.toml
+-rw-r--r--   0        0        0     1454 1970-01-01 00:00:00.000000 webinarru-0.0.53/PKG-INFO
```

### Comparing `webinarru-0.0.52/README.md` & `webinarru-0.0.53/README.md`

 * *Files identical despite different names*

### Comparing `webinarru-0.0.52/WebinarRu/base_api.py` & `webinarru-0.0.53/WebinarRu/base_api.py`

 * *Files identical despite different names*

### Comparing `webinarru-0.0.52/WebinarRu/models.py` & `webinarru-0.0.53/WebinarRu/models.py`

 * *Files identical despite different names*

### Comparing `webinarru-0.0.52/WebinarRu/webinar_api.py` & `webinarru-0.0.53/WebinarRu/webinar_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,17 +119,17 @@
         """
         data = {}
         data.update({"email": email})
         data.update({"name": name})
         data.update({"secondName": second_name})
         data.update({"nickname": nickname}) if nickname else ...
         data.update({"role": role}) if role else ...
-        data.update({"isAutoEnter": is_auto_enter}) if is_auto_enter else ...
-        data.update({"isAccepted": is_accepted}) if is_accepted else ...
-        data.update({"sendEmail": send_email}) if send_email else ...
+        data.update({"isAutoEnter": str(is_auto_enter).lower()}) if is_auto_enter else ...
+        data.update({"isAccepted": str(is_accepted).lower()}) if is_accepted else ...
+        data.update({"sendEmail": str(send_email).lower()}) if send_email else ...
         data.update({"avatar": avatar}) if avatar else ...
         data.update({"pattrName": pattr_name}) if pattr_name else ...
         data.update({"phone": phone}) if phone else ...
         data.update({"description": description}) if description else ...
         data.update({"organization": organization}) if organization else ...
         data.update({"position": position}) if position else ...
         data.update({"sex": sex}) if sex else ...
@@ -151,16 +151,16 @@
         :param send_email: рассылка писем с платформы mts-link.ru;
         :param event_id: Идентификатор серии;
         :return: Данные зарегистрированного участника.
         """
         data = {}
         users = self._make_data_massive_list([user.dict() for user in users], "users")
         data.update(users)
-        data.update({"isAutoEnter": is_auto_enter}) if is_auto_enter else ...
-        data.update({"sendEmail": send_email}) if send_email else ...
+        data.update({"isAutoEnter": str(is_auto_enter).lower()}) if is_auto_enter else ...
+        data.update({"sendEmail": str(send_email).lower()}) if send_email else ...
         registered_participants = await self.post_json(f"/events/{event_id}/invite", data)
         if registered_participants is not None:
             return [
                 RegisteredParticipant(**registered_participant) for registered_participant in registered_participants
             ]
 
     async def get_events_for_user(
@@ -350,15 +350,15 @@
         Удаляется вебинар, статистика, чат/вопросы. Удаление нельзя отменить.
         @param send_email: Рассылка писем с платформы Webinar.ru.
         Флаг определяет отправку письма "К сожалению, мероприятие отменено"
         @param event_session_id: идентификатор вебинара (eventsessionID)
         @return: True если удаление успешно
         """
         params = {}
-        params.update({"sendEmail": "true" if send_email else "false"}) if send_email is not None else ...
+        params.update({"sendEmail": str(send_email).lower()}) if send_email is not None else ...
         delete_event = await self.delete(f"/eventsessions/{event_session_id}", params)
         if delete_event is not None:
             return True if delete_event == 204 else False
 
     async def create_event(
             self,
             name: str,
@@ -419,29 +419,29 @@
             "AccessSettings": access_settings.to_dict,
             "access": access,
         }
         data.update({"password": password}) if password is not None else ...
         data.update({"description": description}) if description is not None else ...
         data.update({"rule": rule}) if rule is not None else ...
         data.update(
-            {"isEventRegAllowed": "true" if is_event_reg_allowed else "false"}
+            {"isEventRegAllowed": str(is_event_reg_allowed).lower()}
         ) if is_event_reg_allowed is not None else ...
         data.update(self._datetime_to_dict("startsAt", starts_at)) if starts_at is not None else ...
         data.update(self._datetime_to_dict("endsAt", ends_at)) if ends_at is not None else ...
         data.update({"timezone": timezone}) if timezone is not None else ...
         data.update({"image": image}) if image is not None else ...
         data.update({"type": event_type}) if event_type is not None else ...
         data.update({"lang": lang}) if lang is not None else ...
         data.update({"urlAlias": url_alias}) if url_alias is not None else ...
         data.update(self._make_massive(lector_ids, "lectorIds")) if lector_ids is not None else ...
         data.update(self._make_massive(tags, "tags")) if tags is not None else ...
         data.update({"duration": duration}) if duration is not None else ...
         data.update({"ownerId": owner_id}) if owner_id is not None else ...
         data.update(
-            {"defaultRemindersEnabled": "true" if default_reminders_enabled else "false"}
+            {"defaultRemindersEnabled": str(default_reminders_enabled).lower()}
         ) if default_reminders_enabled is not None else ...
         data.update({"brandingId": branding_id}) if branding_id is not None else ...
 
         new_event = await self.post_json("/events", data)
         if new_event is not None:
             return CreatedEvent(**new_event)
 
@@ -596,15 +596,15 @@
         data.update({"startType": start_type}) if start_type is not None else ...
         data.update({"description": description}) if description is not None else ...
         data.update({"lang": lang}) if lang is not None else ...
         data.update(self._datetime_to_dict("startsAt", starts_at)) if starts_at is not None else ...
         data.update({"timezone": timezone}) if timezone is not None else ...
         data.update({"image": image}) if image is not None else ...
         data.update({"duration": duration}) if duration is not None else ...
-        data.update({"sendEmail": "true" if send_email else "false"}) if send_email is not None else ...
+        data.update({"sendEmail": str(send_email).lower()}) if send_email is not None else ...
         data.update({"updateContext": update_context}) if update_context is not None else ...
 
         edited_event_session = await self.put(f"/eventsessions/{event_session_id}", data)
         if edited_event_session is not None:
             return True if edited_event_session.status == 204 else False
 
     async def create_webinar(
@@ -708,18 +708,18 @@
         :param is_moderated: статус модерации сообщений
         :param limit: количество отображаемых сообщений. Значение по умолчанию: последние 100.
         :param author_id: идентификатор пользователя, отправившего сообщение
         :param private_chat: получить приватный чат. Параметр используется только с указанием authorId
         :return: массив сообщений
         """
         params = {}
-        params.update({"isModerated": "true" if is_moderated else "false"}) if is_moderated is not None else ...
+        params.update({"isModerated": str(is_moderated).lower()}) if is_moderated is not None else ...
         params.update({"limit": limit}) if limit is not None else ...
         params.update({"author_id": author_id}) if author_id is not None else ...
-        params.update({"privateChat": "true" if private_chat else "false"}) if private_chat is not None else ...
+        params.update({"privateChat": str(private_chat).lower()}) if private_chat is not None else ...
 
         messages = await self.get_json(f"/eventsessions/{event_session_id}/chat", params)
         # print(messages)
         if messages is not None:
             return [ChatMessage(**message) for message in messages]
 
     async def get_files(
@@ -736,15 +736,15 @@
         :param file_format: расширение файла
         :param is_shared: поиск по общей папке
         """
         params = {}
         params.update({"user": user}) if user is not None else ...
         params.update({"parent": parent}) if parent is not None else ...
         params.update({"format": file_format}) if file_format is not None else ...
-        params.update({"isShared": "true" if is_shared else "false"}) if is_shared is not None else ...
+        params.update({"isShared": str(is_shared).lower()}) if is_shared is not None else ...
 
         files = await self.get_json("/fileSystem/files", params)
         # pprint(files)
         if files is not None:
             return [File(**file) for file in files]
 
     async def get_file(
@@ -847,15 +847,15 @@
         Запросом меняются параметры записи: доступность записи по ссылке
         :param record_id: id онлайн-записи
         :param is_viewable: доступность записи;
         :param password: пароль на запись;
         :param view_access: настройка доступа для показа записи.
         """
         params = {}
-        params.update({"isViewable": is_viewable}) if is_viewable is not None else ...
+        params.update({"isViewable": str(is_viewable).lower()}) if is_viewable is not None else ...
         params.update({"password": password}) if password is not None else ...
         params.update({"viewAccess": view_access}) if view_access is not None else ...
 
         await self.put(f"/records/{record_id}", params)
 
     async def share_online_record_by_event_session_id(
             self,
@@ -869,15 +869,15 @@
         настройки доступа и наличие пароля на просмотр
         :param event_session_id: Идентификатор вебинара;
         :param is_viewable: доступность записи;
         :param password: пароль на запись;
         :param view_access: настройка доступа для показа записи.
         """
         params = {}
-        params.update({"isViewable": is_viewable}) if is_viewable is not None else ...
+        params.update({"isViewable": str(is_viewable).lower()}) if is_viewable is not None else ...
         params.update({"password": password}) if password is not None else ...
         params.update({"viewAccess": view_access}) if view_access is not None else ...
 
         await self.put(f"/eventsessions/{event_session_id}/records", params)
 
     async def share_online_record_by_email(
             self,
```

### Comparing `webinarru-0.0.52/pyproject.toml` & `webinarru-0.0.53/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "WebinarRu"
-version = "0.0.52"
+version = "0.0.53"
 description = "Python client for webinar.ru platform"
 authors = ["gulyaeve <gulyaev.e@icloud.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "WebinarRu"}]
 
 [tool.poetry.dependencies]
```

### Comparing `webinarru-0.0.52/PKG-INFO` & `webinarru-0.0.53/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebinarRu
-Version: 0.0.52
+Version: 0.0.53
 Summary: Python client for webinar.ru platform
 License: MIT
 Author: gulyaeve
 Author-email: gulyaev.e@icloud.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

