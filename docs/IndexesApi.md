# IndexesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**searchCreateIndex**](IndexesApi.md#searchCreateIndex) | **POST** /v1/search/indexes | Create a new index |
| [**searchDeleteIndex**](IndexesApi.md#searchDeleteIndex) | **DELETE** /v1/search/indexes/{indexUid} | Delete an index |
| [**searchGetIndex**](IndexesApi.md#searchGetIndex) | **GET** /v1/search/indexes/{indexUid} | Get index information |
| [**searchListIndexes**](IndexesApi.md#searchListIndexes) | **GET** /v1/search/indexes | List all indexes |
| [**searchUpdateIndex**](IndexesApi.md#searchUpdateIndex) | **PATCH** /v1/search/indexes/{indexUid} | Update index (primary key) |


<a id="searchCreateIndex"></a>
# **searchCreateIndex**
> SearchSummarizedTaskView searchCreateIndex(searchIndexCreateRequest)

Create a new index

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IndexesApi()
val searchIndexCreateRequest : SearchIndexCreateRequest =  // SearchIndexCreateRequest | 
try {
    val result : SearchSummarizedTaskView = apiInstance.searchCreateIndex(searchIndexCreateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IndexesApi#searchCreateIndex")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IndexesApi#searchCreateIndex")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **searchIndexCreateRequest** | [**SearchIndexCreateRequest**](SearchIndexCreateRequest.md)|  | |

### Return type

[**SearchSummarizedTaskView**](SearchSummarizedTaskView.md)

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

<a id="searchDeleteIndex"></a>
# **searchDeleteIndex**
> SearchSummarizedTaskView searchDeleteIndex(indexUid)

Delete an index

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IndexesApi()
val indexUid : kotlin.String = indexUid_example // kotlin.String | Unique index identifier
try {
    val result : SearchSummarizedTaskView = apiInstance.searchDeleteIndex(indexUid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IndexesApi#searchDeleteIndex")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IndexesApi#searchDeleteIndex")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **indexUid** | **kotlin.String**| Unique index identifier | |

### Return type

[**SearchSummarizedTaskView**](SearchSummarizedTaskView.md)

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

<a id="searchGetIndex"></a>
# **searchGetIndex**
> SearchIndexView searchGetIndex(indexUid)

Get index information

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IndexesApi()
val indexUid : kotlin.String = indexUid_example // kotlin.String | Unique index identifier
try {
    val result : SearchIndexView = apiInstance.searchGetIndex(indexUid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IndexesApi#searchGetIndex")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IndexesApi#searchGetIndex")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **indexUid** | **kotlin.String**| Unique index identifier | |

### Return type

[**SearchIndexView**](SearchIndexView.md)

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

<a id="searchListIndexes"></a>
# **searchListIndexes**
> SearchPaginatedIndexes searchListIndexes(offset, limit)

List all indexes

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IndexesApi()
val offset : kotlin.Int = 56 // kotlin.Int | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : SearchPaginatedIndexes = apiInstance.searchListIndexes(offset, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IndexesApi#searchListIndexes")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IndexesApi#searchListIndexes")
    e.printStackTrace()
}
```

### Parameters
| **offset** | **kotlin.Int**|  | [optional] [default to 0] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] [default to 20] |

### Return type

[**SearchPaginatedIndexes**](SearchPaginatedIndexes.md)

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

<a id="searchUpdateIndex"></a>
# **searchUpdateIndex**
> SearchSummarizedTaskView searchUpdateIndex(indexUid, searchUpdateIndexRequest)

Update index (primary key)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IndexesApi()
val indexUid : kotlin.String = indexUid_example // kotlin.String | Unique index identifier
val searchUpdateIndexRequest : SearchUpdateIndexRequest =  // SearchUpdateIndexRequest | 
try {
    val result : SearchSummarizedTaskView = apiInstance.searchUpdateIndex(indexUid, searchUpdateIndexRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IndexesApi#searchUpdateIndex")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IndexesApi#searchUpdateIndex")
    e.printStackTrace()
}
```

### Parameters
| **indexUid** | **kotlin.String**| Unique index identifier | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **searchUpdateIndexRequest** | [**SearchUpdateIndexRequest**](SearchUpdateIndexRequest.md)|  | |

### Return type

[**SearchSummarizedTaskView**](SearchSummarizedTaskView.md)

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

