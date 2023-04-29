# Comparing `tmp/tweepy_authlib-1.0.6.tar.gz` & `tmp/tweepy_authlib-1.1.0.tar.gz`

## Comparing `tweepy_authlib-1.0.6.tar` & `tweepy_authlib-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 tweepy_authlib-1.0.6/.editorconfig
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tweepy_authlib-1.0.6/.env.example
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 tweepy_authlib-1.0.6/example_json.py
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 tweepy_authlib-1.0.6/example_pickle.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 tweepy_authlib-1.0.6/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tweepy_authlib-1.0.6/tests/__init__.py
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 tweepy_authlib-1.0.6/tests/test_main.py
--rw-r--r--   0        0        0    27949 2020-02-02 00:00:00.000000 tweepy_authlib-1.0.6/tweepy_authlib/CookieSessionUserHandler.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tweepy_authlib-1.0.6/tweepy_authlib/__about__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tweepy_authlib-1.0.6/tweepy_authlib/__init__.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 tweepy_authlib-1.0.6/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 tweepy_authlib-1.0.6/License.txt
--rw-r--r--   0        0        0     9026 2020-02-02 00:00:00.000000 tweepy_authlib-1.0.6/Readme.md
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 tweepy_authlib-1.0.6/pyproject.toml
--rw-r--r--   0        0        0    10277 2020-02-02 00:00:00.000000 tweepy_authlib-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 tweepy_authlib-1.1.0/.editorconfig
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tweepy_authlib-1.1.0/.env.example
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 tweepy_authlib-1.1.0/example_json.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 tweepy_authlib-1.1.0/example_pickle.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 tweepy_authlib-1.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tweepy_authlib-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 tweepy_authlib-1.1.0/tests/test_main.py
+-rw-r--r--   0        0        0    30327 2020-02-02 00:00:00.000000 tweepy_authlib-1.1.0/tweepy_authlib/CookieSessionUserHandler.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tweepy_authlib-1.1.0/tweepy_authlib/__about__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tweepy_authlib-1.1.0/tweepy_authlib/__init__.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 tweepy_authlib-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 tweepy_authlib-1.1.0/License.txt
+-rw-r--r--   0        0        0    11188 2020-02-02 00:00:00.000000 tweepy_authlib-1.1.0/Readme.md
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 tweepy_authlib-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    12439 2020-02-02 00:00:00.000000 tweepy_authlib-1.1.0/PKG-INFO
```

### Comparing `tweepy_authlib-1.0.6/example_json.py` & `tweepy_authlib-1.1.0/example_pickle.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import dotenv
 import os
-import json
+import pickle
 import tweepy
 from pathlib import Path
-from requests.cookies import RequestsCookieJar
 from tweepy_authlib import CookieSessionUserHandler
 
 try:
     terminal_size = os.get_terminal_size().columns
 except OSError:
     terminal_size = 80
 
@@ -15,42 +14,55 @@
 dotenv.load_dotenv()
 screen_name = os.environ.get('TWITTER_SCREEN_NAME', 'your_screen_name')
 password = os.environ.get('TWITTER_PASSWORD', 'your_password')
 
 # 保存した Cookie を使って認証
 ## 毎回ログインすると不審なログインとして扱われる可能性が高くなるため、
 ## できるだけ以前認証した際に保存した Cookie を使って認証することを推奨
-if Path('cookie.json').exists():
+if Path('cookie.pickle').exists():
 
     # 保存した Cookie を読み込む
-    with open('cookie.json', 'r') as f:
-        cookies_dict = json.load(f)
-
-    # RequestCookieJar オブジェクトに変換
-    cookies = RequestsCookieJar()
-    for key, value in cookies_dict.items():
-        cookies.set(key, value)
+    with open('cookie.pickle', 'rb') as f:
+        cookies = pickle.load(f)
 
     # 読み込んだ RequestCookieJar オブジェクトを CookieSessionUserHandler に渡す
     auth_handler = CookieSessionUserHandler(cookies=cookies)
 
 # スクリーンネームとパスワードを指定して認証
 else:
 
     # スクリーンネームとパスワードを渡す
-    ## スクリーンネームまたはパスワードが間違っている場合は、tweepy.BadRequest がスローされる
-    auth_handler = CookieSessionUserHandler(screen_name=screen_name, password=password)
+    ## スクリーンネームとパスワードを指定する場合は初期化時に認証のための API リクエストが多数行われるため、完了まで数秒かかる
+    try:
+        auth_handler = CookieSessionUserHandler(screen_name=screen_name, password=password)
+    except tweepy.HTTPException as ex:
+        # パスワードが間違っているなどの理由で認証に失敗した場合
+        if len(ex.api_codes) > 0 and len(ex.api_messages) > 0:
+            error_message = f'Code: {ex.api_codes[0]}, Message: {ex.api_messages[0]}'
+        else:
+            error_message = 'Unknown Error'
+        raise Exception(f'Failed to authenticate with password ({error_message})')
+    except tweepy.TweepyException as ex:
+        # 認証フローの途中で予期せぬエラーが発生し、ログインに失敗した
+        error_message = f'Message: {ex}'
+        raise Exception(f'Unexpected error occurred while authenticate with password ({error_message})')
 
     # 現在のログインセッションの Cookie を取得
     cookies = auth_handler.get_cookies()
 
     # Cookie を pickle 化して保存
-    with open('cookie.json', 'w') as f:
-        json.dump(cookies.get_dict(), f, ensure_ascii=False, indent=4)
+    with open('cookie.pickle', 'wb') as f:
+        pickle.dump(cookies, f)
 
 # Tweepy で Twitter API v1.1 にアクセス
 api = tweepy.API(auth_handler)
 print('-' * terminal_size)
 print(api.verify_credentials())
 print('-' * terminal_size)
 print(api.home_timeline())
 print('-' * terminal_size)
+
+# 継続してログインしない場合は明示的にログアウト
+## 単に Cookie を消去するだけだと Twitter にセッションが残り続けてしまう
+## ログアウト後は、取得した Cookie では再認証できなくなる
+#auth_handler.logout()
+#os.unlink('cookie.pickle')
```

### Comparing `tweepy_authlib-1.0.6/tests/test_main.py` & `tweepy_authlib-1.1.0/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
             print(api.update_status(f'Hello, Twitter! (API Test Tweet, {datetime.datetime.now().strftime("%Y/%m/%d %H:%M:%S")})'))
         print('-' * terminal_size)
         print(user)
         print('-' * terminal_size)
         assert user.screen_name == os.environ['TWITTER_SCREEN_NAME']
         assert api.user_timeline(screen_name='elonmusk')[0].user.screen_name == 'elonmusk'
         api.home_timeline()
+        auth_handler.logout()
     else:
         pytest.skip('TWITTER_SCREEN_NAME or TWITTER_PASSWORD is not set.')
 
 
 if __name__ == '__main__':
     dotenv.load_dotenv()
     test_06()
```

### Comparing `tweepy_authlib-1.0.6/tweepy_authlib/CookieSessionUserHandler.py` & `tweepy_authlib-1.1.0/tweepy_authlib/CookieSessionUserHandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,15 @@
             password (Optional[str], optional): Twitter のパスワード. Defaults to None.
 
         Raises:
             ValueError: Cookie が指定されていないのに、スクリーンネームまたはパスワードが (もしくはどちらも) 指定されていない
             ValueError: スクリーンネームが空文字列
             ValueError: パスワードが空文字列
             tweepy.BadRequest: スクリーンネームまたはパスワードが間違っている
+            tweepy.HTTPException: サーバーエラーなどの問題でログインに失敗した
             tweepy.TweepyException: 認証フローの途中でエラーが発生し、ログインに失敗した
         """
 
         self.screen_name = screen_name
         self.password = password
 
         # Cookie が指定されていないのに、スクリーンネームまたはパスワードが (もしくはどちらも) 指定されていない
@@ -224,14 +225,51 @@
 
         Returns:
             str: RequestsCookieJar
         """
         return self._session.cookies
 
 
+    def logout(self) -> None:
+        """
+        ログアウト処理を行い、Twitter からセッションを切断する
+        単に Cookie を削除するだけだと Twitter にセッションが残り続けてしまうため、今後ログインしない場合は明示的にこのメソッドを呼び出すこと
+        このメソッドを呼び出した後は、取得した Cookie では再認証できなくなる
+
+        Raises:
+            tweepy.HTTPException: サーバーエラーなどの問題でログアウトに失敗した
+            tweepy.TweepyException: ログアウト処理中にエラーが発生した
+        """
+
+        # ログアウト API 専用ヘッダー
+        ## self._auth_flow_api_headers と基本的には共通なため、コピーして変更箇所のみ変更する
+        logout_headers = self._auth_flow_api_headers.copy()
+        logout_headers['content-type'] = 'application/x-www-form-urlencoded'
+        del logout_headers['x-guest-token']
+        logout_headers['x-twitter-auth-type'] = 'OAuth2Session'
+        ## ヘッダーの dict をアルファベット順にソート
+        logout_headers = dict(sorted(logout_headers.items(), key=lambda x: x[0]))
+
+        # ログアウト API にログアウトすることを伝える
+        ## この API を実行すると、サーバー側でセッションが切断され、今まで持っていたほとんどの Cookie が消去される
+        logout_api_response = self._session.post('https://api.twitter.com/1.1/account/logout.json', headers=logout_headers, data={
+            'redirectAfterLogout': 'https://twitter.com/account/switch',
+        })
+        if logout_api_response.status_code != 200:
+            raise self._get_tweepy_exception(logout_api_response)
+
+        # 基本固定値のようなので不要だが、念のためステータスチェック
+        try:
+            status = logout_api_response.json()['status']
+        except:
+            raise tweepy.TweepyException('Failed to logout (failed to parse response)')
+        if status != 'ok':
+            raise tweepy.TweepyException(f'Failed to logout (status: {status})')
+
+
     def _on_response_received(self, response: requests.Response, *args, **kwargs) -> None:
         """
         レスポンスが返ってきた際に自動的に CSRF トークンを更新するコールバック
 
         Args:
             response (requests.Response): レスポンス
         """
@@ -395,14 +433,15 @@
 
     def _login(self) -> None:
         """
         スクリーンネームとパスワードを使って認証し、ログインする
 
         Raises:
             tweepy.BadRequest: スクリーンネームまたはパスワードが間違っている
+            tweepy.HTTPException: サーバーエラーなどの問題でログインに失敗した
             tweepy.TweepyException: 認証フローの途中でエラーが発生し、ログインに失敗した
         """
 
         def get_flow_token(response: requests.Response) -> str:
             try:
                 data = response.json()
             except ValueError:
```

### Comparing `tweepy_authlib-1.0.6/.gitignore` & `tweepy_authlib-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tweepy_authlib-1.0.6/License.txt` & `tweepy_authlib-1.1.0/License.txt`

 * *Files identical despite different names*

### Comparing `tweepy_authlib-1.0.6/pyproject.toml` & `tweepy_authlib-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tweepy_authlib-1.0.6/PKG-INFO` & `tweepy_authlib-1.1.0/Readme.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1
-Name: tweepy-authlib
-Version: 1.0.6
-Summary: Twitter Web App (Web 版公式クライアント) の内部 API を使い、Tweepy でスクリーンネームとパスワードで認証するためのライブラリ
-Project-URL: Documentation, https://github.com/tsukumijima/tweepy-authlib
-Project-URL: Issues, https://github.com/tsukumijima/tweepy-authlib/issues
-Project-URL: Source, https://github.com/tsukumijima/tweepy-authlib
-Author: tsukumi
-License-Expression: MIT
-License-File: License.txt
-Keywords: Library,Tweepy,Twitter
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: Japanese
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.8
-Requires-Dist: brotli>=1.0.9
-Requires-Dist: js2py>=0.74
-Requires-Dist: tweepy>=4.12.1
-Description-Content-Type: text/markdown
-
 
 # tweepy-authlib
 
 [![PyPI - Version](https://img.shields.io/pypi/v/tweepy-authlib.svg)](https://pypi.org/project/tweepy-authlib)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tweepy-authlib.svg)](https://pypi.org/project/tweepy-authlib)
 
 -----
@@ -126,16 +98,28 @@
     # 読み込んだ RequestCookieJar オブジェクトを CookieSessionUserHandler に渡す
     auth_handler = CookieSessionUserHandler(cookies=cookies)
 
 # スクリーンネームとパスワードを指定して認証
 else:
 
     # スクリーンネームとパスワードを渡す
-    ## スクリーンネームまたはパスワードが間違っている場合は、tweepy.BadRequest がスローされる
-    auth_handler = CookieSessionUserHandler(screen_name='your_screen_name', password='your_password')
+    ## スクリーンネームとパスワードを指定する場合は初期化時に認証のための API リクエストが多数行われるため、完了まで数秒かかる
+    try:
+        auth_handler = CookieSessionUserHandler(screen_name='your_screen_name', password='your_password')
+    except tweepy.HTTPException as ex:
+        # パスワードが間違っているなどの理由で認証に失敗した場合
+        if len(ex.api_codes) > 0 and len(ex.api_messages) > 0:
+            error_message = f'Code: {ex.api_codes[0]}, Message: {ex.api_messages[0]}'
+        else:
+            error_message = 'Unknown Error'
+        raise Exception(f'Failed to authenticate with password ({error_message})')
+    except tweepy.TweepyException as ex:
+        # 認証フローの途中で予期せぬエラーが発生し、ログインに失敗した
+        error_message = f'Message: {ex}'
+        raise Exception(f'Unexpected error occurred while authenticate with password ({error_message})')
 
     # 現在のログインセッションの Cookie を取得
     cookies = auth_handler.get_cookies()
 
     # Cookie を pickle 化して保存
     with open('cookie.json', 'w') as f:
         json.dump(cookies.get_dict(), f, ensure_ascii=False, indent=4)
@@ -143,14 +127,20 @@
 # Tweepy で Twitter API v1.1 にアクセス
 api = tweepy.API(auth_handler)
 print('-' * terminal_size)
 print(api.verify_credentials())
 print('-' * terminal_size)
 print(api.home_timeline())
 print('-' * terminal_size)
+
+# 継続してログインしない場合は明示的にログアウト
+## 単に Cookie を消去するだけだと Twitter にセッションが残り続けてしまう
+## ログアウト後は、取得した Cookie では再認証できなくなる
+#auth_handler.logout()
+#os.unlink('cookie.json')
 ```
 
 ### With Pickle
 
 ```python
 import os
 import pickle
@@ -175,16 +165,28 @@
     # 読み込んだ RequestCookieJar オブジェクトを CookieSessionUserHandler に渡す
     auth_handler = CookieSessionUserHandler(cookies=cookies)
 
 # スクリーンネームとパスワードを指定して認証
 else:
 
     # スクリーンネームとパスワードを渡す
-    ## スクリーンネームまたはパスワードが間違っている場合は、tweepy.BadRequest がスローされる
-    auth_handler = CookieSessionUserHandler(screen_name='your_screen_name', password='your_password')
+    ## スクリーンネームとパスワードを指定する場合は初期化時に認証のための API リクエストが多数行われるため、完了まで数秒かかる
+    try:
+        auth_handler = CookieSessionUserHandler(screen_name='your_screen_name', password='your_password')
+    except tweepy.HTTPException as ex:
+        # パスワードが間違っているなどの理由で認証に失敗した場合
+        if len(ex.api_codes) > 0 and len(ex.api_messages) > 0:
+            error_message = f'Code: {ex.api_codes[0]}, Message: {ex.api_messages[0]}'
+        else:
+            error_message = 'Unknown Error'
+        raise Exception(f'Failed to authenticate with password ({error_message})')
+    except tweepy.TweepyException as ex:
+        # 認証フローの途中で予期せぬエラーが発生し、ログインに失敗した
+        error_message = f'Message: {ex}'
+        raise Exception(f'Unexpected error occurred while authenticate with password ({error_message})')
 
     # 現在のログインセッションの Cookie を取得
     cookies = auth_handler.get_cookies()
 
     # Cookie を pickle 化して保存
     with open('cookie.pickle', 'wb') as f:
         pickle.dump(cookies, f)
@@ -192,12 +194,18 @@
 # Tweepy で Twitter API v1.1 にアクセス
 api = tweepy.API(auth_handler)
 print('-' * terminal_size)
 print(api.verify_credentials())
 print('-' * terminal_size)
 print(api.home_timeline())
 print('-' * terminal_size)
+
+# 継続してログインしない場合は明示的にログアウト
+## 単に Cookie を消去するだけだと Twitter にセッションが残り続けてしまう
+## ログアウト後は、取得した Cookie では再認証できなくなる
+#auth_handler.logout()
+#os.unlink('cookie.pickle')
 ```
 
 ## License
 
 [MIT License](License.txt)
```

