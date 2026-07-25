# BatchesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**searchGetBatch**](BatchesApi.md#searchGetBatch) | **GET** /v1/search/batches/{batchUid} | Get batch details |
| [**searchListBatches**](BatchesApi.md#searchListBatches) | **GET** /v1/search/batches | List task batches |


<a id="searchGetBatch"></a>
# **searchGetBatch**
> SearchBatchView searchGetBatch(batchUid)

Get batch details

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BatchesApi()
val batchUid : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : SearchBatchView = apiInstance.searchGetBatch(batchUid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BatchesApi#searchGetBatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BatchesApi#searchGetBatch")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **batchUid** | **kotlin.Int**|  | |

### Return type

[**SearchBatchView**](SearchBatchView.md)

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

<a id="searchListBatches"></a>
# **searchListBatches**
> SearchListBatches200Response searchListBatches(limit, from)

List task batches

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BatchesApi()
val limit : kotlin.Int = 56 // kotlin.Int | 
val from : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : SearchListBatches200Response = apiInstance.searchListBatches(limit, from)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BatchesApi#searchListBatches")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BatchesApi#searchListBatches")
    e.printStackTrace()
}
```

### Parameters
| **limit** | **kotlin.Int**|  | [optional] [default to 20] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **from** | **kotlin.Int**|  | [optional] |

### Return type

[**SearchListBatches200Response**](SearchListBatches200Response.md)

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

