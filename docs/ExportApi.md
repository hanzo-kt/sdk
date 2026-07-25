# ExportApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**searchExportData**](ExportApi.md#searchExportData) | **POST** /v1/search/export | Export index data |


<a id="searchExportData"></a>
# **searchExportData**
> kotlin.String searchExportData(searchExportDataRequest)

Export index data

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ExportApi()
val searchExportDataRequest : SearchExportDataRequest =  // SearchExportDataRequest | 
try {
    val result : kotlin.String = apiInstance.searchExportData(searchExportDataRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ExportApi#searchExportData")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ExportApi#searchExportData")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **searchExportDataRequest** | [**SearchExportDataRequest**](SearchExportDataRequest.md)|  | |

### Return type

**kotlin.String**

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
 - **Accept**: application/x-ndjson

