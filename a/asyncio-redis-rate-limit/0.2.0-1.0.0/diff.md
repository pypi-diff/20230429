# Comparing `tmp/asyncio-redis-rate-limit-0.2.0.tar.gz` & `tmp/asyncio_redis_rate_limit-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncio-redis-rate-limit-0.2.0.tar", max compression
+gzip compressed data, was "asyncio_redis_rate_limit-1.0.0.tar", max compression
```

## Comparing `asyncio-redis-rate-limit-0.2.0.tar` & `asyncio_redis_rate_limit-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1103 2022-06-22 15:33:15.888445 asyncio-redis-rate-limit-0.2.0/LICENSE
--rw-r--r--   0        0        0     3387 2022-06-28 06:48:25.939082 asyncio-redis-rate-limit-0.2.0/README.md
--rw-r--r--   0        0        0     4418 2022-06-28 06:48:25.939476 asyncio-redis-rate-limit-0.2.0/asyncio_redis_rate_limit/__init__.py
--rw-r--r--   0        0        0     1897 2022-06-27 09:04:01.161719 asyncio-redis-rate-limit-0.2.0/asyncio_redis_rate_limit/compat.py
--rw-r--r--   0        0        0        0 2022-06-22 15:33:15.593512 asyncio-redis-rate-limit-0.2.0/asyncio_redis_rate_limit/py.typed
--rw-r--r--   0        0        0     1431 2022-06-28 06:49:39.806042 asyncio-redis-rate-limit-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4355 2022-06-28 08:18:15.286649 asyncio-redis-rate-limit-0.2.0/setup.py
--rw-r--r--   0        0        0     4623 2022-06-28 08:18:15.286992 asyncio-redis-rate-limit-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1103 2022-06-22 15:33:15.888445 asyncio_redis_rate_limit-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3448 2023-04-29 13:29:49.572418 asyncio_redis_rate_limit-1.0.0/README.md
+-rw-r--r--   0        0        0     4500 2023-04-29 12:05:40.482571 asyncio_redis_rate_limit-1.0.0/asyncio_redis_rate_limit/__init__.py
+-rw-r--r--   0        0        0     1897 2022-06-27 09:04:01.161719 asyncio_redis_rate_limit-1.0.0/asyncio_redis_rate_limit/compat.py
+-rw-r--r--   0        0        0        0 2022-06-22 15:33:15.593512 asyncio_redis_rate_limit-1.0.0/asyncio_redis_rate_limit/py.typed
+-rw-r--r--   0        0        0     1564 2023-04-29 13:29:49.583616 asyncio_redis_rate_limit-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4787 1970-01-01 00:00:00.000000 asyncio_redis_rate_limit-1.0.0/PKG-INFO
```

### Comparing `asyncio-redis-rate-limit-0.2.0/LICENSE` & `asyncio_redis_rate_limit-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncio-redis-rate-limit-0.2.0/README.md` & `asyncio_redis_rate_limit-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,27 @@
 - Small and simple
 - Can be used as a decorator or as a context manager
 - Can be used for both clients and servers
 - Works with `asyncio`
 - Works with any amount of processes
 - Works with both [`redis.asyncio.client.Redis`](https://redis-py.readthedocs.io/en/stable/examples/asyncio_examples.html) and [`aioredis`](https://github.com/aio-libs/aioredis-py)
 - Free of race-conditions (hopefully!)
+- Supports `redis` since `7.0`
 - Fully typed with annotations and checked with mypy, [PEP561 compatible](https://www.python.org/dev/peps/pep-0561/)
 
 
 ## Installation
 
 ```bash
 pip install asyncio-redis-rate-limit
 ```
 
 Extras available:
 - `pip install asyncio-redis-rate-limit[redis]`
-- `pip install asyncio-redis-rate-limit[aioredis]`
+- `pip install asyncio-redis-rate-limit[aioredis]` (for python versions `<3.11`)
 
 
 ## Example
 
 As a decorator:
 
 ```python
```

### Comparing `asyncio-redis-rate-limit-0.2.0/asyncio_redis_rate_limit/__init__.py` & `asyncio_redis_rate_limit-1.0.0/asyncio_redis_rate_limit/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,15 +92,16 @@
             rate_spec=self._rate_spec,
             cache_prefix=self._cache_prefix,
         )
         pipeline = self._backend.pipeline()
 
         async with self._lock:
             current_rate = await self._run_pipeline(cache_key, pipeline)
-            if current_rate > self._rate_spec.requests:
+            # This looks like a coverage error on 3.10:
+            if current_rate > self._rate_spec.requests:  # pragma: no cover
                 raise RateLimitError('Rate limit is hit', current_rate)
 
     async def _run_pipeline(
         self,
         cache_key: str,
         pipeline: AnyPipeline,
     ) -> int:
@@ -115,15 +116,15 @@
     def _make_cache_key(
         self,
         unique_key: str,
         rate_spec: RateSpec,
         cache_prefix: str,
     ) -> str:
         parts = ''.join([unique_key, str(rate_spec)])
-        return cache_prefix + hashlib.md5(  # noqa: S303
+        return cache_prefix + hashlib.md5(  # noqa: S303, S324
             parts.encode('utf-8'),
         ).hexdigest()
 
 
 def rate_limit(
     rate_spec: RateSpec,
     backend: AnyRedis,
```

### Comparing `asyncio-redis-rate-limit-0.2.0/asyncio_redis_rate_limit/compat.py` & `asyncio_redis_rate_limit-1.0.0/asyncio_redis_rate_limit/compat.py`

 * *Files identical despite different names*

### Comparing `asyncio-redis-rate-limit-0.2.0/setup.py` & `asyncio_redis_rate_limit-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,112 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: asyncio-redis-rate-limit
+Version: 1.0.0
+Summary: Rate limiter for async functions using Redis as a backend
+Home-page: https://github.com/wemake-services/asyncio-redis-rate-limit
+License: MIT
+Keywords: asyncio,rate-limiter,redis,redis-py,aioredis
+Author: Nikita Sobolev
+Author-email: mail@sobolevn.me
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: aioredis
+Provides-Extra: dev
+Provides-Extra: redis
+Requires-Dist: aioredis (>=2.0) ; (python_version < "3.11") and (extra == "aioredis" or extra == "dev")
+Requires-Dist: redis (>=4.5,<5) ; extra == "redis" or extra == "dev"
+Requires-Dist: typing-extensions (>=3.10)
+Project-URL: Funding, https://github.com/sponsors/wemake-services
+Project-URL: Repository, https://github.com/wemake-services/asyncio-redis-rate-limit
+Description-Content-Type: text/markdown
 
-packages = \
-['asyncio_redis_rate_limit']
+# asyncio-redis-rate-limit
 
-package_data = \
-{'': ['*']}
+[![wemake.services](https://img.shields.io/badge/%20-wemake.services-green.svg?label=%20&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAABGdBTUEAALGPC%2FxhBQAAAAFzUkdCAK7OHOkAAAAbUExURQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAP%2F%2F%2F5TvxDIAAAAIdFJOUwAjRA8xXANAL%2Bv0SAAAADNJREFUGNNjYCAIOJjRBdBFWMkVQeGzcHAwksJnAPPZGOGAASzPzAEHEGVsLExQwE7YswCb7AFZSF3bbAAAAABJRU5ErkJggg%3D%3D)](https://wemake-services.github.io)
+[![Build Status](https://github.com/wemake-services/asyncio-redis-rate-limit/workflows/test/badge.svg?branch=master&event=push)](https://github.com/wemake-services/asyncio-redis-rate-limit/actions?query=workflow%3Atest)
+[![codecov](https://codecov.io/gh/wemake-services/asyncio-redis-rate-limit/branch/master/graph/badge.svg)](https://codecov.io/gh/wemake-services/asyncio-redis-rate-limit)
+[![Python Version](https://img.shields.io/pypi/pyversions/asyncio-redis-rate-limit.svg)](https://pypi.org/project/asyncio-redis-rate-limit/)
+[![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide)
 
-install_requires = \
-['typing-extensions>=3.10']
-
-extras_require = \
-{'aioredis': ['aioredis>=2.0'],
- 'dev': ['redis>=4.3', 'aioredis>=2.0'],
- 'redis': ['redis>=4.3']}
-
-setup_kwargs = {
-    'name': 'asyncio-redis-rate-limit',
-    'version': '0.2.0',
-    'description': 'Rate limiter for async functions using Redis as a backend',
-    'long_description': "# asyncio-redis-rate-limit\n\n[![wemake.services](https://img.shields.io/badge/%20-wemake.services-green.svg?label=%20&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAABGdBTUEAALGPC%2FxhBQAAAAFzUkdCAK7OHOkAAAAbUExURQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAP%2F%2F%2F5TvxDIAAAAIdFJOUwAjRA8xXANAL%2Bv0SAAAADNJREFUGNNjYCAIOJjRBdBFWMkVQeGzcHAwksJnAPPZGOGAASzPzAEHEGVsLExQwE7YswCb7AFZSF3bbAAAAABJRU5ErkJggg%3D%3D)](https://wemake-services.github.io)\n[![Build Status](https://github.com/wemake-services/asyncio-redis-rate-limit/workflows/test/badge.svg?branch=master&event=push)](https://github.com/wemake-services/asyncio-redis-rate-limit/actions?query=workflow%3Atest)\n[![codecov](https://codecov.io/gh/wemake-services/asyncio-redis-rate-limit/branch/master/graph/badge.svg)](https://codecov.io/gh/wemake-services/asyncio-redis-rate-limit)\n[![Python Version](https://img.shields.io/pypi/pyversions/asyncio-redis-rate-limit.svg)](https://pypi.org/project/asyncio-redis-rate-limit/)\n[![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide)\n\nRate limiter for async functions using Redis as a backend.\n\n\n## Features\n\n- Small and simple\n- Can be used as a decorator or as a context manager\n- Can be used for both clients and servers\n- Works with `asyncio`\n- Works with any amount of processes\n- Works with both [`redis.asyncio.client.Redis`](https://redis-py.readthedocs.io/en/stable/examples/asyncio_examples.html) and [`aioredis`](https://github.com/aio-libs/aioredis-py)\n- Free of race-conditions (hopefully!)\n- Fully typed with annotations and checked with mypy, [PEP561 compatible](https://www.python.org/dev/peps/pep-0561/)\n\n\n## Installation\n\n```bash\npip install asyncio-redis-rate-limit\n```\n\nExtras available:\n- `pip install asyncio-redis-rate-limit[redis]`\n- `pip install asyncio-redis-rate-limit[aioredis]`\n\n\n## Example\n\nAs a decorator:\n\n```python\n>>> from asyncio_redis_rate_limit import rate_limit, RateSpec\n>>> from redis.asyncio import Redis as AsyncRedis  # pip install redis\n\n>>> redis = AsyncRedis.from_url('redis://localhost:6379')\n\n>>> @rate_limit(\n...    rate_spec=RateSpec(requests=1200, seconds=60),\n...    backend=redis,\n... )\n... async def request() -> ...:\n...     ...   # Do something useful! Call this function as usual.\n\n```\n\nOr as a context manager:\n\n```python\n>>> from asyncio_redis_rate_limit import RateLimiter, RateSpec\n>>> from redis.asyncio import Redis as AsyncRedis  # pip install redis\n\n>>> redis = AsyncRedis.from_url('redis://localhost:6379')\n\n>>> async def request() -> ...:\n...     async with RateLimiter(\n...         unique_key='api-name.com',\n...         backend=redis,\n...         rate_spec=RateSpec(requests=5, seconds=1),\n...     ):\n...         ...  # Do the request itself.\n\n```\n\n\n## License\n\n[MIT](https://github.com/wemake-services/asyncio-redis-rate-limit/blob/master/LICENSE)\n\n\n## Credits\n\nThis project was generated with [`wemake-python-package`](https://github.com/wemake-services/wemake-python-package). Current template version is: [1d63652fbb33ebe2f6d932f511b7f529a4ce2d2a](https://github.com/wemake-services/wemake-python-package/tree/1d63652fbb33ebe2f6d932f511b7f529a4ce2d2a). See what is [updated](https://github.com/wemake-services/wemake-python-package/compare/1d63652fbb33ebe2f6d932f511b7f529a4ce2d2a...master) since then.\n",
-    'author': 'Nikita Sobolev',
-    'author_email': 'mail@sobolevn.me',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/wemake-services/asyncio-redis-rate-limit',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
+Rate limiter for async functions using Redis as a backend.
 
 
-setup(**setup_kwargs)
+## Features
+
+- Small and simple
+- Can be used as a decorator or as a context manager
+- Can be used for both clients and servers
+- Works with `asyncio`
+- Works with any amount of processes
+- Works with both [`redis.asyncio.client.Redis`](https://redis-py.readthedocs.io/en/stable/examples/asyncio_examples.html) and [`aioredis`](https://github.com/aio-libs/aioredis-py)
+- Free of race-conditions (hopefully!)
+- Supports `redis` since `7.0`
+- Fully typed with annotations and checked with mypy, [PEP561 compatible](https://www.python.org/dev/peps/pep-0561/)
+
+
+## Installation
+
+```bash
+pip install asyncio-redis-rate-limit
+```
+
+Extras available:
+- `pip install asyncio-redis-rate-limit[redis]`
+- `pip install asyncio-redis-rate-limit[aioredis]` (for python versions `<3.11`)
+
+
+## Example
+
+As a decorator:
+
+```python
+>>> from asyncio_redis_rate_limit import rate_limit, RateSpec
+>>> from redis.asyncio import Redis as AsyncRedis  # pip install redis
+
+>>> redis = AsyncRedis.from_url('redis://localhost:6379')
+
+>>> @rate_limit(
+...    rate_spec=RateSpec(requests=1200, seconds=60),
+...    backend=redis,
+... )
+... async def request() -> ...:
+...     ...   # Do something useful! Call this function as usual.
+
+```
+
+Or as a context manager:
+
+```python
+>>> from asyncio_redis_rate_limit import RateLimiter, RateSpec
+>>> from redis.asyncio import Redis as AsyncRedis  # pip install redis
+
+>>> redis = AsyncRedis.from_url('redis://localhost:6379')
+
+>>> async def request() -> ...:
+...     async with RateLimiter(
+...         unique_key='api-name.com',
+...         backend=redis,
+...         rate_spec=RateSpec(requests=5, seconds=1),
+...     ):
+...         ...  # Do the request itself.
+
+```
+
+
+## License
+
+[MIT](https://github.com/wemake-services/asyncio-redis-rate-limit/blob/master/LICENSE)
+
+
+## Credits
+
+This project was generated with [`wemake-python-package`](https://github.com/wemake-services/wemake-python-package). Current template version is: [1d63652fbb33ebe2f6d932f511b7f529a4ce2d2a](https://github.com/wemake-services/wemake-python-package/tree/1d63652fbb33ebe2f6d932f511b7f529a4ce2d2a). See what is [updated](https://github.com/wemake-services/wemake-python-package/compare/1d63652fbb33ebe2f6d932f511b7f529a4ce2d2a...master) since then.
+
```

