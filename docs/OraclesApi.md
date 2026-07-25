# OraclesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**graphListOracles**](OraclesApi.md#graphListOracles) | **GET** /v1/oracles | List on-chain price/data oracles |


<a id="graphListOracles"></a>
# **graphListOracles**
> GraphListOracles200Response graphListOracles()

List on-chain price/data oracles

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OraclesApi()
try {
    val result : GraphListOracles200Response = apiInstance.graphListOracles()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OraclesApi#graphListOracles")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OraclesApi#graphListOracles")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**GraphListOracles200Response**](GraphListOracles200Response.md)

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

