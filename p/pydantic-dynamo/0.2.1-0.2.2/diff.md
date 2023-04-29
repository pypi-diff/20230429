# Comparing `tmp/pydantic_dynamo-0.2.1.tar.gz` & `tmp/pydantic_dynamo-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_dynamo-0.2.1.tar", max compression
+gzip compressed data, was "pydantic_dynamo-0.2.2.tar", max compression
```

## Comparing `pydantic_dynamo-0.2.1.tar` & `pydantic_dynamo-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1121 2023-03-07 03:45:50.202681 pydantic_dynamo-0.2.1/LICENSE
--rw-r--r--   0        0        0        0 2023-03-07 03:36:36.814175 pydantic_dynamo-0.2.1/pydantic_dynamo/__init__.py
--rw-r--r--   0        0        0      243 2023-04-04 19:40:26.272160 pydantic_dynamo-0.2.1/pydantic_dynamo/constants.py
--rw-r--r--   0        0        0       53 2023-03-07 03:09:09.986643 pydantic_dynamo-0.2.1/pydantic_dynamo/exceptions.py
--rw-r--r--   0        0        0     3294 2023-04-19 02:51:16.873917 pydantic_dynamo-0.2.1/pydantic_dynamo/models.py
--rw-r--r--   0        0        0    14586 2023-04-13 17:24:33.661892 pydantic_dynamo-0.2.1/pydantic_dynamo/repository.py
--rw-r--r--   0        0        0    10579 2023-04-19 02:51:16.873917 pydantic_dynamo-0.2.1/pydantic_dynamo/utils.py
--rw-r--r--   0        0        0        0 2023-04-04 19:23:43.683503 pydantic_dynamo-0.2.1/pydantic_dynamo/v2/__init__.py
--rw-r--r--   0        0        0     4355 2023-04-23 13:36:23.098647 pydantic_dynamo-0.2.1/pydantic_dynamo/v2/models.py
--rw-r--r--   0        0        0    16611 2023-04-23 13:30:24.492470 pydantic_dynamo-0.2.1/pydantic_dynamo/v2/repository.py
--rw-r--r--   0        0        0     3781 2023-04-23 13:31:55.765230 pydantic_dynamo-0.2.1/pydantic_dynamo/v2/sync_repository.py
--rw-r--r--   0        0        0     1190 2023-04-23 13:42:21.894819 pydantic_dynamo-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    15243 2023-04-20 16:42:35.339053 pydantic_dynamo-0.2.1/README.md
--rw-r--r--   0        0        0    15448 1970-01-01 00:00:00.000000 pydantic_dynamo-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1121 2023-03-07 03:45:50.202681 pydantic_dynamo-0.2.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-03-07 03:36:36.814175 pydantic_dynamo-0.2.2/pydantic_dynamo/__init__.py
+-rw-r--r--   0        0        0      243 2023-04-04 19:40:26.272160 pydantic_dynamo-0.2.2/pydantic_dynamo/constants.py
+-rw-r--r--   0        0        0       53 2023-03-07 03:09:09.986643 pydantic_dynamo-0.2.2/pydantic_dynamo/exceptions.py
+-rw-r--r--   0        0        0     3294 2023-04-19 02:51:16.873917 pydantic_dynamo-0.2.2/pydantic_dynamo/models.py
+-rw-r--r--   0        0        0    14586 2023-04-13 17:24:33.661892 pydantic_dynamo-0.2.2/pydantic_dynamo/repository.py
+-rw-r--r--   0        0        0    10579 2023-04-19 02:51:16.873917 pydantic_dynamo-0.2.2/pydantic_dynamo/utils.py
+-rw-r--r--   0        0        0        0 2023-04-04 19:23:43.683503 pydantic_dynamo-0.2.2/pydantic_dynamo/v2/__init__.py
+-rw-r--r--   0        0        0     4403 2023-04-29 12:58:54.202235 pydantic_dynamo-0.2.2/pydantic_dynamo/v2/models.py
+-rw-r--r--   0        0        0    17272 2023-04-29 12:59:41.536221 pydantic_dynamo-0.2.2/pydantic_dynamo/v2/repository.py
+-rw-r--r--   0        0        0     3805 2023-04-29 13:00:04.168642 pydantic_dynamo-0.2.2/pydantic_dynamo/v2/sync_repository.py
+-rw-r--r--   0        0        0     1260 2023-04-29 12:57:04.660325 pydantic_dynamo-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    16867 2023-04-29 12:57:04.658325 pydantic_dynamo-0.2.2/README.md
+-rw-r--r--   0        0        0    17035 1970-01-01 00:00:00.000000 pydantic_dynamo-0.2.2/PKG-INFO
```

### Comparing `pydantic_dynamo-0.2.1/LICENSE` & `pydantic_dynamo-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_dynamo-0.2.1/pydantic_dynamo/models.py` & `pydantic_dynamo-0.2.2/pydantic_dynamo/models.py`

 * *Files identical despite different names*

### Comparing `pydantic_dynamo-0.2.1/pydantic_dynamo/repository.py` & `pydantic_dynamo-0.2.2/pydantic_dynamo/repository.py`

 * *Files identical despite different names*

### Comparing `pydantic_dynamo-0.2.1/pydantic_dynamo/utils.py` & `pydantic_dynamo-0.2.2/pydantic_dynamo/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_dynamo-0.2.1/pydantic_dynamo/v2/models.py` & `pydantic_dynamo-0.2.2/pydantic_dynamo/v2/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,45 +23,45 @@
     contents: Iterable[PartitionedContent[ObjT]]
 
 
 class ReadOnlyAbstractRepository(AbstractAsyncContextManager, Generic[ObjT]):
     @abstractmethod
     async def get(
         self, partition_id: Optional[Sequence[str]], content_id: Optional[Sequence[str]]
-    ) -> GetResponse:
+    ) -> GetResponse[ObjT]:
         pass
 
     @abstractmethod
     def get_batch(
         self,
         request_ids: Sequence[Tuple[Optional[Sequence[str]], Optional[Sequence[str]]]],
-    ) -> AsyncIterator[BatchResponse]:
+    ) -> AsyncIterator[BatchResponse[ObjT]]:
         pass
 
     @abstractmethod
     def list(
         self,
         partition_id: Optional[Sequence[str]],
         content_prefix: Optional[Sequence[str]],
         sort_ascending: bool = True,
         limit: Optional[int] = None,
         filters: Optional[FilterCommand] = None,
-    ) -> AsyncIterator[BatchResponse]:
+    ) -> AsyncIterator[BatchResponse[ObjT]]:
         pass
 
     @abstractmethod
     def list_between(
         self,
         partition_id: Optional[Sequence[str]],
         content_start: Optional[Sequence[str]],
         content_end: Optional[Sequence[str]],
         sort_ascending: bool = True,
         limit: Optional[int] = None,
         filters: Optional[FilterCommand] = None,
-    ) -> AsyncIterator[BatchResponse]:
+    ) -> AsyncIterator[BatchResponse[ObjT]]:
         pass
 
 
 class AbstractRepository(ReadOnlyAbstractRepository[ObjT]):
     @abstractmethod
     async def put(self, content: PartitionedContent[ObjT]) -> None:
         pass
@@ -89,45 +89,45 @@
         pass
 
 
 class SyncReadOnlyAbstractRepository(AbstractContextManager, Generic[ObjT]):
     @abstractmethod
     def get(
         self, partition_id: Optional[Sequence[str]], content_id: Optional[Sequence[str]]
-    ) -> GetResponse:
+    ) -> GetResponse[ObjT]:
         pass
 
     @abstractmethod
     def get_batch(
         self,
         request_ids: Sequence[Tuple[Optional[Sequence[str]], Optional[Sequence[str]]]],
-    ) -> Iterator[BatchResponse]:
+    ) -> Iterator[BatchResponse[ObjT]]:
         pass
 
     @abstractmethod
     def list(
         self,
         partition_id: Optional[Sequence[str]],
         content_prefix: Optional[Sequence[str]],
         sort_ascending: bool = True,
         limit: Optional[int] = None,
         filters: Optional[FilterCommand] = None,
-    ) -> Iterator[BatchResponse]:
+    ) -> Iterator[BatchResponse[ObjT]]:
         pass
 
     @abstractmethod
     def list_between(
         self,
         partition_id: Optional[Sequence[str]],
         content_start: Optional[Sequence[str]],
         content_end: Optional[Sequence[str]],
         sort_ascending: bool = True,
         limit: Optional[int] = None,
         filters: Optional[FilterCommand] = None,
-    ) -> Iterator[BatchResponse]:
+    ) -> Iterator[BatchResponse[ObjT]]:
         pass
 
 
 class SyncAbstractRepository(SyncReadOnlyAbstractRepository[ObjT]):
     @abstractmethod
     def put(self, content: PartitionedContent[ObjT]) -> None:
         pass
```

### Comparing `pydantic_dynamo-0.2.1/pydantic_dynamo/v2/repository.py` & `pydantic_dynamo-0.2.2/pydantic_dynamo/v2/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         partition_name: str,
         content_type: str,
         table_name: str,
         partition_key: str,
         sort_key: str,
         table,
         resource,
+        consistent_reads: bool = False,
     ):
         """
 
         :param item_class: pydantic model class reference representing a single
             database record. This should match ObjT
         :param partition_prefix: first part of the concatenated value used in the
             partition key value.
@@ -70,25 +71,28 @@
         :param table_name: the region-specific name of the DynamoDB table
         :param partition_key: the name of the attribute defined as the table's partition key
         :param sort_key: the name of the attribute defined as the table's sort key
         :param table: instance of the Table service object
             from `await resource.Table(table_name)`
         :param resource: instance of the resource service object
             from `async with aioboto3.session.Session().resource(**kwargs)`
+        :param consistent_reads: boolean to determine if read operations should be performed
+            with strong consistency. Default is False and uses eventual consistency
         """
         self._item_class = item_class
         self._item_schema = self._item_class.schema()
         self._partition_prefix = partition_prefix
         self._partition_name = partition_name
         self._content_type = content_type
         self._table_name = table_name
         self._partition_key = partition_key
         self._sort_key = sort_key
         self._table = table
         self._resource = resource
+        self._consistent_reads = consistent_reads
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         pass
 
     @property
     def context(self) -> Dict[str, str]:
         return {
@@ -147,44 +151,45 @@
         if require_exists:
             build_kwargs["key"] = key
         args = build_update_args_for_command(**build_kwargs)  # type: ignore
         await execute_update_item(self._table, key, args)
 
     async def get(
         self, partition_id: Optional[Sequence[str]], content_id: Optional[Sequence[str]]
-    ) -> GetResponse:
+    ) -> GetResponse[ObjT]:
         if partition_id is None:
             partition_id = EMPTY_LIST
         if content_id is None:
             content_id = EMPTY_LIST
         log_context = {
             "partition_id": partition_id,
             "content_id": content_id,
             **self.context,
         }
         logger.info("Getting item from table by key", extra=log_context)
         response = await self._table.get_item(
             Key={
                 self._partition_key: self._partition_id(partition_id),
                 self._sort_key: self._content_id(content_id),
-            }
+            },
+            ConsistentRead=self._consistent_reads,
         )
         db_item = response.get("Item")
         if db_item:
             logger.info("Found item from table by key", extra=log_context)
             content = self._db_item_to_object(db_item)
         else:
             logger.info("No item found in table by key", extra=log_context)
             content = None
         return GetResponse(content=content)
 
     async def get_batch(
         self,
         request_ids: Sequence[Tuple[Optional[Sequence[str]], Optional[Sequence[str]]]],
-    ) -> AsyncIterator[BatchResponse]:
+    ) -> AsyncIterator[BatchResponse[ObjT]]:
         batch_number = 0
         for request_id_batch in chunks(request_ids, size=100):
             batch_number += 1
             logger.info(
                 "Starting batch get items request",
                 extra={
                     "batch_number": batch_number,
@@ -195,15 +200,17 @@
                 {
                     self._partition_key: self._partition_id(partition_id),
                     self._sort_key: self._content_id(content_id),
                 }
                 for partition_id, content_id in request_id_batch
             ]
             batch_response = await self._resource.batch_get_item(
-                RequestItems={self._table_name: {"Keys": batch_keys}}
+                RequestItems={
+                    self._table_name: {"Keys": batch_keys, "ConsistentRead": self._consistent_reads}
+                }
             )
             yield BatchResponse(
                 contents=(
                     self._db_item_to_object(db_item)
                     for db_item in batch_response["Responses"].get(self._table_name, [])
                 )
             )
@@ -212,15 +219,20 @@
                     "Getting unprocessed keys",
                     extra={
                         "batch_number": batch_number,
                         "batch_size": len(unprocessed_keys),
                     },
                 )
                 batch_response = await self._resource.batch_get_item(
-                    RequestItems={self._table_name: {"Keys": unprocessed_keys}}
+                    RequestItems={
+                        self._table_name: {
+                            "Keys": unprocessed_keys,
+                            "ConsistentRead": self._consistent_reads,
+                        }
+                    }
                 )
                 yield BatchResponse(
                     contents=(
                         self._db_item_to_object(db_item)
                         for db_item in batch_response["Responses"].get(self._table_name, [])
                     )
                 )
@@ -228,15 +240,15 @@
     async def list(
         self,
         partition_id: Optional[Sequence[str]],
         content_prefix: Optional[Sequence[str]],
         sort_ascending: bool = True,
         limit: Optional[int] = None,
         filters: Optional[FilterCommand] = None,
-    ) -> AsyncIterator[BatchResponse]:
+    ) -> AsyncIterator[BatchResponse[ObjT]]:
         if partition_id is None:
             partition_id = EMPTY_LIST
         if content_prefix is None:
             content_prefix = EMPTY_LIST
 
         condition = Key(self._partition_key).eq(self._partition_id(partition_id)) & Key(
             self._sort_key
@@ -253,15 +265,15 @@
         self,
         partition_id: Optional[Sequence[str]],
         content_start: Optional[Sequence[str]],
         content_end: Optional[Sequence[str]],
         sort_ascending: bool = True,
         limit: Optional[int] = None,
         filters: Optional[FilterCommand] = None,
-    ) -> AsyncIterator[BatchResponse]:
+    ) -> AsyncIterator[BatchResponse[ObjT]]:
         log_context = {
             "partition_id": partition_id,
             "content_start": content_start,
             "content_end": content_end,
             **self.context,
         }
         if partition_id is None:
@@ -373,14 +385,15 @@
         limit: Optional[int] = None,
         filters: Optional[FilterCommand] = None,
         select_fields: Optional[Sequence[str]] = None,
     ) -> AsyncGenerator[List[Dict], None]:
         query_kwargs = {
             "KeyConditionExpression": key_condition_expression,
             "ScanIndexForward": sort_ascending,
+            "ConsistentRead": self._consistent_reads,
         }
         if filters:
             validate_filters_for_schema(self._item_schema, filters)
             if filter_expression := build_filter_expression(filters):
                 query_kwargs[FILTER_EXPRESSION] = filter_expression
         if limit and FILTER_EXPRESSION not in query_kwargs:
             query_kwargs["Limit"] = limit
```

### Comparing `pydantic_dynamo-0.2.1/pydantic_dynamo/v2/sync_repository.py` & `pydantic_dynamo-0.2.2/pydantic_dynamo/v2/sync_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,47 +45,47 @@
         self, partition_id: Optional[Sequence[str]], content_prefix: Optional[Sequence[str]]
     ) -> None:
         loop = asyncio.get_event_loop()
         loop.run_until_complete(self._async_repo.delete(partition_id, content_prefix))
 
     def get(
         self, partition_id: Optional[Sequence[str]], content_id: Optional[Sequence[str]]
-    ) -> GetResponse:
+    ) -> GetResponse[ObjT]:
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(self._async_repo.get(partition_id, content_id))
 
     def get_batch(
         self, request_ids: Sequence[Tuple[Optional[Sequence[str]], Optional[Sequence[str]]]]
-    ) -> Iterator[BatchResponse]:
+    ) -> Iterator[BatchResponse[ObjT]]:
         loop = asyncio.get_event_loop()
         return iter_over_async(self._async_repo.get_batch(request_ids), loop)
 
     def list(
         self,
         partition_id: Optional[Sequence[str]],
         content_prefix: Optional[Sequence[str]],
         sort_ascending: bool = True,
         limit: Optional[int] = None,
         filters: Optional[FilterCommand] = None,
-    ) -> Iterator[BatchResponse]:
+    ) -> Iterator[BatchResponse[ObjT]]:
         loop = asyncio.get_event_loop()
         return iter_over_async(
             self._async_repo.list(partition_id, content_prefix, sort_ascending, limit, filters),
             loop,
         )
 
     def list_between(
         self,
         partition_id: Optional[Sequence[str]],
         content_start: Optional[Sequence[str]],
         content_end: Optional[Sequence[str]],
         sort_ascending: bool = True,
         limit: Optional[int] = None,
         filters: Optional[FilterCommand] = None,
-    ) -> Iterator[BatchResponse]:
+    ) -> Iterator[BatchResponse[ObjT]]:
         loop = asyncio.get_event_loop()
         return iter_over_async(
             self._async_repo.list_between(
                 partition_id, content_start, content_end, sort_ascending, limit, filters
             ),
             loop,
         )
```

### Comparing `pydantic_dynamo-0.2.1/pyproject.toml` & `pydantic_dynamo-0.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-dynamo"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["David Jetter <davidajetter@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pydantic_dynamo"}]
 homepage = "https://github.com/david-a-jetter/pydantic-dynamo"
 
 [tool.poetry.dependencies]
@@ -21,25 +21,30 @@
 faker = "^17.6.0"
 doit = "^0.36.0"
 pytest-cov = "^4.0.0"
 mypy = "^1.1.1"
 flake8 = "^6.0.0"
 testcontainers = "^3.7.1"
 tzdata = "^2023.3"
+pytest-asyncio = "^0.21.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 100
 
 #[tool.coverage.run]
 #source = ["pydantic_dynamo"]
 
+
+[tool.pytest]
+asyncio_mode = "auto"
+
 [tool.mypy]
 python_version = 3.9
 plugins = "pydantic.mypy"
 warn_return_any = true
 warn_unused_configs = true
 show_error_codes = true
```

### Comparing `pydantic_dynamo-0.2.1/README.md` & `pydantic_dynamo-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -103,17 +103,45 @@
         partition_name="integration",
         content_type="example",
         table_name="table_name",
         partition_key="PARTITION_KEY",
         sort_key="SORT_KEY",
         table=await resource.Table("table_name"),
         resource=resource,
+        consistent_reads=False,  # default
     )
 ```
 
+The repository class also implements `AsyncContextManager` so it can be readily used in `async with...` statements.
+This may make it easier to properly manage other object dependencies in factory/builder functions.
+```python
+from contextlib import asynccontextmanager
+from aioboto3 import Session
+from pydantic_dynamo.v2.repository import DynamoRepository
+from tests.models import Example  # Use your record model instead
+
+@asynccontextmanager
+async def build_repo() -> DynamoRepository[Example]:
+    session = Session()
+    boto3_kwargs = {"service_name": "dynamodb"}  # endpoint_url, region_name, etc.
+    async with session.resource(**boto3_kwargs) as resource, DynamoRepository[Example](
+        item_class=Example,
+        partition_prefix="test",
+        partition_name="integration",
+        content_type="example",
+        table_name="table_name",
+        partition_key="PARTITION_KEY",
+        sort_key="SORT_KEY",
+        table=await resource.Table("table_name"),
+        resource=resource,
+        consistent_reads=False,  # default
+    ) as repo:
+        yield repo
+```
+
 There is also a synchronous variant that can be used if you don't want to work with async/await and async generators
 in your business code. Most of the subsequent documentation is focused on the async variant.
 
 ```python
 from aioboto3 import Session
 from pydantic_dynamo.v2.repository import DynamoRepository
 from pydantic_dynamo.v2.sync_repository import SyncDynamoRepository
@@ -128,18 +156,27 @@
         partition_name="integration",
         content_type="example",
         table_name="table_name",
         partition_key="PARTITION_KEY",
         sort_key="SORT_KEY",
         table=await resource.Table("table_name"),
         resource=resource,
+        consistent_reads=False,  # default
     )
 
     sync_repo = SyncDynamoRepository[Example](async_repo=repo)
 ```
+
+#### Consistent Reads
+By default, both boto3 and this library use eventually consistent read operations.
+You can configure a repository instance to use strongly consistent reads by passing the
+`consistent_reads` kwarg as `True` during instantiation.
+
+You can [read more about read consistency in AWS's documentation.](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.ReadConsistency.html)
+
 ### Saving Data
 
 Data is saved using an instance of the generic `PartitionedContent[ObjT]` class found in 
 [models.py](./pydantic_dynamo/models.py). The `partition_ids` and `content_ids` are `List[str]`. 
 Each value in the list is concatenated before saving, and prefixed with the repository's configured values.
 
 For the `content_ids` field, you can leverage this to achieve degrees of query-ability for
```

### Comparing `pydantic_dynamo-0.2.1/PKG-INFO` & `pydantic_dynamo-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-dynamo
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Home-page: https://github.com/david-a-jetter/pydantic-dynamo
 Author: David Jetter
 Author-email: davidajetter@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -121,17 +121,45 @@
         partition_name="integration",
         content_type="example",
         table_name="table_name",
         partition_key="PARTITION_KEY",
         sort_key="SORT_KEY",
         table=await resource.Table("table_name"),
         resource=resource,
+        consistent_reads=False,  # default
     )
 ```
 
+The repository class also implements `AsyncContextManager` so it can be readily used in `async with...` statements.
+This may make it easier to properly manage other object dependencies in factory/builder functions.
+```python
+from contextlib import asynccontextmanager
+from aioboto3 import Session
+from pydantic_dynamo.v2.repository import DynamoRepository
+from tests.models import Example  # Use your record model instead
+
+@asynccontextmanager
+async def build_repo() -> DynamoRepository[Example]:
+    session = Session()
+    boto3_kwargs = {"service_name": "dynamodb"}  # endpoint_url, region_name, etc.
+    async with session.resource(**boto3_kwargs) as resource, DynamoRepository[Example](
+        item_class=Example,
+        partition_prefix="test",
+        partition_name="integration",
+        content_type="example",
+        table_name="table_name",
+        partition_key="PARTITION_KEY",
+        sort_key="SORT_KEY",
+        table=await resource.Table("table_name"),
+        resource=resource,
+        consistent_reads=False,  # default
+    ) as repo:
+        yield repo
+```
+
 There is also a synchronous variant that can be used if you don't want to work with async/await and async generators
 in your business code. Most of the subsequent documentation is focused on the async variant.
 
 ```python
 from aioboto3 import Session
 from pydantic_dynamo.v2.repository import DynamoRepository
 from pydantic_dynamo.v2.sync_repository import SyncDynamoRepository
@@ -146,18 +174,27 @@
         partition_name="integration",
         content_type="example",
         table_name="table_name",
         partition_key="PARTITION_KEY",
         sort_key="SORT_KEY",
         table=await resource.Table("table_name"),
         resource=resource,
+        consistent_reads=False,  # default
     )
 
     sync_repo = SyncDynamoRepository[Example](async_repo=repo)
 ```
+
+#### Consistent Reads
+By default, both boto3 and this library use eventually consistent read operations.
+You can configure a repository instance to use strongly consistent reads by passing the
+`consistent_reads` kwarg as `True` during instantiation.
+
+You can [read more about read consistency in AWS's documentation.](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.ReadConsistency.html)
+
 ### Saving Data
 
 Data is saved using an instance of the generic `PartitionedContent[ObjT]` class found in 
 [models.py](./pydantic_dynamo/models.py). The `partition_ids` and `content_ids` are `List[str]`. 
 Each value in the list is concatenated before saving, and prefixed with the repository's configured values.
 
 For the `content_ids` field, you can leverage this to achieve degrees of query-ability for
```

