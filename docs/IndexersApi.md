# IndexersApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**graphListIndexers**](IndexersApi.md#graphListIndexers) | **GET** /v1/indexers | List the deployment&#39;s chain indexer(s) |


<a id="graphListIndexers"></a>
# **graphListIndexers**
> GraphListIndexers200Response graphListIndexers()

List the deployment&#39;s chain indexer(s)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IndexersApi()
try {
    val result : GraphListIndexers200Response = apiInstance.graphListIndexers()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IndexersApi#graphListIndexers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IndexersApi#graphListIndexers")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**GraphListIndexers200Response**](GraphListIndexers200Response.md)

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

