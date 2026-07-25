# MultiSearchApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**searchMultiSearch**](MultiSearchApi.md#searchMultiSearch) | **POST** /v1/search/multi-search | Perform a multi-index search |


<a id="searchMultiSearch"></a>
# **searchMultiSearch**
> SearchMultiSearch200Response searchMultiSearch(searchFederatedSearch)

Perform a multi-index search

Bundle multiple search queries in a single request. Supports both independent per-index results and federated (merged) results. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MultiSearchApi()
val searchFederatedSearch : SearchFederatedSearch =  // SearchFederatedSearch | 
try {
    val result : SearchMultiSearch200Response = apiInstance.searchMultiSearch(searchFederatedSearch)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MultiSearchApi#searchMultiSearch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MultiSearchApi#searchMultiSearch")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **searchFederatedSearch** | [**SearchFederatedSearch**](SearchFederatedSearch.md)|  | |

### Return type

[**SearchMultiSearch200Response**](SearchMultiSearch200Response.md)

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

