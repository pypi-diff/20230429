# Comparing `tmp/yeref-0.1.47.tar.gz` & `tmp/yeref-0.1.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.47.tar", last modified: Fri Apr 28 11:35:27 2023, max compression
+gzip compressed data, was "yeref-0.1.48.tar", last modified: Sat Apr 29 13:59:14 2023, max compression
```

## Comparing `yeref-0.1.47.tar` & `yeref-0.1.48.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-28 11:35:27.520586 yeref-0.1.47/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-28 11:35:27.520815 yeref-0.1.47/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-28 11:35:27.522379 yeref-0.1.47/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1154 2023-04-28 11:35:19.000000 yeref-0.1.47/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-28 11:35:27.511388 yeref-0.1.47/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.47/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   249969 2023-04-27 19:38:16.000000 yeref-0.1.47/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   192928 2023-04-27 18:43:33.000000 yeref-0.1.47/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-28 11:35:27.519894 yeref-0.1.47/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-28 11:35:27.000000 yeref-0.1.47/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-04-28 11:35:27.000000 yeref-0.1.47/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-28 11:35:27.000000 yeref-0.1.47/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-28 11:35:27.000000 yeref-0.1.47/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-29 13:59:14.811012 yeref-0.1.48/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-29 13:59:14.811288 yeref-0.1.48/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-29 13:59:14.812275 yeref-0.1.48/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1154 2023-04-29 13:59:02.000000 yeref-0.1.48/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-29 13:59:14.804125 yeref-0.1.48/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.48/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   252103 2023-04-29 13:49:34.000000 yeref-0.1.48/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   192928 2023-04-28 18:02:08.000000 yeref-0.1.48/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-29 13:59:14.810250 yeref-0.1.48/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-29 13:59:14.000000 yeref-0.1.48/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-04-29 13:59:14.000000 yeref-0.1.48/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-29 13:59:14.000000 yeref-0.1.48/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-29 13:59:14.000000 yeref-0.1.48/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.47/setup.py` & `yeref-0.1.48/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.47',
+      version='0.1.48',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -39,10 +39,10 @@
 # python setup.py bdist_wheel
 # endregion
 
 # python -m build
 
 # twine upload dist/*
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.47-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.48-py3-none-any.whl
 
 # python3 -m pip install --upgrade yeref
```

### Comparing `yeref-0.1.47/yeref/l_.py` & `yeref-0.1.48/yeref/l_.py`

 * *Files 1% similar despite different names*

```diff
@@ -1759,14 +1759,38 @@
     'ru': "👩🏽‍💻 <b>Выбери</b> media-заметку для удаления",
     'en': "👩🏽‍💻 <b>Select</b> media note to delete",
     'es': "👩🏽‍💻 <b>Seleccione</b> nota multimedia para eliminar",
     'fr': "👩🏽‍💻 <b>Sélectionnez</b> la note multimédia à supprimer",
     'zh': "👩🏽‍💻<b>选择</b>要删除的媒体备注",
     'ar': "<b>حدد</b> ملاحظة وسائط لحذفها",
 }
+l_media_show = {
+    'ru': "👩🏽‍💻 <b>Введи</b> текст для поиска по media-заметкам",
+    'en': "👩🏽‍💻 <b>Select</b> media note to delete",
+    'es': "👩🏽‍💻 <b>Seleccione</b> nota multimedia para eliminar",
+    'fr': "👩🏽‍💻 <b>Sélectionnez</b> la note multimédia à supprimer",
+    'zh': "👩🏽‍💻<b>选择</b>要删除的媒体备注",
+    'ar': "<b>حدد</b> ملاحظة وسائط لحذفها",
+}
+l_media_random = {
+    'ru': "🎲 Случайный выбор",
+    'en': "👩🏽‍💻 <b>Select</b> media note to delete",
+    'es': "👩🏽‍💻 <b>Seleccione</b> nota multimedia para eliminar",
+    'fr': "👩🏽‍💻 <b>Sélectionnez</b> la note multimédia à supprimer",
+    'zh': "👩🏽‍💻<b>选择</b>要删除的媒体备注",
+    'ar': "<b>حدد</b> ملاحظة وسائط لحذفها",
+}
+l_media_none = {
+    'ru': "👩🏽‍💻 <b>Media</b>-заметок не найдено",
+    'en': "👩🏽‍💻 <b>Select</b> media note to delete",
+    'es': "👩🏽‍💻 <b>Seleccione</b> nota multimedia para eliminar",
+    'fr': "👩🏽‍💻 <b>Sélectionnez</b> la note multimédia à supprimer",
+    'zh': "👩🏽‍💻<b>选择</b>要删除的媒体备注",
+    'ar': "<b>حدد</b> ملاحظة وسائط لحذفها",
+}
 l_media_file = {
     'ru': "👩🏽‍💻 1/2. <b>Прикрепи</b> audio/video, text/photo контент для создания media-заметки",
     'en': "👩🏽‍💻 1/2. <b>Attach</b> audio/video, text/photo content to create a media note",
     'es': "👩🏽‍💻 1/2. <b>Adjunte</b> contenido de audio/video, texto/foto para crear una nota multimedia",
     'fr': "👩🏽‍💻 1/2. <b>Joignez</b> du contenu audio/vidéo, texte/photo pour créer une note multimédia",
     'zh': "👩🏽‍💻 1/2。<b>附加</b>音频/视频、文本/照片内容以创建媒体说明",
     'ar': "👩🏽‍💻 1/2. <b>قم بإرفاق</b> محتوى صوت / فيديو ونص / صورة لإنشاء ملاحظة وسائط",
@@ -2905,15 +2929,15 @@
     'en': "➕ Add channel",
     'es': "➕ Agregar grupo",
     'fr': "➕ Ajouter un channele",
     'zh': "➕ 添加組",
     'ar': "➕ إضافة مجموعة",
 }
 l_commands_handler = {
-    'ru': "⚙️ <b>Настройка</b> канала <b>{0}</b> {1}\n\n<b>⛏ Admin-команды @{2}</b>\n/update <i>обновление параметров</i>\n/transfer   <i>передача admin-прав</i>\n/info   <i>информация</i>\n/stat   <i>статистика</i>\n/parse  <i>выгрузка базы подписчиков</i>\n/videochat 1 1 <i>анонс видео-трансляции</i>\n/clean  <i>долгая очистка канала от deleted/scam/fake-аккаунтов, а также по 🕵🏽 Авто-бан правилам</i>\n/channel NAME   <i>добавить канал для проверки подписки</i>",
+    'ru': "⚙️ <b>Настройка</b> канала <b>{0}</b> {1}\n\n<b>⛏ Admin-команды @{2}</b>\n/update <i>обновление параметров</i>\n/transfer   <i>передача admin-прав</i>\n/info   <i>информация</i>\n/stat   <i>статистика</i>\n/parse  <i>выгрузка базы подписчиков</i>\n/videochat 1 1 <i>анонс видео-трансляции</i>\n/clean  <i>долгая очистка канала от deleted/scam/fake-аккаунтов, а также по 🕵🏽 Авто-бан правилам</i>\n/channel NAME   <i>добавить другой канал для проверки подписки</i>",
     'en': "⚙️ <b>channel</b> settings of <b>{0}</b> {1}\n\n<b>⛏ Admin-commands @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/log   <i>see logs</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-accounts</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from channel for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in channel for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-accounts</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for channel</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
     'es': "⚙️ Configuración de <b>Grupo</b> de <b>{0}</b> {1}\n\n<b>⛏ Comandos de administración @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/log   <i>see logs</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-accounts</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from channel for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in channel for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-accounts</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for channel</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
     'fr': "⚙️ Paramètres de <b>channele</b> de <b>{0}</b> {1}\n\n<b>⛏ Commandes d'administration @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/log   <i>see logs</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-accounts</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from channel for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in channel for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-accounts</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for channel</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
     'zh': "⚙️ <b>組</b>設置 <b>{0}</b> {1}\n\n<b>⛏ 管理員命令 @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/log   <i>see logs</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-accounts</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from channel for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in channel for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-accounts</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for channel</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
     'ar': "⚙️ إعدادات <b> المجموعة </b> الخاصة بـ <b>{0}</b> {1}\n\n<b>⛏ أوامر المسؤول @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/parse  <i>[all|old|premium|active|online]</i>\n/log   <i>see logs</i>\n<code>/parse old</code> - <i>parsing old id-accounts</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from channel for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in channel for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-accounts</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for channel</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
 }
 l_info_restrict = {
@@ -3194,22 +3218,14 @@
     'ru': "👮🏽 Готово! Проверка подписки на {0}-канал настроена\n\nОпцию можно включить в настройках, нажав [✅☑Вкл подписку]",
     'en': "👮🏽 Ready! Subscribe checking to {0}-channel is configured\n\nEnable this option in the Settings by pushing [✅☑Enable subscription]",
     'es': "👮🏽 Listo! La verificación de suscripción a {0}-canal está configurada\n\nActive esta opción en Configuración presionando [✅☑Habilitar suscripción]",
     'fr': "👮🏽 Prêt! La vérification de l'abonnement à la chaîne {0} est configurée\n\nActivez cette option dans les paramètres par push [✅☑Activer l'abonnement]",
     'zh': "👮🏽 準備好了！ 已配置對 {0} 頻道的訂閱檢查\n\n通過推送在“設置”中打開此選項 [✅☑啟用訂閱]",
     'ar': "👮🏽 جاهز! التحقق من الاشتراك في {0} - تم تكوين القناة \n\n قم بتشغيل هذا الخيار في الإعدادات عن طريق الدفع [✅☑ تمكين الاشتراك]",
 }
-l_parse_rights = {
-    'ru': "👩🏽‍💻 В настройках [Администраторы] вкл опцию для @{0}-бота:\n[✅ Назначение администраторов]\n\n🕚Подожди 1min",
-    'en': "In the Settings [Administrators] for @{0} enable:\n[✅ Delete Msgs]\n[✅ Ban Users]\n[✅ Invite Users]\n🕚Wait for 1min",
-    'es': "En la Configuración [Administradores] para @{0} active:\n[✅ Eliminar mensajes]\n[✅ Prohibir usuarios]\n[✅ Invitar usuarios]\n🕚Espere 1 minuto",
-    'fr': "Dans les paramètres [Administrateurs] pour @{0}, activez :\n[✅ Supprimer les messages]\n[✅ Bannir les utilisateurs]\n[✅ Inviter des utilisateurs]\n🕚Attendez 1 minute",
-    'zh': "在@{0}的設置[管理員]中打開：\n[✅刪除消息]\n[✅禁止用戶]\n[✅邀請用戶]\n🕚等待1分鐘",
-    'ar': " في الإعدادات [Administrators] لـ @{0} شغّل:\n [✅ حذف الرسائل] \n على [✅ حظر المستخدمين] \n [✅ دعوة المستخدمين] \n وانتظر لمدة دقيقة واحدة",
-}
 l_videochat_rights = {
     'ru': "🎥 В настройках [Администраторы] вкл опцию для @{0}-бота:\n[✅ Назначение администраторов]\n[✅ Управление трансляциями]\n\n🕚Подожди 1min",
     'en': "In the Settings [Administrators] for @{0} enable:\n[✅ Delete Msgs]\n[✅ Ban Users]\n[✅ Invite Users]\n🕚Wait for 1min",
     'es': "En la Configuración [Administradores] para @{0} active:\n[✅ Eliminar mensajes]\n[✅ Prohibir usuarios]\n[✅ Invitar usuarios]\n🕚Espere 1 minuto",
     'fr': "Dans les paramètres [Administrateurs] pour @{0}, activez :\n[✅ Supprimer les messages]\n[✅ Bannir les utilisateurs]\n[✅ Inviter des utilisateurs]\n🕚Attendez 1 minute",
     'zh': "在@{0}的設置[管理員]中打開：\n[✅刪除消息]\n[✅禁止用戶]\n[✅邀請用戶]\n🕚等待1分鐘",
     'ar': " في الإعدادات [Administrators] لـ @{0} شغّل:\n [✅ حذف الرسائل] \n على [✅ حظر المستخدمين] \n [✅ دعوة المستخدمين] \n وانتظر لمدة دقيقة واحدة",
@@ -3235,23 +3251,23 @@
     'en': "🎥 Send this command as reply to message",
     'es': "🎥 Enviar este comando como respuesta al mensaje",
     'fr': "🎥 Envoyez cette commande en réponse au message",
     'zh': "🎥 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_ban_users_start = {
-    'ru': "👩🏽‍💻 Начинаем очистку канала\nТекущее количество пользователей: {0}",
+    'ru': "👩🏽‍💻 Начинаем очистку канала\nТекущее количество пользователей в базе: {0}",
     'en': "🎥 Send this command as reply to message",
     'es': "🎥 Enviar este comando como respuesta al mensaje",
     'fr': "🎥 Envoyez cette commande en réponse au message",
     'zh': "🎥 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_ban_users_stop = {
-    'ru': "👩🏽‍💻 Очистка завершена\nТекущее количество пользователей {0} (-{1})",
+    'ru': "👩🏽‍💻 Очистка завершена\nТекущее количество пользователей в базе: {0} (-{1})",
     'en': "🎥 Send this command as reply to message",
     'es': "🎥 Enviar este comando como respuesta al mensaje",
     'fr': "🎥 Envoyez cette commande en réponse au message",
     'zh': "🎥 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_ccheck_handler = {
@@ -3274,14 +3290,22 @@
     'ru': "👮🏽 В настройках [Администраторы] вкл опцию для @{0}-бота:\n[✅ Удаление сообщ]\n[✅ Блокировка польз]\n[✅ Добавление участ]\n\n🕚Подожди 1min",
     'en': "👮🏽 In the Settings [Administrators] for @{0} enable:\n[✅ Delete Msgs]\n[✅ Ban Users]\n[✅ Invite Users]\n🕚Wait for 1min",
     'es': "👮🏽 En la Configuración [Administradores] para @{0} active:\n[✅ Eliminar mensajes]\n[✅ Prohibir usuarios]\n[✅ Invitar usuarios]\n🕚Espere 1 minuto",
     'fr': "👮🏽 Dans les paramètres [Administrateurs] pour @{0}, activez :\n[✅ Supprimer les messages]\n[✅ Bannir les utilisateurs]\n[✅ Inviter des utilisateurs]\n🕚Attendez 1 minute",
     'zh': "👮🏽 在@{0}的設置[管理員]中打開：\n[✅刪除消息]\n[✅禁止用戶]\n[✅邀請用戶]\n🕚等待1分鐘",
     'ar': " في الإعدادات [Administrators] لـ @{0} شغّل:\n [✅ حذف الرسائل] \n على [✅ حظر المستخدمين] \n [✅ دعوة المستخدمين] \n وانتظر لمدة دقيقة واحدة",
 }
+l_ccheck_chn_finish = {
+    'ru': "👮🏽 <b>Добро пожаловать</b>:\n\n{0}",
+    'en': "👮🏽 To check <i>subscription</i> you have to add channel by command:\n\n/channel LINK",
+    'es': "👮🏽 Para verificar la <i>suscripción</i>, debe agregar el canal mediante el comando:\n\n/channel LINK",
+    'fr': "👮🏽 Pour vérifier l'<i>abonnement</i>, vous devez ajouter une chaîne par commande :\n\n/channel LINK",
+    'zh': "👮🏽 要檢查<i>訂閱</i>，您必須通過命令添加頻道：\n\n/channel LINK",
+    'ar': "👮🏽 للتحقق من <i> اشتراك </i> ، عليك إضافة قناة بأمر: \n\n/ channel LINK",
+}
 l_ccheck_free_on = {
     'ru': "✅☑Вкл свободный вход",
     'en': "✅☑On free entrance",
     'es': "✅☑En entrada libre",
     'fr': "✅☑En entrée libre",
     'zh': "✅☑免費入場",
     'ar': "✅☑ الدخول مجاني",
@@ -3830,10 +3854,18 @@
     'ru': "👥 Готово! Собрано реальных участников: <u>{0}</u>\n\n👩🏽‍💻 Остальные подписчики будут постепенно пополнять базу, пока у @{1}-бота есть права [✅ Назначение администраторов]\n\n{2}",
     'en': "👥 Ready! Gathered members: <u>{0}</u>. You can immediately make an <b>sending</b> or <b>inviting</b> to channel by received members{1}",
     'es': "👥 Listo! Miembros reunidos: <u>{0}</u>. Inmediatamente puede hacer un <b>envío</b> o <b>invitación</b> al grupo por miembros recibidos{1}",
     'fr': "👥 Prêt ! Membres réunis : <u>{0}</u>. Vous pouvez immédiatement faire un <b>envoi</b> ou <b>inviter</b> pour channeler par membres reçus{1}",
     'zh': "👥 準備好了！ 聚集成員：<u>{0}</u>。 您可以立即<b>發送</b>或<b>邀請</b>按收到的成員分組{1}",
     'ar': "🔥 جاهز! الأعضاء الذين تم تجميعهم: <u>{0}</u>. يمكنك على الفور إجراء <b> إرسال </b> أو <b> دعوة </b> للانضمام إلى المجموعة بواسطة الأعضاء المستلمين {1}",
 }
+l_parse_rights = {
+    'ru': "👥 В настройках [Администраторы] вкл опцию для @{0}-бота:\n[✅ Назначение администраторов]\n🕚Подожди 1min\n👩🏽‍💻 Выполни команду /parse\n\n⚙️ <b>Команды</b> /cmd",
+    'en': "In the Settings [Administrators] for @{0} enable:\n[✅ Delete Msgs]\n[✅ Ban Users]\n[✅ Invite Users]\n🕚Wait for 1min",
+    'es': "En la Configuración [Administradores] para @{0} active:\n[✅ Eliminar mensajes]\n[✅ Prohibir usuarios]\n[✅ Invitar usuarios]\n🕚Espere 1 minuto",
+    'fr': "Dans les paramètres [Administrateurs] pour @{0}, activez :\n[✅ Supprimer les messages]\n[✅ Bannir les utilisateurs]\n[✅ Inviter des utilisateurs]\n🕚Attendez 1 minute",
+    'zh': "在@{0}的設置[管理員]中打開：\n[✅刪除消息]\n[✅禁止用戶]\n[✅邀請用戶]\n🕚等待1分鐘",
+    'ar': " في الإعدادات [Administrators] لـ @{0} شغّل:\n [✅ حذف الرسائل] \n على [✅ حظر المستخدمين] \n [✅ دعوة المستخدمين] \n وانتظر لمدة دقيقة واحدة",
+}
 # endregion
 # endregion
```

### Comparing `yeref-0.1.47/yeref/yeref.py` & `yeref-0.1.48/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,18 +89,18 @@
           f'%B5%D0%B3%D0%BE%20%D0%BF%D1%80%D0%BE%D0%B4%D1%83%D0%BA%D1%82%D0%B0!'
 
 ferey_thumb = 'https://telegra.ph/file/bf7d8c073cdfa91b6d624.jpg'
 ferey_theme = 'https://t.me/addtheme/lzbKZktZjqv5VDdY'
 ferey_wp = 'https://t.me/bg/Mr2tXPkzQUoGAgAAv-ssUh01-P4'
 ferey_set = 'https://t.me/addstickers/Mr2tXPkzQUoGAgAAv-ssUh01-P4'
 ferey_emoji = 'https://t.me/addemoji/Mr2tXPkzQUoGAgAAv-ssUh01-P4'
-reactions_ = ['👍', '👎', '❤', '🔥', '🥰', '👏', '😁', '🤔', '🤯', '😱', '🤬', '😢', '🎉', '🤩', '🤮', '💩', '🙏',
+reactions_ = ['👍', '❤', '🔥', '🥰', '👏', '😁', '🤔', '🤯', '😱', '🤬', '😢', '🎉', '🤩', '🙏',
               '👌', '🕊', '🤡', '🥱', '🥴', '😍', '🐳', '❤\u200d🔥', '🌚', '🌭', '💯', '🤣', '⚡', '🍌', '🏆',
-              '💔', '🤨', '😐', '🍓', '🍾', '💋', '🖕', '😈', '😴', '😭', '🤓', '👻', '👨\u200d💻', '👀', '🎃',
-              '🙈', '😇', '😨', '🤝', '✍', '🤗', '\U0001fae1', '😂']
+              '💔', '🤨', '😐', '🍓', '🍾', '💋', '😈', '😴', '😭', '🤓', '👻', '👨\u200d💻', '👀', '🎃',
+              '🙈', '😇', '😨', '🤝', '✍', '🤗', '\U0001fae1', '😂', '🎄', '⛄', ' 🆒', '🗿']
 themes_ = ['🐥', '⛄', '💎', '👨\u200d🏫', '🌷', '💜', '🎄', '🎮']  # все в порядке, все ставятся, если не стояли
 bot_father = "@BotFather"
 text_jpeg = 'https://telegra.ph/file/0c675e5a3724deff3b2e1.jpg'
 bot_logo_jpeg = 'https://telegra.ph/file/99d4f150a52dcf78b3e8a.jpg'
 channel_logo_jpeg = 'https://telegra.ph/file/8418e1cd70484eac89477.jpg'
 group_logo_jpeg = 'https://telegra.ph/file/807e0d4fc4f271899272a.jpg'
 payment_photo = 'https://telegra.ph/file/75747cf7bc68f45a0e8b8.jpg'
```

