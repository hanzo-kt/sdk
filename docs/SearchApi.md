# SearchApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**botSearchPersonas**](SearchApi.md#botSearchPersonas) | **GET** /v1/bot/search/personas | Lexical search for personas |
| [**botSearchSkills**](SearchApi.md#botSearchSkills) | **GET** /v1/bot/search/skills | Hybrid vector + lexical search for skills |
| [**chatGetSearchEnable**](SearchApi.md#chatGetSearchEnable) | **GET** /v1/chat/search/enable | Check if search is enabled |
| [**commerceSearchNotes**](SearchApi.md#commerceSearchNotes) | **POST** /v1/commerce/search/note | Search notes |
| [**commerceSearchOrders**](SearchApi.md#commerceSearchOrders) | **GET** /v1/commerce/search/order | Search orders |
| [**commerceSearchUsers**](SearchApi.md#commerceSearchUsers) | **GET** /v1/commerce/search/user | Search users |
| [**kbKbSearch**](SearchApi.md#kbKbSearch) | **POST** /v1/kb/search | Semantic search over the org&#39;s knowledge |
| [**productGetSearchStats**](SearchApi.md#productGetSearchStats) | **GET** /v1/search-docs/stats | Get aggregate search statistics |
| [**productListSearchIndexes**](SearchApi.md#productListSearchIndexes) | **GET** /v1/search-docs/indexes | List search indexes |
| [**provisioningCreateSearch**](SearchApi.md#provisioningCreateSearch) | **POST** /v1/search | Provision a search resource |
| [**provisioningDeleteSearch**](SearchApi.md#provisioningDeleteSearch) | **DELETE** /v1/search/{name} | Deprovision a search resource |
| [**provisioningGetSearch**](SearchApi.md#provisioningGetSearch) | **GET** /v1/search/{name} | Get one search resource |
| [**provisioningListSearch**](SearchApi.md#provisioningListSearch) | **GET** /v1/search | List search resources for the caller&#39;s org |
| [**searchSearchGet**](SearchApi.md#searchSearchGet) | **GET** /v1/search/indexes/{indexUid}/search | Search documents (GET) |
| [**searchSearchPost**](SearchApi.md#searchSearchPost) | **POST** /v1/search/indexes/{indexUid}/search | Search documents (POST) |
| [**vectorRecommendPoints**](SearchApi.md#vectorRecommendPoints) | **POST** /v1/vector/collections/{collection_name}/points/recommend | Recommend points |
| [**vectorSearchBatch**](SearchApi.md#vectorSearchBatch) | **POST** /v1/vector/collections/{collection_name}/points/search/batch | Batch search |
| [**vectorSearchPoints**](SearchApi.md#vectorSearchPoints) | **POST** /v1/vector/collections/{collection_name}/points/search | Search points |
| [**websearchWebSearch**](SearchApi.md#websearchWebSearch) | **GET** /v1/websearch/search | Search the web (SearXNG JSON contract, proxied verbatim) |


<a id="botSearchPersonas"></a>
# **botSearchPersonas**
> BotSearchPersonas200Response botSearchPersonas(q, limit)

Lexical search for personas

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SearchApi()
val q : kotlin.String = q_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : BotSearchPersonas200Response = apiInstance.botSearchPersonas(q, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchApi#botSearchPersonas")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchApi#botSearchPersonas")
    e.printStackTrace()
}
```

### Parameters
| **q** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] [default to 20] |

### Return type

[**BotSearchPersonas200Response**](BotSearchPersonas200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="botSearchSkills"></a>
# **botSearchSkills**
> BotSearchPersonas200Response botSearchSkills(q, limit)

Hybrid vector + lexical search for skills

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SearchApi()
val q : kotlin.String = q_example // kotlin.String | Search query
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : BotSearchPersonas200Response = apiInstance.botSearchSkills(q, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchApi#botSearchSkills")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchApi#botSearchSkills")
    e.printStackTrace()
}
```

### Parameters
| **q** | **kotlin.String**| Search query | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] [default to 20] |

### Return type

[**BotSearchPersonas200Response**](BotSearchPersonas200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="chatGetSearchEnable"></a>
# **chatGetSearchEnable**
> kotlin.Boolean chatGetSearchEnable()

Check if search is enabled

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SearchApi()
try {
    val result : kotlin.Boolean = apiInstance.chatGetSearchEnable()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchApi#chatGetSearchEnable")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchApi#chatGetSearchEnable")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

**kotlin.Boolean**

### Authorization


Configure bearerAuth statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearerAuth dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="commerceSearchNotes"></a>
# **commerceSearchNotes**
> kotlin.collections.List&lt;CommerceNote&gt; commerceSearchNotes(commerceSearchNotesRequest)

Search notes

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SearchApi()
val commerceSearchNotesRequest : CommerceSearchNotesRequest =  // CommerceSearchNotesRequest | 
try {
    val result : kotlin.collections.List<CommerceNote> = apiInstance.commerceSearchNotes(commerceSearchNotesRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchApi#commerceSearchNotes")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchApi#commerceSearchNotes")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceSearchNotesRequest** | [**CommerceSearchNotesRequest**](CommerceSearchNotesRequest.md)|  | |

### Return type

[**kotlin.collections.List&lt;CommerceNote&gt;**](CommerceNote.md)

### Authorization


Configure bearerAuth statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearerAuth dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="commerceSearchOrders"></a>
# **commerceSearchOrders**
> kotlin.collections.List&lt;CommerceOrder&gt; commerceSearchOrders(q)

Search orders

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SearchApi()
val q : kotlin.String = q_example // kotlin.String | 
try {
    val result : kotlin.collections.List<CommerceOrder> = apiInstance.commerceSearchOrders(q)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchApi#commerceSearchOrders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchApi#commerceSearchOrders")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **q** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.List&lt;CommerceOrder&gt;**](CommerceOrder.md)

### Authorization


Configure bearerAuth statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearerAuth dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="commerceSearchUsers"></a>
# **commerceSearchUsers**
> kotlin.collections.List&lt;CommerceUser&gt; commerceSearchUsers(q)

Search users

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SearchApi()
val q : kotlin.String = q_example // kotlin.String | 
try {
    val result : kotlin.collections.List<CommerceUser> = apiInstance.commerceSearchUsers(q)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchApi#commerceSearchUsers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchApi#commerceSearchUsers")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **q** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.List&lt;CommerceUser&gt;**](CommerceUser.md)

### Authorization


Configure bearerAuth statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearerAuth dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="kbKbSearch"></a>
# **kbKbSearch**
> KbKbSearch200Response kbKbSearch(kbSearchRequest)

Semantic search over the org&#39;s knowledge

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SearchApi()
val kbSearchRequest : KbSearchRequest =  // KbSearchRequest | 
try {
    val result : KbKbSearch200Response = apiInstance.kbKbSearch(kbSearchRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchApi#kbKbSearch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchApi#kbKbSearch")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kbSearchRequest** | [**KbSearchRequest**](KbSearchRequest.md)|  | |

### Return type

[**KbKbSearch200Response**](KbKbSearch200Response.md)

### Authorization


Configure bearerAuth statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearerAuth dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="productGetSearchStats"></a>
# **productGetSearchStats**
> ProductSearchStats productGetSearchStats()

Get aggregate search statistics

Returns the total document count across all Meilisearch indexes. Meilisearch keeps no query-history counters, so &#x60;totalSearches&#x60;, &#x60;totalSessions&#x60;, and the &#x60;searchesPerDay&#x60; series are reported as an honest zero/empty rather than a fabricated number. If the upstream is unreachable, returns HTTP 200 with all counters zeroed. Authenticated with the opaque search service key. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SearchApi()
try {
    val result : ProductSearchStats = apiInstance.productGetSearchStats()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchApi#productGetSearchStats")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchApi#productGetSearchStats")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ProductSearchStats**](ProductSearchStats.md)

### Authorization


Configure bearerAuth statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearerAuth dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="productListSearchIndexes"></a>
# **productListSearchIndexes**
> ProductListSearchIndexes200Response productListSearchIndexes()

List search indexes

Returns every Meilisearch index with its document count and, on a best-effort basis, its created/last-indexed timestamps. If the upstream Meilisearch is unreachable, returns HTTP 200 with an empty &#x60;indexes&#x60; array. Authenticated with the opaque search service key. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SearchApi()
try {
    val result : ProductListSearchIndexes200Response = apiInstance.productListSearchIndexes()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchApi#productListSearchIndexes")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchApi#productListSearchIndexes")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ProductListSearchIndexes200Response**](ProductListSearchIndexes200Response.md)

### Authorization


Configure bearerAuth statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearerAuth dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="provisioningCreateSearch"></a>
# **provisioningCreateSearch**
> ProvisioningCreateResponse provisioningCreateSearch(provisioningCreateRequest)

Provision a search resource

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SearchApi()
val provisioningCreateRequest : ProvisioningCreateRequest =  // ProvisioningCreateRequest | 
try {
    val result : ProvisioningCreateResponse = apiInstance.provisioningCreateSearch(provisioningCreateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchApi#provisioningCreateSearch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchApi#provisioningCreateSearch")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **provisioningCreateRequest** | [**ProvisioningCreateRequest**](ProvisioningCreateRequest.md)|  | |

### Return type

[**ProvisioningCreateResponse**](ProvisioningCreateResponse.md)

### Authorization


Configure bearerAuth statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearerAuth dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="provisioningDeleteSearch"></a>
# **provisioningDeleteSearch**
> provisioningDeleteSearch(name)

Deprovision a search resource

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SearchApi()
val name : kotlin.String = name_example // kotlin.String | The user-supplied resource name (slug). Lowercased and trimmed server-side; must match `^[a-z0-9]([a-z0-9-]{0,38}[a-z0-9])?$`. 
try {
    apiInstance.provisioningDeleteSearch(name)
} catch (e: ClientException) {
    println("4xx response calling SearchApi#provisioningDeleteSearch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchApi#provisioningDeleteSearch")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**| The user-supplied resource name (slug). Lowercased and trimmed server-side; must match &#x60;^[a-z0-9]([a-z0-9-]{0,38}[a-z0-9])?$&#x60;.  | |

### Return type

null (empty response body)

### Authorization


Configure bearerAuth statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearerAuth dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="provisioningGetSearch"></a>
# **provisioningGetSearch**
> ProvisioningGetResponse provisioningGetSearch(name)

Get one search resource

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SearchApi()
val name : kotlin.String = name_example // kotlin.String | The user-supplied resource name (slug). Lowercased and trimmed server-side; must match `^[a-z0-9]([a-z0-9-]{0,38}[a-z0-9])?$`. 
try {
    val result : ProvisioningGetResponse = apiInstance.provisioningGetSearch(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchApi#provisioningGetSearch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchApi#provisioningGetSearch")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**| The user-supplied resource name (slug). Lowercased and trimmed server-side; must match &#x60;^[a-z0-9]([a-z0-9-]{0,38}[a-z0-9])?$&#x60;.  | |

### Return type

[**ProvisioningGetResponse**](ProvisioningGetResponse.md)

### Authorization


Configure bearerAuth statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearerAuth dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="provisioningListSearch"></a>
# **provisioningListSearch**
> kotlin.collections.List&lt;ProvisioningListItem&gt; provisioningListSearch()

List search resources for the caller&#39;s org

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SearchApi()
try {
    val result : kotlin.collections.List<ProvisioningListItem> = apiInstance.provisioningListSearch()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchApi#provisioningListSearch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchApi#provisioningListSearch")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;ProvisioningListItem&gt;**](ProvisioningListItem.md)

### Authorization


Configure bearerAuth statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearerAuth dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="searchSearchGet"></a>
# **searchSearchGet**
> SearchSearchResult searchSearchGet(indexUid, q, offset, limit, attributesToRetrieve, attributesToHighlight, attributesToCrop, cropLength, filter, sort, facets, showMatchesPosition, showRankingScore, matchingStrategy)

Search documents (GET)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SearchApi()
val indexUid : kotlin.String = indexUid_example // kotlin.String | Unique index identifier
val q : kotlin.String = q_example // kotlin.String | Search query
val offset : kotlin.Int = 56 // kotlin.Int | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val attributesToRetrieve : kotlin.String = attributesToRetrieve_example // kotlin.String | Comma-separated list of attributes to return
val attributesToHighlight : kotlin.String = attributesToHighlight_example // kotlin.String | 
val attributesToCrop : kotlin.String = attributesToCrop_example // kotlin.String | 
val cropLength : kotlin.Int = 56 // kotlin.Int | 
val filter : kotlin.String = filter_example // kotlin.String | Filter expression
val sort : kotlin.String = sort_example // kotlin.String | Comma-separated sort rules
val facets : kotlin.String = facets_example // kotlin.String | Comma-separated facet attributes
val showMatchesPosition : kotlin.Boolean = true // kotlin.Boolean | 
val showRankingScore : kotlin.Boolean = true // kotlin.Boolean | 
val matchingStrategy : kotlin.String = matchingStrategy_example // kotlin.String | 
try {
    val result : SearchSearchResult = apiInstance.searchSearchGet(indexUid, q, offset, limit, attributesToRetrieve, attributesToHighlight, attributesToCrop, cropLength, filter, sort, facets, showMatchesPosition, showRankingScore, matchingStrategy)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchApi#searchSearchGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchApi#searchSearchGet")
    e.printStackTrace()
}
```

### Parameters
| **indexUid** | **kotlin.String**| Unique index identifier | |
| **q** | **kotlin.String**| Search query | [optional] |
| **offset** | **kotlin.Int**|  | [optional] [default to 0] |
| **limit** | **kotlin.Int**|  | [optional] [default to 20] |
| **attributesToRetrieve** | **kotlin.String**| Comma-separated list of attributes to return | [optional] |
| **attributesToHighlight** | **kotlin.String**|  | [optional] |
| **attributesToCrop** | **kotlin.String**|  | [optional] |
| **cropLength** | **kotlin.Int**|  | [optional] [default to 10] |
| **filter** | **kotlin.String**| Filter expression | [optional] |
| **sort** | **kotlin.String**| Comma-separated sort rules | [optional] |
| **facets** | **kotlin.String**| Comma-separated facet attributes | [optional] |
| **showMatchesPosition** | **kotlin.Boolean**|  | [optional] |
| **showRankingScore** | **kotlin.Boolean**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **matchingStrategy** | **kotlin.String**|  | [optional] [enum: last, all, frequency] |

### Return type

[**SearchSearchResult**](SearchSearchResult.md)

### Authorization


Configure bearerAuth statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearerAuth dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="searchSearchPost"></a>
# **searchSearchPost**
> SearchSearchResult searchSearchPost(indexUid, searchSearchQuery)

Search documents (POST)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SearchApi()
val indexUid : kotlin.String = indexUid_example // kotlin.String | Unique index identifier
val searchSearchQuery : SearchSearchQuery =  // SearchSearchQuery | 
try {
    val result : SearchSearchResult = apiInstance.searchSearchPost(indexUid, searchSearchQuery)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchApi#searchSearchPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchApi#searchSearchPost")
    e.printStackTrace()
}
```

### Parameters
| **indexUid** | **kotlin.String**| Unique index identifier | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **searchSearchQuery** | [**SearchSearchQuery**](SearchSearchQuery.md)|  | |

### Return type

[**SearchSearchResult**](SearchSearchResult.md)

### Authorization


Configure bearerAuth statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearerAuth dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="vectorRecommendPoints"></a>
# **vectorRecommendPoints**
> VectorRecommendPoints200Response vectorRecommendPoints(collectionName, vectorRecommendPointsRequest)

Recommend points

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SearchApi()
val collectionName : kotlin.String = collectionName_example // kotlin.String | 
val vectorRecommendPointsRequest : VectorRecommendPointsRequest =  // VectorRecommendPointsRequest | 
try {
    val result : VectorRecommendPoints200Response = apiInstance.vectorRecommendPoints(collectionName, vectorRecommendPointsRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchApi#vectorRecommendPoints")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchApi#vectorRecommendPoints")
    e.printStackTrace()
}
```

### Parameters
| **collectionName** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **vectorRecommendPointsRequest** | [**VectorRecommendPointsRequest**](VectorRecommendPointsRequest.md)|  | |

### Return type

[**VectorRecommendPoints200Response**](VectorRecommendPoints200Response.md)

### Authorization


Configure bearerAuth statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearerAuth dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="vectorSearchBatch"></a>
# **vectorSearchBatch**
> VectorSearchBatch200Response vectorSearchBatch(collectionName, vectorSearchBatchRequest)

Batch search

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SearchApi()
val collectionName : kotlin.String = collectionName_example // kotlin.String | 
val vectorSearchBatchRequest : VectorSearchBatchRequest =  // VectorSearchBatchRequest | 
try {
    val result : VectorSearchBatch200Response = apiInstance.vectorSearchBatch(collectionName, vectorSearchBatchRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchApi#vectorSearchBatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchApi#vectorSearchBatch")
    e.printStackTrace()
}
```

### Parameters
| **collectionName** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **vectorSearchBatchRequest** | [**VectorSearchBatchRequest**](VectorSearchBatchRequest.md)|  | |

### Return type

[**VectorSearchBatch200Response**](VectorSearchBatch200Response.md)

### Authorization


Configure bearerAuth statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearerAuth dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="vectorSearchPoints"></a>
# **vectorSearchPoints**
> VectorRecommendPoints200Response vectorSearchPoints(collectionName, vectorSearchRequest)

Search points

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SearchApi()
val collectionName : kotlin.String = collectionName_example // kotlin.String | 
val vectorSearchRequest : VectorSearchRequest =  // VectorSearchRequest | 
try {
    val result : VectorRecommendPoints200Response = apiInstance.vectorSearchPoints(collectionName, vectorSearchRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchApi#vectorSearchPoints")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchApi#vectorSearchPoints")
    e.printStackTrace()
}
```

### Parameters
| **collectionName** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **vectorSearchRequest** | [**VectorSearchRequest**](VectorSearchRequest.md)|  | |

### Return type

[**VectorRecommendPoints200Response**](VectorRecommendPoints200Response.md)

### Authorization


Configure bearerAuth statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearerAuth dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="websearchWebSearch"></a>
# **websearchWebSearch**
> WebsearchSearchResponse websearchWebSearch(q, format)

Search the web (SearXNG JSON contract, proxied verbatim)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SearchApi()
val q : kotlin.String = q_example // kotlin.String | Search query
val format : kotlin.String = format_example // kotlin.String | 
try {
    val result : WebsearchSearchResponse = apiInstance.websearchWebSearch(q, format)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchApi#websearchWebSearch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchApi#websearchWebSearch")
    e.printStackTrace()
}
```

### Parameters
| **q** | **kotlin.String**| Search query | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **format** | **kotlin.String**|  | [optional] [default to Format.json] [enum: json] |

### Return type

[**WebsearchSearchResponse**](WebsearchSearchResponse.md)

### Authorization


Configure serviceKey:
    ApiClient.apiKey["X-API-Key"] = ""
    ApiClient.apiKeyPrefix["X-API-Key"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

