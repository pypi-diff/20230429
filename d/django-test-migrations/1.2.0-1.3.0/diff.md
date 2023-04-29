# Comparing `tmp/django-test-migrations-1.2.0.tar.gz` & `tmp/django_test_migrations-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-test-migrations-1.2.0.tar", max compression
+gzip compressed data, was "django_test_migrations-1.3.0.tar", max compression
```

## Comparing `django-test-migrations-1.2.0.tar` & `django_test_migrations-1.3.0.tar`

### file list

```diff
@@ -1,36 +1,35 @@
--rw-r--r--   0        0        0     1072 2019-11-21 13:08:51.945590 django-test-migrations-1.2.0/LICENSE
--rw-r--r--   0        0        0    11714 2021-12-13 22:11:43.423519 django-test-migrations-1.2.0/README.md
--rw-r--r--   0        0        0       24 2019-11-18 14:40:47.934023 django-test-migrations-1.2.0/django_test_migrations/__init__.py
--rw-r--r--   0        0        0        0 2021-01-05 09:32:19.116603 django-test-migrations-1.2.0/django_test_migrations/checks/__init__.py
--rw-r--r--   0        0        0     2689 2021-01-05 09:32:19.117113 django-test-migrations-1.2.0/django_test_migrations/checks/autonames.py
--rw-r--r--   0        0        0      340 2021-01-05 09:32:19.117313 django-test-migrations-1.2.0/django_test_migrations/checks/database_configuration.py
--rw-r--r--   0        0        0      156 2021-01-05 09:32:19.117453 django-test-migrations-1.2.0/django_test_migrations/constants.py
--rw-r--r--   0        0        0       24 2019-11-18 20:58:47.638663 django-test-migrations-1.2.0/django_test_migrations/contrib/__init__.py
--rw-r--r--   0        0        0     2174 2021-01-05 09:32:19.117808 django-test-migrations-1.2.0/django_test_migrations/contrib/django_checks.py
--rw-r--r--   0        0        0     2989 2021-03-15 07:27:54.885398 django-test-migrations-1.2.0/django_test_migrations/contrib/pytest_plugin.py
--rw-r--r--   0        0        0     2170 2021-01-05 09:32:19.118337 django-test-migrations-1.2.0/django_test_migrations/contrib/unittest_case.py
--rw-r--r--   0        0        0        0 2021-01-05 09:32:19.118466 django-test-migrations-1.2.0/django_test_migrations/db/__init__.py
--rw-r--r--   0        0        0      322 2021-01-05 09:32:19.118699 django-test-migrations-1.2.0/django_test_migrations/db/backends/__init__.py
--rw-r--r--   0        0        0        0 2021-01-05 09:32:19.118819 django-test-migrations-1.2.0/django_test_migrations/db/backends/base/__init__.py
--rw-r--r--   0        0        0     1231 2021-01-05 09:32:19.118986 django-test-migrations-1.2.0/django_test_migrations/db/backends/base/configuration.py
--rw-r--r--   0        0        0     1075 2021-01-05 09:32:19.119204 django-test-migrations-1.2.0/django_test_migrations/db/backends/exceptions.py
--rw-r--r--   0        0        0        0 2021-01-05 09:32:19.119439 django-test-migrations-1.2.0/django_test_migrations/db/backends/mysql/__init__.py
--rw-r--r--   0        0        0      867 2021-01-05 09:32:19.119812 django-test-migrations-1.2.0/django_test_migrations/db/backends/mysql/configuration.py
--rw-r--r--   0        0        0        0 2021-01-05 09:32:19.119971 django-test-migrations-1.2.0/django_test_migrations/db/backends/postgresql/__init__.py
--rw-r--r--   0        0        0      991 2021-01-05 09:32:19.120147 django-test-migrations-1.2.0/django_test_migrations/db/backends/postgresql/configuration.py
--rw-r--r--   0        0        0     1172 2021-02-12 12:20:39.984884 django-test-migrations-1.2.0/django_test_migrations/db/backends/registry.py
--rw-r--r--   0        0        0        0 2021-01-05 09:32:19.120403 django-test-migrations-1.2.0/django_test_migrations/db/checks/__init__.py
--rw-r--r--   0        0        0     3475 2021-01-05 09:32:19.120559 django-test-migrations-1.2.0/django_test_migrations/db/checks/statement_timeout.py
--rw-r--r--   0        0        0      492 2021-01-05 09:32:19.120692 django-test-migrations-1.2.0/django_test_migrations/exceptions.py
--rw-r--r--   0        0        0        0 2021-01-05 09:32:19.120808 django-test-migrations-1.2.0/django_test_migrations/logic/__init__.py
--rw-r--r--   0        0        0      190 2021-01-05 09:32:19.121033 django-test-migrations-1.2.0/django_test_migrations/logic/datetime.py
--rw-r--r--   0        0        0      354 2021-01-05 09:32:19.121163 django-test-migrations-1.2.0/django_test_migrations/logic/migrations.py
--rw-r--r--   0        0        0     3039 2021-01-05 09:32:19.122074 django-test-migrations-1.2.0/django_test_migrations/migrator.py
--rw-r--r--   0        0        0     4597 2021-02-12 12:20:26.260767 django-test-migrations-1.2.0/django_test_migrations/plan.py
--rw-r--r--   0        0        0        0 2019-11-18 17:27:26.682463 django-test-migrations-1.2.0/django_test_migrations/py.typed
--rw-r--r--   0        0        0      532 2021-01-05 09:32:19.122875 django-test-migrations-1.2.0/django_test_migrations/signals.py
--rw-r--r--   0        0        0     4270 2021-01-05 09:32:19.123177 django-test-migrations-1.2.0/django_test_migrations/sql.py
--rw-r--r--   0        0        0      799 2021-01-05 09:32:19.123363 django-test-migrations-1.2.0/django_test_migrations/types.py
--rw-r--r--   0        0        0     1622 2021-12-13 22:08:37.509186 django-test-migrations-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    13427 2021-12-13 22:15:38.400358 django-test-migrations-1.2.0/setup.py
--rw-r--r--   0        0        0    13134 2021-12-13 22:15:38.401194 django-test-migrations-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2019-11-21 13:08:51.945590 django_test_migrations-1.3.0/LICENSE
+-rw-r--r--   0        0        0    12260 2023-04-29 15:18:40.815072 django_test_migrations-1.3.0/README.md
+-rw-r--r--   0        0        0       24 2019-11-18 14:40:47.934023 django_test_migrations-1.3.0/django_test_migrations/__init__.py
+-rw-r--r--   0        0        0        0 2021-01-05 09:32:19.116603 django_test_migrations-1.3.0/django_test_migrations/checks/__init__.py
+-rw-r--r--   0        0        0     2689 2021-01-05 09:32:19.117113 django_test_migrations-1.3.0/django_test_migrations/checks/autonames.py
+-rw-r--r--   0        0        0      340 2021-01-05 09:32:19.117313 django_test_migrations-1.3.0/django_test_migrations/checks/database_configuration.py
+-rw-r--r--   0        0        0      156 2021-01-05 09:32:19.117453 django_test_migrations-1.3.0/django_test_migrations/constants.py
+-rw-r--r--   0        0        0       24 2019-11-18 20:58:47.638663 django_test_migrations-1.3.0/django_test_migrations/contrib/__init__.py
+-rw-r--r--   0        0        0     2174 2021-01-05 09:32:19.117808 django_test_migrations-1.3.0/django_test_migrations/contrib/django_checks.py
+-rw-r--r--   0        0        0     2989 2021-03-15 07:27:54.885398 django_test_migrations-1.3.0/django_test_migrations/contrib/pytest_plugin.py
+-rw-r--r--   0        0        0     2170 2021-01-05 09:32:19.118337 django_test_migrations-1.3.0/django_test_migrations/contrib/unittest_case.py
+-rw-r--r--   0        0        0        0 2021-01-05 09:32:19.118466 django_test_migrations-1.3.0/django_test_migrations/db/__init__.py
+-rw-r--r--   0        0        0      322 2021-01-05 09:32:19.118699 django_test_migrations-1.3.0/django_test_migrations/db/backends/__init__.py
+-rw-r--r--   0        0        0        0 2021-01-05 09:32:19.118819 django_test_migrations-1.3.0/django_test_migrations/db/backends/base/__init__.py
+-rw-r--r--   0        0        0     1231 2023-04-29 15:06:03.487494 django_test_migrations-1.3.0/django_test_migrations/db/backends/base/configuration.py
+-rw-r--r--   0        0        0     1075 2021-01-05 09:32:19.119204 django_test_migrations-1.3.0/django_test_migrations/db/backends/exceptions.py
+-rw-r--r--   0        0        0        0 2021-01-05 09:32:19.119439 django_test_migrations-1.3.0/django_test_migrations/db/backends/mysql/__init__.py
+-rw-r--r--   0        0        0      867 2021-01-05 09:32:19.119812 django_test_migrations-1.3.0/django_test_migrations/db/backends/mysql/configuration.py
+-rw-r--r--   0        0        0        0 2021-01-05 09:32:19.119971 django_test_migrations-1.3.0/django_test_migrations/db/backends/postgresql/__init__.py
+-rw-r--r--   0        0        0      991 2021-01-05 09:32:19.120147 django_test_migrations-1.3.0/django_test_migrations/db/backends/postgresql/configuration.py
+-rw-r--r--   0        0        0     1172 2021-02-12 12:20:39.984884 django_test_migrations-1.3.0/django_test_migrations/db/backends/registry.py
+-rw-r--r--   0        0        0        0 2021-01-05 09:32:19.120403 django_test_migrations-1.3.0/django_test_migrations/db/checks/__init__.py
+-rw-r--r--   0        0        0     3477 2022-09-05 13:14:12.143851 django_test_migrations-1.3.0/django_test_migrations/db/checks/statement_timeout.py
+-rw-r--r--   0        0        0      492 2021-01-05 09:32:19.120692 django_test_migrations-1.3.0/django_test_migrations/exceptions.py
+-rw-r--r--   0        0        0        0 2021-01-05 09:32:19.120808 django_test_migrations-1.3.0/django_test_migrations/logic/__init__.py
+-rw-r--r--   0        0        0      192 2022-09-05 13:14:12.144952 django_test_migrations-1.3.0/django_test_migrations/logic/datetime.py
+-rw-r--r--   0        0        0      354 2021-01-05 09:32:19.121163 django_test_migrations-1.3.0/django_test_migrations/logic/migrations.py
+-rw-r--r--   0        0        0     3039 2021-01-05 09:32:19.122074 django_test_migrations-1.3.0/django_test_migrations/migrator.py
+-rw-r--r--   0        0        0     4597 2021-02-12 12:20:26.260767 django_test_migrations-1.3.0/django_test_migrations/plan.py
+-rw-r--r--   0        0        0        0 2019-11-18 17:27:26.682463 django_test_migrations-1.3.0/django_test_migrations/py.typed
+-rw-r--r--   0        0        0      532 2021-01-05 09:32:19.122875 django_test_migrations-1.3.0/django_test_migrations/signals.py
+-rw-r--r--   0        0        0     1668 2023-04-29 15:06:03.489644 django_test_migrations-1.3.0/django_test_migrations/sql.py
+-rw-r--r--   0        0        0      621 2023-04-29 15:06:03.489968 django_test_migrations-1.3.0/django_test_migrations/types.py
+-rw-r--r--   0        0        0     1561 2023-04-29 15:18:40.822412 django_test_migrations-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    13591 1970-01-01 00:00:00.000000 django_test_migrations-1.3.0/PKG-INFO
```

### Comparing `django-test-migrations-1.2.0/LICENSE` & `django_test_migrations-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-test-migrations-1.2.0/README.md` & `django_test_migrations-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # django-test-migrations
 
-[![wemake.services](https://img.shields.io/badge/%20-wemake.services-green.svg?label=%20&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAABGdBTUEAALGPC%2FxhBQAAAAFzUkdCAK7OHOkAAAAbUExURQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAP%2F%2F%2F5TvxDIAAAAIdFJOUwAjRA8xXANAL%2Bv0SAAAADNJREFUGNNjYCAIOJjRBdBFWMkVQeGzcHAwksJnAPPZGOGAASzPzAEHEGVsLExQwE7YswCb7AFZSF3bbAAAAABJRU5ErkJggg%3D%3D)](https://wemake.services)
+[![wemake.services](https://img.shields.io/badge/%20-wemake.services-green.svg?label=%20&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAABGdBTUEAALGPC%2FxhBQAAAAFzUkdCAK7OHOkAAAAbUExURQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAP%2F%2F%2F5TvxDIAAAAIdFJOUwAjRA8xXANAL%2Bv0SAAAADNJREFUGNNjYCAIOJjRBdBFWMkVQeGzcHAwksJnAPPZGOGAASzPzAEHEGVsLExQwE7YswCb7AFZSF3bbAAAAABJRU5ErkJggg%3D%3D)](https://wemake-services.github.io)
 [![Build status](https://github.com/wemake-services/django-test-migrations/workflows/test/badge.svg?branch=master&event=push)](https://github.com/wemake-services/django-test-migrations/actions?query=workflow%3Atest)
 [![codecov](https://codecov.io/gh/wemake-services/django-test-migrations/branch/master/graph/badge.svg)](https://codecov.io/gh/wemake-services/django-test-migrations)
 [![Python Version](https://img.shields.io/pypi/pyversions/django-test-migrations.svg)](https://pypi.org/project/django-test-migrations/)
 ![PyPI - Django Version](https://img.shields.io/pypi/djversions/django-test-migrations)
 [![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide)
 
 
@@ -26,32 +26,33 @@
 
 ```bash
 pip install django-test-migrations
 ```
 
 We support several `django` versions:
 
-- `1.11`
 - `2.2`
-- `3.1`
 - `3.2`
 - `4.0`
+- `4.1`
+- `4.2`
 
-Other versions might work too, but they are not officially supported.
+Other versions most likely will work too,
+but they are not officially supported.
 
 
-## Testing django migrations
+## Testing Django migrations
 
 Testing migrations is not a frequent thing in `django` land.
 But, sometimes it is totally required. When?
 
 When we do complex schema or data changes
 and what to be sure that existing data won't be corrupted.
 We might also want to be sure that all migrations can be safely rolled back.
-And as a final touch we want to be sure that migrations
+And as a final touch, we want to be sure that migrations
 are in the correct order and have correct dependencies.
 
 ### Testing forward migrations
 
 To test all migrations we have a [`Migrator`](https://github.com/wemake-services/django-test-migrations/blob/master/django_test_migrations/migrator.py) class.
 
 It has three methods to work with:
@@ -127,16 +128,16 @@
 
 # Cleanup:
 migrator.reset()
 ```
 
 ### Testing migrations ordering
 
-Sometimes we also want to be sure that our migrations are in the correct order.
-And all our `dependecies = [...]` are correct.
+Sometimes we also want to be sure that our migrations are in the correct order
+and that all our `dependencies = [...]` are correct.
 
 To achieve that we have [`plan.py`](https://github.com/wemake-services/django-test-migrations/blob/master/django_test_migrations/plan.py) module.
 
 That's how it can be used:
 
 ```python
 from django_test_migrations.plan import all_migrations, nodes_to_tuples
@@ -151,28 +152,50 @@
     ('other_app', '0002_auto_20191120_2230'),
 ]
 ```
 
 This way you can be sure that migrations
 and apps that depend on each other will be executed in the correct order.
 
+### `factory_boy` integration
+
+If you use factories to create models, you can replace their respective
+`.build()` or `.create()` calls with methods of `factory` and pass the
+model name and factory class as arguments:
+
+```python
+import factory
+
+old_state = migrator.apply_initial_migration(
+    ('main_app', '0002_someitem_is_clean'),
+)
+SomeItem = old_state.apps.get_model('main_app', 'SomeItem')
+
+# instead of
+# item = SomeItemFactory.create()
+# use this:
+factory.create(SomeItem, FACTORY_CLASS=SomeItemFactory)
+
+# ...
+```
+
 
 ## Test framework integrations 🐍
 
 We support several test frameworks as first-class citizens.
 That's a testing tool after all!
 
 Note that the Django `post_migrate` signal's receiver list is cleared at
 the start of tests and restored afterwards. If you need to test your
 own `post_migrate` signals then attach/remove them during a test.
 
 ### pytest
 
 We ship `django-test-migrations` with a `pytest` plugin
-that provides two convinient fixtures:
+that provides two convenient fixtures:
 
 - `migrator_factory` that gives you an opportunity
   to create `Migrator` classes for any database
 - `migrator` instance for the `'default'` database
 
 That's how it can be used:
 
@@ -181,15 +204,15 @@
 
 @pytest.mark.django_db()
 def test_pytest_plugin_initial(migrator):
     """Ensures that the initial migration works."""
     old_state = migrator.apply_initial_migration(('main_app', None))
 
     with pytest.raises(LookupError):
-        # Models does not yet exist:
+        # Model does not yet exist:
         old_state.apps.get_model('main_app', 'SomeItem')
 
     new_state = migrator.apply_tested_migration(('main_app', '0001_initial'))
     # After the initial migration is done, we can use the model state:
     SomeItem = new_state.apps.get_model('main_app', 'SomeItem')
     assert SomeItem.objects.filter(string_field='').count() == 0
 ```
@@ -233,42 +256,42 @@
 #### pytest
 
 `django_test_migrations` adds `migration_test` marker to each test using
 `migrator_factory` or `migrator` fixture.
 To run only migrations test, use `-m` option:
 
 ```bash
-pytest -m migration_test  # runs only migraion tests
-pytest -m "not migration_test"  # runs all except migraion tests
+pytest -m migration_test  # Runs only migration tests
+pytest -m "not migration_test"  # Runs all except migration tests
 ```
 
 #### unittest
 
 `django_test_migrations` adds `migration_test`
 [tag](https://docs.djangoproject.com/en/3.0/topics/testing/tools/#tagging-tests)
 to every `MigratorTestCase` subclass.
 To run only migrations tests, use `--tag` option:
 
 ```bash
-python mange.py test --tag=migration_test  # runs only migraion tests
-python mange.py test --exclude-tag=migration_test  # runs all except migraion tests
+python mange.py test --tag=migration_test  # Runs only migration tests
+python mange.py test --exclude-tag=migration_test  # Runs all except migration tests
 ```
 
 
 ## Django Checks
 
 `django_test_migrations` comes with 2 groups of Django's checks for:
 
 + detecting migrations scripts automatically generated names
 + validating some subset of database settings
 
 ### Testing migration names
 
 `django` generates migration names for you when you run `makemigrations`.
-And these names are bad ([read more](https://adamj.eu/tech/2020/02/24/how-to-disallow-auto-named-django-migrations/) about why it is bad)!
+These names are bad ([read more](https://adamj.eu/tech/2020/02/24/how-to-disallow-auto-named-django-migrations/) about why it is bad)!
 Just look at this: `0004_auto_20191119_2125.py`
 
 What does this migration do? What changes does it have?
 
 One can also pass `--name` attribute when creating migrations, but it is easy to forget.
 
 We offer an automated solution: `django` check
@@ -281,15 +304,15 @@
     # ...
 
     # Our custom check:
     'django_test_migrations.contrib.django_checks.AutoNames',
 ]
 ```
 
-And then in your CI run:
+Then in your CI run:
 
 ```bash
 python manage.py check --deploy
 ```
 
 This way you will be safe from wrong names in your migrations.
 
@@ -300,15 +323,15 @@
 
 DTM_IGNORED_MIGRATIONS = {
     ('main_app', '0004_auto_20191119_2125'),
     ('dependency_app', '0001_auto_20201110_2100'),
 }
 ```
 
-And we won't complain about them.
+Then we won't complain about them.
 
 Or you can completely ignore entire app:
 
 ```python
 # settings.py
 
 DTM_IGNORED_MIGRATIONS = {
```

### Comparing `django-test-migrations-1.2.0/django_test_migrations/checks/autonames.py` & `django_test_migrations-1.3.0/django_test_migrations/checks/autonames.py`

 * *Files identical despite different names*

### Comparing `django-test-migrations-1.2.0/django_test_migrations/contrib/django_checks.py` & `django_test_migrations-1.3.0/django_test_migrations/contrib/django_checks.py`

 * *Files identical despite different names*

### Comparing `django-test-migrations-1.2.0/django_test_migrations/contrib/pytest_plugin.py` & `django_test_migrations-1.3.0/django_test_migrations/contrib/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `django-test-migrations-1.2.0/django_test_migrations/contrib/unittest_case.py` & `django_test_migrations-1.3.0/django_test_migrations/contrib/unittest_case.py`

 * *Files identical despite different names*

### Comparing `django-test-migrations-1.2.0/django_test_migrations/db/backends/base/configuration.py` & `django_test_migrations-1.3.0/django_test_migrations/db/backends/base/configuration.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 
 class BaseDatabaseConfiguration(abc.ABC):
     """Interact with database's settings."""
 
     vendor: ClassVar[str]
     statement_timeout: ClassVar[str]
 
-    def __init__(self, connection: AnyConnection) -> None:
-        """Bind database ``connection`` used to retrieve settings values."""
-        self.connection = connection
-
     @classmethod
     def __init_subclass__(cls, **kwargs) -> None:
         """Register ``BaseDatabaseConfiguration`` subclass of db ``vendor``."""
         if not inspect.isabstract(cls):
             database_configuration_registry.setdefault(cls.vendor, cls)
 
+    def __init__(self, connection: AnyConnection) -> None:
+        """Bind database ``connection`` used to retrieve settings values."""
+        self.connection = connection
+
     @abc.abstractmethod
     def get_setting_value(self, name: str) -> DatabaseSettingValue:
         """Retrieve value of ``vendor`` database's ``name`` setting.
 
         Raises:
             DatabaseConfigurationSettingNotFound
```

### Comparing `django-test-migrations-1.2.0/django_test_migrations/db/backends/exceptions.py` & `django_test_migrations-1.3.0/django_test_migrations/db/backends/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-test-migrations-1.2.0/django_test_migrations/db/backends/mysql/configuration.py` & `django_test_migrations-1.3.0/django_test_migrations/db/backends/mysql/configuration.py`

 * *Files identical despite different names*

### Comparing `django-test-migrations-1.2.0/django_test_migrations/db/backends/postgresql/configuration.py` & `django_test_migrations-1.3.0/django_test_migrations/db/backends/postgresql/configuration.py`

 * *Files identical despite different names*

### Comparing `django-test-migrations-1.2.0/django_test_migrations/db/backends/registry.py` & `django_test_migrations-1.3.0/django_test_migrations/db/backends/registry.py`

 * *Files identical despite different names*

### Comparing `django-test-migrations-1.2.0/django_test_migrations/db/checks/statement_timeout.py` & `django_test_migrations-1.3.0/django_test_migrations/db/checks/statement_timeout.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from django.db import connections
 from typing_extensions import Final
 
 from django_test_migrations.db.backends import exceptions, registry
 from django_test_migrations.db.backends.base.configuration import (
     BaseDatabaseConfiguration,
 )
-from django_test_migrations.logic.datetime import timedelta_to_miliseconds
+from django_test_migrations.logic.datetime import timedelta_to_milliseconds
 from django_test_migrations.types import AnyConnection
 
 #: We use this value as a unique identifier of databases related check.
 CHECK_NAME: Final = 'django_test_migrations.checks.database_configuration'
 STATEMENT_TIMEOUT_MINUTES_UPPER_LIMIT: Final = 30
 
 
@@ -76,15 +76,15 @@
 
 
 def _ensure_statement_timeout_not_too_high(
     database_configuration: BaseDatabaseConfiguration,
     setting_value: int,
     messages: List[CheckMessage],
 ) -> None:
-    upper_limit = timedelta_to_miliseconds(
+    upper_limit = timedelta_to_milliseconds(
         datetime.timedelta(minutes=STATEMENT_TIMEOUT_MINUTES_UPPER_LIMIT),
     )
     if setting_value > upper_limit:
         messages.append(
             Warning(
                 (
                     '{0}: statement timeout "{1}" setting value - "{2} ms" ' +
```

### Comparing `django-test-migrations-1.2.0/django_test_migrations/migrator.py` & `django_test_migrations-1.3.0/django_test_migrations/migrator.py`

 * *Files identical despite different names*

### Comparing `django-test-migrations-1.2.0/django_test_migrations/plan.py` & `django_test_migrations-1.3.0/django_test_migrations/plan.py`

 * *Files identical despite different names*

### Comparing `django-test-migrations-1.2.0/django_test_migrations/signals.py` & `django_test_migrations-1.3.0/django_test_migrations/signals.py`

 * *Files identical despite different names*

### Comparing `django-test-migrations-1.2.0/django_test_migrations/types.py` & `django_test_migrations-1.3.0/django_test_migrations/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,12 @@
 from typing import List, Optional, Tuple, Union
 
-import django
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.migrations import Migration
-
-if django.VERSION < (3, 2):
-    from django.db import (  # noqa: WPS433
-        DefaultConnectionProxy as ConnectionProxy,
-    )
-else:
-    from django.utils.connection import ConnectionProxy  # noqa: WPS440, WPS433
+from django.utils.connection import ConnectionProxy
 
 # Migration target: (app_name, migration_name)
 # Regular or rollback migration: 0001 -> 0002, or 0002 -> 0001
 # Rollback migration to initial state: 0001 -> None
 MigrationTarget = Tuple[str, Optional[str]]
 MigrationSpec = Union[MigrationTarget, List[MigrationTarget]]
```

### Comparing `django-test-migrations-1.2.0/pyproject.toml` & `django_test_migrations-1.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,10 @@
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
-
-
-[tool.nitpick]
-style = "https://raw.githubusercontent.com/wemake-services/wemake-python-styleguide/master/styles/nitpick-style-wemake.toml"
-
-
 [tool.poetry]
 name = "django-test-migrations"
-version = "1.2.0"
+version = "1.3.0"
 description = "Test django schema and data migrations, including ordering"
 license = "MIT"
 
 authors = [
   "sobolevn <mail@sobolevn.me>"
 ]
 
@@ -39,36 +30,44 @@
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Internet :: WWW/HTTP",
   "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
   "Framework :: Django",
-  "Framework :: Django :: 1.11",
-  "Framework :: Django :: 2.2",
-  "Framework :: Django :: 3.0",
-  "Framework :: Django :: 3.1",
+  "Framework :: Django :: 3.2",
+  "Framework :: Django :: 4.0",
+  "Framework :: Django :: 4.1",
 ]
 
 [tool.poetry.plugins.pytest11]
 django_test_migrations = "django_test_migrations.contrib.pytest_plugin"
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.8"
 typing_extensions = ">=3.6,<5"
 
 [tool.poetry.dev-dependencies]
-django = "^3.2"
+django = "^4.2"
 
-mypy = "^0.910"
-wemake-python-styleguide = "^0.16"
-flake8-pytest-style = "^1.5"
-nitpick = "^0.29"
-
-safety = "^1.10"
-
-pytest = "^6.2"
-pytest-cov = "^3.0"
-pytest-randomly = "^3.10"
+mypy = "^1.2"
+wemake-python-styleguide = "^0.17"
+flake8-pytest-style = "^1.7"
+nitpick = "^0.33"
+
+safety = "^2.3"
+
+pytest = "^7.3"
+pytest-cov = "^4.0"
+pytest-randomly = "^3.12"
 pytest-django = "^4.5"
-pytest-pythonpath = "^0.7"
-pytest-mock = "^3.6"
+pytest-mock = "^3.10"
+
+
+[build-system]
+requires = ["poetry-core>=1.5.0"]
+build-backend = "poetry.core.masonry.api"
+
+
+[tool.nitpick]
+style = "https://raw.githubusercontent.com/wemake-services/wemake-python-styleguide/master/styles/nitpick-style-wemake.toml"
+
```

### Comparing `django-test-migrations-1.2.0/setup.py` & `django_test_migrations-1.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,411 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-test-migrations
+Version: 1.3.0
+Summary: Test django schema and data migrations, including ordering
+Home-page: https://github.com/wemake-services/django-test-migrations
+License: MIT
+Keywords: django,django-tests,django-migrations,django-orm,migrations,orm,sql,tests,test,pytest,pytest-plugin
+Author: sobolevn
+Author-email: mail@sobolevn.me
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: typing_extensions (>=3.6,<5)
+Project-URL: Repository, https://github.com/wemake-services/django-test-migrations
+Description-Content-Type: text/markdown
 
-packages = \
-['django_test_migrations',
- 'django_test_migrations.checks',
- 'django_test_migrations.contrib',
- 'django_test_migrations.db',
- 'django_test_migrations.db.backends',
- 'django_test_migrations.db.backends.base',
- 'django_test_migrations.db.backends.mysql',
- 'django_test_migrations.db.backends.postgresql',
- 'django_test_migrations.db.checks',
- 'django_test_migrations.logic']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['typing_extensions>=3.6,<5']
-
-entry_points = \
-{'pytest11': ['django_test_migrations = '
-              'django_test_migrations.contrib.pytest_plugin']}
-
-setup_kwargs = {
-    'name': 'django-test-migrations',
-    'version': '1.2.0',
-    'description': 'Test django schema and data migrations, including ordering',
-    'long_description': '# django-test-migrations\n\n[![wemake.services](https://img.shields.io/badge/%20-wemake.services-green.svg?label=%20&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAABGdBTUEAALGPC%2FxhBQAAAAFzUkdCAK7OHOkAAAAbUExURQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAP%2F%2F%2F5TvxDIAAAAIdFJOUwAjRA8xXANAL%2Bv0SAAAADNJREFUGNNjYCAIOJjRBdBFWMkVQeGzcHAwksJnAPPZGOGAASzPzAEHEGVsLExQwE7YswCb7AFZSF3bbAAAAABJRU5ErkJggg%3D%3D)](https://wemake.services)\n[![Build status](https://github.com/wemake-services/django-test-migrations/workflows/test/badge.svg?branch=master&event=push)](https://github.com/wemake-services/django-test-migrations/actions?query=workflow%3Atest)\n[![codecov](https://codecov.io/gh/wemake-services/django-test-migrations/branch/master/graph/badge.svg)](https://codecov.io/gh/wemake-services/django-test-migrations)\n[![Python Version](https://img.shields.io/pypi/pyversions/django-test-migrations.svg)](https://pypi.org/project/django-test-migrations/)\n![PyPI - Django Version](https://img.shields.io/pypi/djversions/django-test-migrations)\n[![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide)\n\n\n## Features\n\n- Allows to test `django` schema and data migrations\n- Allows to test both forward and rollback migrations\n- Allows to test the migrations order\n- Allows to test migration names\n- Allows to test database configuration\n- Fully typed with annotations and checked with `mypy`, [PEP561 compatible](https://www.python.org/dev/peps/pep-0561/)\n- Easy to start: has lots of docs, tests, and tutorials\n\nRead the [announcing post](https://sobolevn.me/2019/10/testing-django-migrations).\nSee real-world [usage example](https://github.com/wemake-services/wemake-django-template).\n\n\n## Installation\n\n```bash\npip install django-test-migrations\n```\n\nWe support several `django` versions:\n\n- `1.11`\n- `2.2`\n- `3.1`\n- `3.2`\n- `4.0`\n\nOther versions might work too, but they are not officially supported.\n\n\n## Testing django migrations\n\nTesting migrations is not a frequent thing in `django` land.\nBut, sometimes it is totally required. When?\n\nWhen we do complex schema or data changes\nand what to be sure that existing data won\'t be corrupted.\nWe might also want to be sure that all migrations can be safely rolled back.\nAnd as a final touch we want to be sure that migrations\nare in the correct order and have correct dependencies.\n\n### Testing forward migrations\n\nTo test all migrations we have a [`Migrator`](https://github.com/wemake-services/django-test-migrations/blob/master/django_test_migrations/migrator.py) class.\n\nIt has three methods to work with:\n\n- `.apply_initial_migration()` which takes app and migration names to generate\n  a state before the actual migration happens. It creates the `before state`\n  by applying all migrations up to and including the ones passed as an argument.\n\n- `.apply_tested_migration()` which takes app and migration names to perform the\n  actual migration\n\n- `.reset()` to clean everything up after we are done with testing\n\nSo, here\'s an example:\n\n```python\nfrom django_test_migrations.migrator import Migrator\n\nmigrator = Migrator(database=\'default\')\n\n# Initial migration, currently our model has only a single string field:\n# Note:\n# We are testing migration `0002_someitem_is_clean`, so we are specifying\n# the name of the previous migration (`0001_initial`) in the\n# .apply_initial_migration() method in order to prepare a state of the database\n# before applying the migration we are going to test.\n#\nold_state = migrator.apply_initial_migration((\'main_app\', \'0001_initial\'))\nSomeItem = old_state.apps.get_model(\'main_app\', \'SomeItem\')\n\n# Let\'s create a model with just a single field specified:\nSomeItem.objects.create(string_field=\'a\')\nassert len(SomeItem._meta.get_fields()) == 2  # id + string_field\n\n# Now this migration will add `is_clean` field to the model:\nnew_state = migrator.apply_tested_migration(\n    (\'main_app\', \'0002_someitem_is_clean\'),\n)\nSomeItem = new_state.apps.get_model(\'main_app\', \'SomeItem\')\n\n# We can now test how our migration worked, new field is there:\nassert SomeItem.objects.filter(is_clean=True).count() == 0\nassert len(SomeItem._meta.get_fields()) == 3  # id + string_field + is_clean\n\n# Cleanup:\nmigrator.reset()\n```\n\nThat was an example of a forward migration.\n\n### Backward migration\n\nThe thing is that you can also test backward migrations.\nNothing really changes except migration names that you pass and your logic:\n\n```python\nmigrator = Migrator()\n\n# Currently our model has two field, but we need a rollback:\nold_state = migrator.apply_initial_migration(\n    (\'main_app\', \'0002_someitem_is_clean\'),\n)\nSomeItem = old_state.apps.get_model(\'main_app\', \'SomeItem\')\n\n# Create some data to illustrate your cases:\n# ...\n\n# Now this migration will drop `is_clean` field:\nnew_state = migrator.apply_tested_migration((\'main_app\', \'0001_initial\'))\n\n# Assert the results:\n# ...\n\n# Cleanup:\nmigrator.reset()\n```\n\n### Testing migrations ordering\n\nSometimes we also want to be sure that our migrations are in the correct order.\nAnd all our `dependecies = [...]` are correct.\n\nTo achieve that we have [`plan.py`](https://github.com/wemake-services/django-test-migrations/blob/master/django_test_migrations/plan.py) module.\n\nThat\'s how it can be used:\n\n```python\nfrom django_test_migrations.plan import all_migrations, nodes_to_tuples\n\nmain_migrations = all_migrations(\'default\', [\'main_app\', \'other_app\'])\nassert nodes_to_tuples(main_migrations) == [\n    (\'main_app\', \'0001_initial\'),\n    (\'main_app\', \'0002_someitem_is_clean\'),\n    (\'other_app\', \'0001_initial\'),\n    (\'main_app\', \'0003_update_is_clean\'),\n    (\'main_app\', \'0004_auto_20191119_2125\'),\n    (\'other_app\', \'0002_auto_20191120_2230\'),\n]\n```\n\nThis way you can be sure that migrations\nand apps that depend on each other will be executed in the correct order.\n\n\n## Test framework integrations 🐍\n\nWe support several test frameworks as first-class citizens.\nThat\'s a testing tool after all!\n\nNote that the Django `post_migrate` signal\'s receiver list is cleared at\nthe start of tests and restored afterwards. If you need to test your\nown `post_migrate` signals then attach/remove them during a test.\n\n### pytest\n\nWe ship `django-test-migrations` with a `pytest` plugin\nthat provides two convinient fixtures:\n\n- `migrator_factory` that gives you an opportunity\n  to create `Migrator` classes for any database\n- `migrator` instance for the `\'default\'` database\n\nThat\'s how it can be used:\n\n```python\nimport pytest\n\n@pytest.mark.django_db()\ndef test_pytest_plugin_initial(migrator):\n    """Ensures that the initial migration works."""\n    old_state = migrator.apply_initial_migration((\'main_app\', None))\n\n    with pytest.raises(LookupError):\n        # Models does not yet exist:\n        old_state.apps.get_model(\'main_app\', \'SomeItem\')\n\n    new_state = migrator.apply_tested_migration((\'main_app\', \'0001_initial\'))\n    # After the initial migration is done, we can use the model state:\n    SomeItem = new_state.apps.get_model(\'main_app\', \'SomeItem\')\n    assert SomeItem.objects.filter(string_field=\'\').count() == 0\n```\n\n### unittest\n\nWe also ship an integration with the built-in `unittest` framework.\n\nHere\'s how it can be used:\n\n```python\nfrom django_test_migrations.contrib.unittest_case import MigratorTestCase\n\nclass TestDirectMigration(MigratorTestCase):\n    """This class is used to test direct migrations."""\n\n    migrate_from = (\'main_app\', \'0002_someitem_is_clean\')\n    migrate_to = (\'main_app\', \'0003_update_is_clean\')\n\n    def prepare(self):\n        """Prepare some data before the migration."""\n        SomeItem = self.old_state.apps.get_model(\'main_app\', \'SomeItem\')\n        SomeItem.objects.create(string_field=\'a\')\n        SomeItem.objects.create(string_field=\'a b\')\n\n    def test_migration_main0003(self):\n        """Run the test itself."""\n        SomeItem = self.new_state.apps.get_model(\'main_app\', \'SomeItem\')\n\n        assert SomeItem.objects.count() == 2\n        assert SomeItem.objects.filter(is_clean=True).count() == 1\n```\n\n### Choosing only migrations tests\n\nIn CI systems it is important to get instant feedback. Running tests that\napply database migration can slow down tests execution, so it is often a good\nidea to run standard, fast, regular unit tests without migrations in parallel\nwith slower migrations tests.\n\n#### pytest\n\n`django_test_migrations` adds `migration_test` marker to each test using\n`migrator_factory` or `migrator` fixture.\nTo run only migrations test, use `-m` option:\n\n```bash\npytest -m migration_test  # runs only migraion tests\npytest -m "not migration_test"  # runs all except migraion tests\n```\n\n#### unittest\n\n`django_test_migrations` adds `migration_test`\n[tag](https://docs.djangoproject.com/en/3.0/topics/testing/tools/#tagging-tests)\nto every `MigratorTestCase` subclass.\nTo run only migrations tests, use `--tag` option:\n\n```bash\npython mange.py test --tag=migration_test  # runs only migraion tests\npython mange.py test --exclude-tag=migration_test  # runs all except migraion tests\n```\n\n\n## Django Checks\n\n`django_test_migrations` comes with 2 groups of Django\'s checks for:\n\n+ detecting migrations scripts automatically generated names\n+ validating some subset of database settings\n\n### Testing migration names\n\n`django` generates migration names for you when you run `makemigrations`.\nAnd these names are bad ([read more](https://adamj.eu/tech/2020/02/24/how-to-disallow-auto-named-django-migrations/) about why it is bad)!\nJust look at this: `0004_auto_20191119_2125.py`\n\nWhat does this migration do? What changes does it have?\n\nOne can also pass `--name` attribute when creating migrations, but it is easy to forget.\n\nWe offer an automated solution: `django` check\nthat produces an error for each badly named migration.\n\nAdd our check into your `INSTALLED_APPS`:\n\n```python\nINSTALLED_APPS = [\n    # ...\n\n    # Our custom check:\n    \'django_test_migrations.contrib.django_checks.AutoNames\',\n]\n```\n\nAnd then in your CI run:\n\n```bash\npython manage.py check --deploy\n```\n\nThis way you will be safe from wrong names in your migrations.\n\nDo you have a migrations that cannot be renamed? Add them to the ignore list:\n\n```python\n# settings.py\n\nDTM_IGNORED_MIGRATIONS = {\n    (\'main_app\', \'0004_auto_20191119_2125\'),\n    (\'dependency_app\', \'0001_auto_20201110_2100\'),\n}\n```\n\nAnd we won\'t complain about them.\n\nOr you can completely ignore entire app:\n\n```python\n# settings.py\n\nDTM_IGNORED_MIGRATIONS = {\n    (\'dependency_app\', \'*\'),\n    (\'another_dependency_app\', \'*\'),\n}\n```\n\n### Database configuration\n\nAdd our check to `INSTALLED_APPS`:\n\n```python\nINSTALLED_APPS = [\n    # ...\n\n    # Our custom check:\n    \'django_test_migrations.contrib.django_checks.DatabaseConfiguration\',\n]\n```\n\nThen just run `check` management command in your CI like listed in section\nabove.\n\n\n## Related projects\n\nYou might also like:\n\n- [django-migration-linter](https://github.com/3YOURMIND/django-migration-linter) - Detect backward incompatible migrations for your django project.\n- [wemake-django-template](https://github.com/wemake-services/wemake-django-template/) - Bleeding edge django template focused on code quality and security with both `django-test-migrations` and `django-migration-linter` on board.\n\n\n## Credits\n\nThis project is based on work of other awesome people:\n\n- [@asfaltboy](https://gist.github.com/asfaltboy/b3e6f9b5d95af8ba2cc46f2ba6eae5e2)\n- [@blueyed](https://gist.github.com/blueyed/4fb0a807104551f103e6)\n- [@fernandogrd](https://gist.github.com/blueyed/4fb0a807104551f103e6#gistcomment-1546191)\n- [@adamchainz](https://adamj.eu/tech/2020/02/24/how-to-disallow-auto-named-django-migrations/)\n\n\n## License\n\nMIT.\n',
-    'author': 'sobolevn',
-    'author_email': 'mail@sobolevn.me',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/wemake-services/django-test-migrations',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.6,<4.0',
+# django-test-migrations
+
+[![wemake.services](https://img.shields.io/badge/%20-wemake.services-green.svg?label=%20&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAABGdBTUEAALGPC%2FxhBQAAAAFzUkdCAK7OHOkAAAAbUExURQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAP%2F%2F%2F5TvxDIAAAAIdFJOUwAjRA8xXANAL%2Bv0SAAAADNJREFUGNNjYCAIOJjRBdBFWMkVQeGzcHAwksJnAPPZGOGAASzPzAEHEGVsLExQwE7YswCb7AFZSF3bbAAAAABJRU5ErkJggg%3D%3D)](https://wemake-services.github.io)
+[![Build status](https://github.com/wemake-services/django-test-migrations/workflows/test/badge.svg?branch=master&event=push)](https://github.com/wemake-services/django-test-migrations/actions?query=workflow%3Atest)
+[![codecov](https://codecov.io/gh/wemake-services/django-test-migrations/branch/master/graph/badge.svg)](https://codecov.io/gh/wemake-services/django-test-migrations)
+[![Python Version](https://img.shields.io/pypi/pyversions/django-test-migrations.svg)](https://pypi.org/project/django-test-migrations/)
+![PyPI - Django Version](https://img.shields.io/pypi/djversions/django-test-migrations)
+[![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide)
+
+
+## Features
+
+- Allows to test `django` schema and data migrations
+- Allows to test both forward and rollback migrations
+- Allows to test the migrations order
+- Allows to test migration names
+- Allows to test database configuration
+- Fully typed with annotations and checked with `mypy`, [PEP561 compatible](https://www.python.org/dev/peps/pep-0561/)
+- Easy to start: has lots of docs, tests, and tutorials
+
+Read the [announcing post](https://sobolevn.me/2019/10/testing-django-migrations).
+See real-world [usage example](https://github.com/wemake-services/wemake-django-template).
+
+
+## Installation
+
+```bash
+pip install django-test-migrations
+```
+
+We support several `django` versions:
+
+- `2.2`
+- `3.2`
+- `4.0`
+- `4.1`
+- `4.2`
+
+Other versions most likely will work too,
+but they are not officially supported.
+
+
+## Testing Django migrations
+
+Testing migrations is not a frequent thing in `django` land.
+But, sometimes it is totally required. When?
+
+When we do complex schema or data changes
+and what to be sure that existing data won't be corrupted.
+We might also want to be sure that all migrations can be safely rolled back.
+And as a final touch, we want to be sure that migrations
+are in the correct order and have correct dependencies.
+
+### Testing forward migrations
+
+To test all migrations we have a [`Migrator`](https://github.com/wemake-services/django-test-migrations/blob/master/django_test_migrations/migrator.py) class.
+
+It has three methods to work with:
+
+- `.apply_initial_migration()` which takes app and migration names to generate
+  a state before the actual migration happens. It creates the `before state`
+  by applying all migrations up to and including the ones passed as an argument.
+
+- `.apply_tested_migration()` which takes app and migration names to perform the
+  actual migration
+
+- `.reset()` to clean everything up after we are done with testing
+
+So, here's an example:
+
+```python
+from django_test_migrations.migrator import Migrator
+
+migrator = Migrator(database='default')
+
+# Initial migration, currently our model has only a single string field:
+# Note:
+# We are testing migration `0002_someitem_is_clean`, so we are specifying
+# the name of the previous migration (`0001_initial`) in the
+# .apply_initial_migration() method in order to prepare a state of the database
+# before applying the migration we are going to test.
+#
+old_state = migrator.apply_initial_migration(('main_app', '0001_initial'))
+SomeItem = old_state.apps.get_model('main_app', 'SomeItem')
+
+# Let's create a model with just a single field specified:
+SomeItem.objects.create(string_field='a')
+assert len(SomeItem._meta.get_fields()) == 2  # id + string_field
+
+# Now this migration will add `is_clean` field to the model:
+new_state = migrator.apply_tested_migration(
+    ('main_app', '0002_someitem_is_clean'),
+)
+SomeItem = new_state.apps.get_model('main_app', 'SomeItem')
+
+# We can now test how our migration worked, new field is there:
+assert SomeItem.objects.filter(is_clean=True).count() == 0
+assert len(SomeItem._meta.get_fields()) == 3  # id + string_field + is_clean
+
+# Cleanup:
+migrator.reset()
+```
+
+That was an example of a forward migration.
+
+### Backward migration
+
+The thing is that you can also test backward migrations.
+Nothing really changes except migration names that you pass and your logic:
+
+```python
+migrator = Migrator()
+
+# Currently our model has two field, but we need a rollback:
+old_state = migrator.apply_initial_migration(
+    ('main_app', '0002_someitem_is_clean'),
+)
+SomeItem = old_state.apps.get_model('main_app', 'SomeItem')
+
+# Create some data to illustrate your cases:
+# ...
+
+# Now this migration will drop `is_clean` field:
+new_state = migrator.apply_tested_migration(('main_app', '0001_initial'))
+
+# Assert the results:
+# ...
+
+# Cleanup:
+migrator.reset()
+```
+
+### Testing migrations ordering
+
+Sometimes we also want to be sure that our migrations are in the correct order
+and that all our `dependencies = [...]` are correct.
+
+To achieve that we have [`plan.py`](https://github.com/wemake-services/django-test-migrations/blob/master/django_test_migrations/plan.py) module.
+
+That's how it can be used:
+
+```python
+from django_test_migrations.plan import all_migrations, nodes_to_tuples
+
+main_migrations = all_migrations('default', ['main_app', 'other_app'])
+assert nodes_to_tuples(main_migrations) == [
+    ('main_app', '0001_initial'),
+    ('main_app', '0002_someitem_is_clean'),
+    ('other_app', '0001_initial'),
+    ('main_app', '0003_update_is_clean'),
+    ('main_app', '0004_auto_20191119_2125'),
+    ('other_app', '0002_auto_20191120_2230'),
+]
+```
+
+This way you can be sure that migrations
+and apps that depend on each other will be executed in the correct order.
+
+### `factory_boy` integration
+
+If you use factories to create models, you can replace their respective
+`.build()` or `.create()` calls with methods of `factory` and pass the
+model name and factory class as arguments:
+
+```python
+import factory
+
+old_state = migrator.apply_initial_migration(
+    ('main_app', '0002_someitem_is_clean'),
+)
+SomeItem = old_state.apps.get_model('main_app', 'SomeItem')
+
+# instead of
+# item = SomeItemFactory.create()
+# use this:
+factory.create(SomeItem, FACTORY_CLASS=SomeItemFactory)
+
+# ...
+```
+
+
+## Test framework integrations 🐍
+
+We support several test frameworks as first-class citizens.
+That's a testing tool after all!
+
+Note that the Django `post_migrate` signal's receiver list is cleared at
+the start of tests and restored afterwards. If you need to test your
+own `post_migrate` signals then attach/remove them during a test.
+
+### pytest
+
+We ship `django-test-migrations` with a `pytest` plugin
+that provides two convenient fixtures:
+
+- `migrator_factory` that gives you an opportunity
+  to create `Migrator` classes for any database
+- `migrator` instance for the `'default'` database
+
+That's how it can be used:
+
+```python
+import pytest
+
+@pytest.mark.django_db()
+def test_pytest_plugin_initial(migrator):
+    """Ensures that the initial migration works."""
+    old_state = migrator.apply_initial_migration(('main_app', None))
+
+    with pytest.raises(LookupError):
+        # Model does not yet exist:
+        old_state.apps.get_model('main_app', 'SomeItem')
+
+    new_state = migrator.apply_tested_migration(('main_app', '0001_initial'))
+    # After the initial migration is done, we can use the model state:
+    SomeItem = new_state.apps.get_model('main_app', 'SomeItem')
+    assert SomeItem.objects.filter(string_field='').count() == 0
+```
+
+### unittest
+
+We also ship an integration with the built-in `unittest` framework.
+
+Here's how it can be used:
+
+```python
+from django_test_migrations.contrib.unittest_case import MigratorTestCase
+
+class TestDirectMigration(MigratorTestCase):
+    """This class is used to test direct migrations."""
+
+    migrate_from = ('main_app', '0002_someitem_is_clean')
+    migrate_to = ('main_app', '0003_update_is_clean')
+
+    def prepare(self):
+        """Prepare some data before the migration."""
+        SomeItem = self.old_state.apps.get_model('main_app', 'SomeItem')
+        SomeItem.objects.create(string_field='a')
+        SomeItem.objects.create(string_field='a b')
+
+    def test_migration_main0003(self):
+        """Run the test itself."""
+        SomeItem = self.new_state.apps.get_model('main_app', 'SomeItem')
+
+        assert SomeItem.objects.count() == 2
+        assert SomeItem.objects.filter(is_clean=True).count() == 1
+```
+
+### Choosing only migrations tests
+
+In CI systems it is important to get instant feedback. Running tests that
+apply database migration can slow down tests execution, so it is often a good
+idea to run standard, fast, regular unit tests without migrations in parallel
+with slower migrations tests.
+
+#### pytest
+
+`django_test_migrations` adds `migration_test` marker to each test using
+`migrator_factory` or `migrator` fixture.
+To run only migrations test, use `-m` option:
+
+```bash
+pytest -m migration_test  # Runs only migration tests
+pytest -m "not migration_test"  # Runs all except migration tests
+```
+
+#### unittest
+
+`django_test_migrations` adds `migration_test`
+[tag](https://docs.djangoproject.com/en/3.0/topics/testing/tools/#tagging-tests)
+to every `MigratorTestCase` subclass.
+To run only migrations tests, use `--tag` option:
+
+```bash
+python mange.py test --tag=migration_test  # Runs only migration tests
+python mange.py test --exclude-tag=migration_test  # Runs all except migration tests
+```
+
+
+## Django Checks
+
+`django_test_migrations` comes with 2 groups of Django's checks for:
+
++ detecting migrations scripts automatically generated names
++ validating some subset of database settings
+
+### Testing migration names
+
+`django` generates migration names for you when you run `makemigrations`.
+These names are bad ([read more](https://adamj.eu/tech/2020/02/24/how-to-disallow-auto-named-django-migrations/) about why it is bad)!
+Just look at this: `0004_auto_20191119_2125.py`
+
+What does this migration do? What changes does it have?
+
+One can also pass `--name` attribute when creating migrations, but it is easy to forget.
+
+We offer an automated solution: `django` check
+that produces an error for each badly named migration.
+
+Add our check into your `INSTALLED_APPS`:
+
+```python
+INSTALLED_APPS = [
+    # ...
+
+    # Our custom check:
+    'django_test_migrations.contrib.django_checks.AutoNames',
+]
+```
+
+Then in your CI run:
+
+```bash
+python manage.py check --deploy
+```
+
+This way you will be safe from wrong names in your migrations.
+
+Do you have a migrations that cannot be renamed? Add them to the ignore list:
+
+```python
+# settings.py
+
+DTM_IGNORED_MIGRATIONS = {
+    ('main_app', '0004_auto_20191119_2125'),
+    ('dependency_app', '0001_auto_20201110_2100'),
 }
+```
+
+Then we won't complain about them.
+
+Or you can completely ignore entire app:
+
+```python
+# settings.py
+
+DTM_IGNORED_MIGRATIONS = {
+    ('dependency_app', '*'),
+    ('another_dependency_app', '*'),
+}
+```
+
+### Database configuration
+
+Add our check to `INSTALLED_APPS`:
+
+```python
+INSTALLED_APPS = [
+    # ...
+
+    # Our custom check:
+    'django_test_migrations.contrib.django_checks.DatabaseConfiguration',
+]
+```
+
+Then just run `check` management command in your CI like listed in section
+above.
+
+
+## Related projects
+
+You might also like:
+
+- [django-migration-linter](https://github.com/3YOURMIND/django-migration-linter) - Detect backward incompatible migrations for your django project.
+- [wemake-django-template](https://github.com/wemake-services/wemake-django-template/) - Bleeding edge django template focused on code quality and security with both `django-test-migrations` and `django-migration-linter` on board.
+
+
+## Credits
+
+This project is based on work of other awesome people:
+
+- [@asfaltboy](https://gist.github.com/asfaltboy/b3e6f9b5d95af8ba2cc46f2ba6eae5e2)
+- [@blueyed](https://gist.github.com/blueyed/4fb0a807104551f103e6)
+- [@fernandogrd](https://gist.github.com/blueyed/4fb0a807104551f103e6#gistcomment-1546191)
+- [@adamchainz](https://adamj.eu/tech/2020/02/24/how-to-disallow-auto-named-django-migrations/)
+
+
+## License
 
+MIT.
 
-setup(**setup_kwargs)
```

