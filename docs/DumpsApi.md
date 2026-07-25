# DumpsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**searchCreateDump**](DumpsApi.md#searchCreateDump) | **POST** /v1/search/dumps | Create a database dump |


<a id="searchCreateDump"></a>
# **searchCreateDump**
> SearchSummarizedTaskView searchCreateDump()

Create a database dump

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DumpsApi()
try {
    val result : SearchSummarizedTaskView = apiInstance.searchCreateDump()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DumpsApi#searchCreateDump")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DumpsApi#searchCreateDump")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

