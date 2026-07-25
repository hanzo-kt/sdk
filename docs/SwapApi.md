# SwapApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**searchSwapIndexes**](SwapApi.md#searchSwapIndexes) | **POST** /v1/search/swap-indexes | Swap two index identifiers |


<a id="searchSwapIndexes"></a>
# **searchSwapIndexes**
> SearchSummarizedTaskView searchSwapIndexes(searchSwapIndexesRequestInner)

Swap two index identifiers

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SwapApi()
val searchSwapIndexesRequestInner : kotlin.collections.List<SearchSwapIndexesRequestInner> =  // kotlin.collections.List<SearchSwapIndexesRequestInner> | 
try {
    val result : SearchSummarizedTaskView = apiInstance.searchSwapIndexes(searchSwapIndexesRequestInner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SwapApi#searchSwapIndexes")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SwapApi#searchSwapIndexes")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **searchSwapIndexesRequestInner** | [**kotlin.collections.List&lt;SearchSwapIndexesRequestInner&gt;**](SearchSwapIndexesRequestInner.md)|  | |

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

