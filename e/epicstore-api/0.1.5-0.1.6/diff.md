# Comparing `tmp/epicstore_api-0.1.5.tar.gz` & `tmp/epicstore_api-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\epicstore_api-0.1.5.tar", last modified: Tue Feb 21 18:44:40 2023, max compression
+gzip compressed data, was "dist\epicstore_api-0.1.6.tar", last modified: Sat Apr 29 14:45:48 2023, max compression
```

## Comparing `epicstore_api-0.1.5.tar` & `epicstore_api-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-02-21 18:44:40.366915 epicstore_api-0.1.5/
--rw-rw-rw-   0        0        0     2983 2023-02-21 18:44:40.366915 epicstore_api-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1619 2022-11-21 17:13:50.000000 epicstore_api-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-02-21 18:44:40.333908 epicstore_api-0.1.5/epicstore_api/
--rw-rw-rw-   0        0        0      299 2022-11-21 17:14:46.000000 epicstore_api-0.1.5/epicstore_api/__init__.py
--rw-rw-rw-   0        0        0    17353 2023-02-21 18:41:14.000000 epicstore_api-0.1.5/epicstore_api/api.py
--rw-rw-rw-   0        0        0     1769 2023-02-21 18:41:14.000000 epicstore_api-0.1.5/epicstore_api/exc.py
-drwxrwxrwx   0        0        0        0 2023-02-21 18:44:40.363914 epicstore_api-0.1.5/epicstore_api/models/
--rw-rw-rw-   0        0        0     1209 2022-11-21 17:14:46.000000 epicstore_api-0.1.5/epicstore_api/models/__init__.py
--rw-rw-rw-   0        0        0     2739 2022-11-21 17:14:46.000000 epicstore_api-0.1.5/epicstore_api/models/categories.py
--rw-rw-rw-   0        0        0     1475 2022-11-21 17:14:46.000000 epicstore_api-0.1.5/epicstore_api/models/product_types.py
--rw-rw-rw-   0        0        0    15470 2022-11-21 17:14:46.000000 epicstore_api-0.1.5/epicstore_api/queries.py
-drwxrwxrwx   0        0        0        0 2023-02-21 18:44:40.348912 epicstore_api-0.1.5/epicstore_api.egg-info/
--rw-rw-rw-   0        0        0     2983 2023-02-21 18:44:40.000000 epicstore_api-0.1.5/epicstore_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      401 2023-02-21 18:44:40.000000 epicstore_api-0.1.5/epicstore_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-21 18:44:40.000000 epicstore_api-0.1.5/epicstore_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-02-21 18:44:40.000000 epicstore_api-0.1.5/epicstore_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-02-21 18:44:40.000000 epicstore_api-0.1.5/epicstore_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-21 18:44:40.366915 epicstore_api-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1294 2023-02-21 18:39:50.000000 epicstore_api-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 14:45:48.079554 epicstore_api-0.1.6/
+-rw-rw-rw-   0        0        0     2983 2023-04-29 14:45:48.079554 epicstore_api-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1619 2022-11-21 17:13:50.000000 epicstore_api-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 14:45:48.058556 epicstore_api-0.1.6/epicstore_api/
+-rw-rw-rw-   0        0        0      299 2023-04-29 14:21:08.000000 epicstore_api-0.1.6/epicstore_api/__init__.py
+-rw-rw-rw-   0        0        0    18647 2023-04-29 14:35:37.000000 epicstore_api-0.1.6/epicstore_api/api.py
+-rw-rw-rw-   0        0        0     1769 2023-04-29 14:21:08.000000 epicstore_api-0.1.6/epicstore_api/exc.py
+drwxrwxrwx   0        0        0        0 2023-04-29 14:45:48.078560 epicstore_api-0.1.6/epicstore_api/models/
+-rw-rw-rw-   0        0        0     1258 2023-04-29 14:21:08.000000 epicstore_api-0.1.6/epicstore_api/models/__init__.py
+-rw-rw-rw-   0        0        0     2739 2023-04-29 14:21:08.000000 epicstore_api-0.1.6/epicstore_api/models/categories.py
+-rw-rw-rw-   0        0        0     1846 2023-04-29 14:21:08.000000 epicstore_api-0.1.6/epicstore_api/models/collection_types.py
+-rw-rw-rw-   0        0        0     1475 2023-04-29 14:21:08.000000 epicstore_api-0.1.6/epicstore_api/models/product_types.py
+-rw-rw-rw-   0        0        0    18275 2023-04-29 14:21:08.000000 epicstore_api-0.1.6/epicstore_api/queries.py
+drwxrwxrwx   0        0        0        0 2023-04-29 14:45:48.075555 epicstore_api-0.1.6/epicstore_api.egg-info/
+-rw-rw-rw-   0        0        0     2983 2023-04-29 14:45:47.000000 epicstore_api-0.1.6/epicstore_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-04-29 14:45:47.000000 epicstore_api-0.1.6/epicstore_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 14:45:47.000000 epicstore_api-0.1.6/epicstore_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-29 14:45:47.000000 epicstore_api-0.1.6/epicstore_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-29 14:45:47.000000 epicstore_api-0.1.6/epicstore_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 14:45:48.079554 epicstore_api-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1294 2023-04-29 14:06:46.000000 epicstore_api-0.1.6/setup.py
```

### Comparing `epicstore_api-0.1.5/PKG-INFO` & `epicstore_api-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: epicstore_api
-Version: 0.1.5
+Version: 0.1.6
 Summary: An API wrapper for Epic Games Store written in Python
 Home-page: https://github.com/SD4RK/epicstore_api
 Author: SD4RK
 License: MIT
-Download-URL: https://github.com/SD4RK/epicstore_api/archive/v_0.1.5.tar.gz
+Download-URL: https://github.com/SD4RK/epicstore_api/archive/v_0.1.6.tar.gz
 Description: # epicstore_api
         
         [![Current pypi version](https://img.shields.io/pypi/v/epicstore-api.svg)](https://pypi.org/project/epicstore-api/)
         [![Supported py versions](https://img.shields.io/pypi/pyversions/epicstore-api.svg)](https://pypi.org/project/epicstore-api/)
         [![Downloads](https://pepy.tech/badge/epicstore-api)](https://pypi.org/project/epicstore-api/)
         
         An unofficial library to work with Epic Games Store Web API.
```

### Comparing `epicstore_api-0.1.5/README.md` & `epicstore_api-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `epicstore_api-0.1.5/epicstore_api/api.py` & `epicstore_api-0.1.6/epicstore_api/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 """
 MIT License
 
-Copyright (c) 2020-2022 SD4RK
+Copyright (c) 2020-2023 SD4RK
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -25,25 +25,26 @@
 """
 
 
 import json
 import requests
 from typing import Union, List, NamedTuple
 from .exc import EGSNotFound, EGSException
-from .models import EGSCategory, EGSProductType
+from .models import EGSCategory, EGSProductType, EGSCollectionType
 from .queries import (CATALOG_QUERY,
                       PROMOTIONS_QUERY,
                       CATALOG_TAGS_QUERY,
                       FEED_QUERY,
                       PREREQUISITES_QUERY,
                       OFFERS_QUERY,
                       STORE_QUERY,
                       ADDONS_QUERY,
                       MEDIA_QUERY,
-                      PRODUCT_REVIEWS_QUERY)
+                      PRODUCT_REVIEWS_QUERY,
+                      COLLECTION_QUERY)
 
 
 class OfferData(NamedTuple):
     namespace: str
     offer_id: str
 
 
@@ -131,14 +132,38 @@
                     'quantity': 1
                 }],
                 'calculateTax': should_calculate_tax,
                 'includeSubItems': include_sub_items
             } for offer in offers]
         )
 
+    def get_collection(self, collection: EGSCollectionType) -> dict:
+        """Returns games from the collection by the given collection type
+        (see the documentation for CollectionType class).
+
+        :param collection: Needed collection type.
+        """
+        raw = self._make_graphql_query(
+            COLLECTION_QUERY,
+            slug=collection.value,
+            # This query always returns 1004 error by default. That is not controlled by us and the error itself
+            # is happening even in the official EGS client itself, they're just ignoring it, so we will too.
+            suppress_errors=True
+        )
+        # Cleanup for the 1004 errors that always pop up by default to not mess someone up by this.
+        if 'errors' in raw:
+            for error in raw['errors'].copy():
+                service_response = json.loads(error.get('serviceResponse', {}))
+                if service_response:
+                    if service_response.get('numericErrorCode') == 1004:
+                        raw['errors'].remove(error)
+            if not raw['errors']:
+                raw.pop('errors')
+        return raw
+
     def fetch_media(self, media_ref_id: str) -> dict:
         """Returns media-file (type of the file, its url and so on) by the
         file's media ref ID.
 
         :param media_ref_id: File's media ref ID.
         """
         return self._make_graphql_query(
@@ -400,24 +425,25 @@
         self._get_errors(response)
         return response
 
     def _make_graphql_query(
         self,
         query_string,
         headers={},
+        suppress_errors=False,
         *multiple_query_variables,
         **variables
     ) -> dict:
         if not multiple_query_variables:
             variables.update({'locale': self.locale, 'country': self.country})
             # This variables are default and exist in all graphql queries
             response = self._session.post(
                 'https://graphql.epicgames.com/graphql',
                 json={'query': query_string, 'variables': variables},
-                headers=headers
+                headers=headers,
             ).json()
         else:
             data = []
             for variables in multiple_query_variables:
                 variables_ = {
                     'locale': self.locale,
                     'country': self.country,
@@ -428,15 +454,16 @@
                     'variables': variables_
                 })
             response = self._session.post(
                 'https://graphql.epicgames.com/graphql',
                 json=data,
                 headers=headers
             ).json()
-        self._get_errors(response)
+        if not suppress_errors:
+            self._get_errors(response)
         return response
 
     @staticmethod
     def _get_errors(resp):
         r = []
         if not isinstance(resp, list):
             r.append(resp)
```

### Comparing `epicstore_api-0.1.5/epicstore_api/exc.py` & `epicstore_api-0.1.6/epicstore_api/exc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 """
 MIT License
 
-Copyright (c) 2020-2022 SD4RK
+Copyright (c) 2020-2023 SD4RK
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `epicstore_api-0.1.5/epicstore_api/models/__init__.py` & `epicstore_api-0.1.6/epicstore_api/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 """
 MIT License
 
-Copyright (c) 2020-2022 SD4RK
+Copyright (c) 2020-2023 SD4RK
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -23,7 +23,8 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 
 from .categories import EGSCategory
 from .product_types import EGSProductType
+from .collection_types import EGSCollectionType
```

### Comparing `epicstore_api-0.1.5/epicstore_api/models/categories.py` & `epicstore_api-0.1.6/epicstore_api/models/categories.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 """
 MIT License
 
-Copyright (c) 2020-2022 SD4RK
+Copyright (c) 2020-2023 SD4RK
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `epicstore_api-0.1.5/epicstore_api/models/product_types.py` & `epicstore_api-0.1.6/epicstore_api/models/product_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 """
 MIT License
 
-Copyright (c) 2020-2022 SD4RK
+Copyright (c) 2020-2023 SD4RK
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `epicstore_api-0.1.5/epicstore_api/queries.py` & `epicstore_api-0.1.6/epicstore_api/queries.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 """
 MIT License
 
-Copyright (c) 2020-2022 SD4RK
+Copyright (c) 2020-2023 SD4RK
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -31,8 +31,9 @@
 CATALOG_TAGS_QUERY = "\n            query catalogTags($namespace: String!)\n            {\n                Catalog {\n                    tags (\n                        namespace: $namespace,\n                        start: 0,\n                        count: 999\n                    ) {\n                        elements {\n                            aliases,\n                            id,\n                            name,\n                            referenceCount,\n                            status\n                        }\n                    }\n                }\n            }\n            "
 FEED_QUERY = "\n            query feedQuery($locale: String!, $countryCode: String, $offset: Int, $postsPerPage: Int, $category: String) {\n                TransientStream {\n                    myTransientFeed(countryCode: $countryCode, locale: $locale) {\n                        id\n                        activity {\n                            # TODO Comment in to enable welcome post when requirements are finalized\n                            # ...on SimpleActivity {\n                            #     type\n                            #     created_at\n                            # }\n                            ...on LinkAccountActivity {\n                                type\n                                created_at\n                                platforms\n                            }\n                            ...on SuggestedFriendsActivity {\n                                type\n                                created_at\n                                platform\n                                suggestions {\n                                    epicId\n                                    epicDisplayName\n                                    platformFullName\n                                    platformAvatar\n                                }\n                            }\n                            ...on IncomingInvitesActivity {\n                                type\n                                created_at\n                                invites {\n                                    epicId\n                                    epicDisplayName\n                                }\n                            }\n                            ...on RecentPlayersActivity {\n                                type\n                                created_at\n                                players {\n                                    epicId\n                                    epicDisplayName\n                                    playedGameName\n                                }\n                            }\n                        }\n                    }\n                }\n                Blog {\n                    dieselBlogPosts: getPosts(locale: $locale, offset: $offset, postsPerPage: $postsPerPage, category: $category) {\n                        blogList {\n                            _id\n                            author\n                            category\n                            content\n                            urlPattern\n                            slug\n                            sticky\n                            title\n                            date\n                            image\n                            shareImage\n                            trendingImage\n                            url\n                            featured\n                            link\n                            externalLink\n                        }\n                    }\n                }\n            }"
 PREREQUISITES_QUERY = "\n    query fetchPrerequisites($offerParams: [OfferParams]) {\n        Launcher{\n            prerequisites(offerParams:$offerParams) {\n                namespace,\n                offerId,\n                missingPrerequisiteItems\n                satisfiesPrerequisites\n            }\n        }\n    }\n"
 OFFERS_QUERY = "\n    query catalogQuery($productNamespace: String!, $offerId: String!, $locale: String, $country: String!, $includeSubItems: Boolean!) {\n  Catalog {\n    catalogOffer(namespace: $productNamespace, id: $offerId, locale: $locale) {\n      title\n      id\n      namespace\n      description\n      effectiveDate\n      expiryDate\n      isCodeRedemptionOnly\n      keyImages {\n        type\n        url\n      }\n      seller {\n        id\n        name\n      }\n      productSlug\n      urlSlug\n      url\n      tags {\n        id\n      }\n      items {\n        id\n        namespace\n      }\n      customAttributes {\n        key\n        value\n      }\n      categories {\n        path\n      }\n      price(country: $country) {\n        totalPrice {\n          discountPrice\n          originalPrice\n          voucherDiscount\n          discount\n          currencyCode\n          currencyInfo {\n            decimals\n          }\n          fmtPrice(locale: $locale) {\n            originalPrice\n            discountPrice\n            intermediatePrice\n          }\n        }\n        lineOffers {\n          appliedRules {\n            id\n            endDate\n            discountSetting {\n              discountType\n            }\n          }\n        }\n      }\n    }\n    offerSubItems(namespace: $productNamespace, id: $offerId) @include(if: $includeSubItems) {\n      namespace\n      id\n      releaseInfo {\n        appId\n        platform\n      }\n    }\n  }\n}\n"
 MEDIA_QUERY = "\n    query fetchMediaRef($mediaRefId: String!) {\n      Media {\n        getMediaRef(mediaRefId: $mediaRefId) {\n          accountId\n          outputs {\n            duration\n            url\n            width\n            height\n            key\n            contentType\n          }\n          namespace\n        }\n      }\n    }\n"
 PRODUCT_REVIEWS_QUERY = "\n            query productReviewsQuery($sku: String!) {\n                OpenCritic {\n                    productReviews(sku: $sku) {\n                        id\n                        name\n                        openCriticScore\n                        reviewCount\n                        percentRecommended\n                        openCriticUrl\n                        award\n                        topReviews {\n                            publishedDate\n                            externalUrl\n                            snippet\n                            language\n                            score\n                            author\n                            ScoreFormat {\n                                id\n                                description\n                            }\n                            OutletId\n                            outletName\n                            displayScore\n                        }\n                    }\n                }\n            }\n        "
 ADDONS_QUERY = "query getAddonsByNamespace($categories: String!, $count: Int!, $country: String!, $locale: String!, $namespace: String!, $sortBy: String!, $sortDir: String!) {\n  Catalog {\n    catalogOffers(namespace: $namespace, locale: $locale, params: {category: $categories, count: $count, country: $country, sortBy: $sortBy, sortDir: $sortDir}) {\n      elements {\n        countriesBlacklist\n        customAttributes {\n          key\n          value\n        }\n        description\n        developer\n        effectiveDate\n        id\n        isFeatured\n        keyImages {\n          type\n          url\n        }\n        lastModifiedDate\n        longDescription\n        namespace\n        offerType\n        productSlug\n        releaseDate\n        status\n        technicalDetails\n        title\n        urlSlug\n      }\n    }\n  }\n}\n"
+COLLECTION_QUERY = "query collectionLayoutQuery($locale: String, $country: String!, $slug: String) {\n  Storefront {\n    collectionLayout(locale: $locale, slug: $slug) {\n      _activeDate\n      _locale\n      _metaTags\n      _slug\n      _title\n      _urlPattern\n      lastModified\n      regionBlock\n      affiliateId\n      takeover {\n        banner {\n          altText\n          src\n        }\n        description\n        eyebrow\n        title\n      }\n      seo {\n        title\n        description\n        keywords\n        image {\n          src\n          altText\n        }\n        twitter {\n          title\n          description\n        }\n        og {\n          title\n          description\n          image {\n            src\n            alt\n          }\n        }\n      }\n      collectionOffers {\n        title\n        id\n        namespace\n        description\n        effectiveDate\n        countriesBlacklist\n        countriesWhitelist\n        developerDisplayName\n        publisherDisplayName\n        keyImages {\n          type\n          url\n        }\n        seller {\n          id\n          name\n        }\n        releaseDate\n        pcReleaseDate\n        approximateReleasePlan {\n          day\n          month\n          quarter\n          year\n          releaseDateType\n        }\n        prePurchase\n        productSlug\n        urlSlug\n        url\n        items {\n          id\n          namespace\n        }\n        customAttributes {\n          key\n          value\n        }\n        categories {\n          path\n        }\n        linkedOfferId\n        linkedOffer {\n          effectiveDate\n          customAttributes {\n            key\n            value\n          }\n        }\n        catalogNs {\n          mappings(pageType: \"productHome\") {\n            pageSlug\n            pageType\n          }\n        }\n        offerMappings {\n          pageSlug\n          pageType\n        }\n        price(country: $country) {\n          totalPrice {\n            currencyCode\n            currencyInfo {\n              decimals\n              symbol\n            }\n            discountPrice\n            originalPrice\n            voucherDiscount\n            discount\n            fmtPrice(locale: $locale) {\n              originalPrice\n              discountPrice\n              intermediatePrice\n            }\n          }\n          lineOffers {\n            appliedRules {\n              id\n              endDate\n            }\n          }\n        }\n      }\n      pageTheme {\n        preferredMode\n        light {\n          theme\n          accent\n        }\n        dark {\n          theme\n          accent\n        }\n      }\n      redirect {\n        code\n        url\n      }\n    }\n  }\n}\n"
 # XXX: This code violates PEP 8, line > 79 chars
```

### Comparing `epicstore_api-0.1.5/epicstore_api.egg-info/PKG-INFO` & `epicstore_api-0.1.6/epicstore_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: epicstore-api
-Version: 0.1.5
+Version: 0.1.6
 Summary: An API wrapper for Epic Games Store written in Python
 Home-page: https://github.com/SD4RK/epicstore_api
 Author: SD4RK
 License: MIT
-Download-URL: https://github.com/SD4RK/epicstore_api/archive/v_0.1.5.tar.gz
+Download-URL: https://github.com/SD4RK/epicstore_api/archive/v_0.1.6.tar.gz
 Description: # epicstore_api
         
         [![Current pypi version](https://img.shields.io/pypi/v/epicstore-api.svg)](https://pypi.org/project/epicstore-api/)
         [![Supported py versions](https://img.shields.io/pypi/pyversions/epicstore-api.svg)](https://pypi.org/project/epicstore-api/)
         [![Downloads](https://pepy.tech/badge/epicstore-api)](https://pypi.org/project/epicstore-api/)
         
         An unofficial library to work with Epic Games Store Web API.
```

### Comparing `epicstore_api-0.1.5/setup.py` & `epicstore_api-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 AUTHOR = 'SD4RK'
-VERSION = '0.1.5'
+VERSION = '0.1.6'
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='epicstore_api',
     version=VERSION,
```

