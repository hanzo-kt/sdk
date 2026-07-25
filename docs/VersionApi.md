# VersionApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**searchGetVersion**](VersionApi.md#searchGetVersion) | **GET** /v1/search/version | Get server version |


<a id="searchGetVersion"></a>
# **searchGetVersion**
> SearchVersionResponse searchGetVersion()

Get server version

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VersionApi()
try {
    val result : SearchVersionResponse = apiInstance.searchGetVersion()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VersionApi#searchGetVersion")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VersionApi#searchGetVersion")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**SearchVersionResponse**](SearchVersionResponse.md)

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

