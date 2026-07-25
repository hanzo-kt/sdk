# SimilarApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**searchFindSimilar**](SimilarApi.md#searchFindSimilar) | **POST** /v1/search/indexes/{indexUid}/similar | Find similar documents |


<a id="searchFindSimilar"></a>
# **searchFindSimilar**
> SearchSimilarResult searchFindSimilar(indexUid, searchSimilarQuery)

Find similar documents

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SimilarApi()
val indexUid : kotlin.String = indexUid_example // kotlin.String | Unique index identifier
val searchSimilarQuery : SearchSimilarQuery =  // SearchSimilarQuery | 
try {
    val result : SearchSimilarResult = apiInstance.searchFindSimilar(indexUid, searchSimilarQuery)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SimilarApi#searchFindSimilar")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SimilarApi#searchFindSimilar")
    e.printStackTrace()
}
```

### Parameters
| **indexUid** | **kotlin.String**| Unique index identifier | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **searchSimilarQuery** | [**SearchSimilarQuery**](SearchSimilarQuery.md)|  | |

### Return type

[**SearchSimilarResult**](SearchSimilarResult.md)

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

