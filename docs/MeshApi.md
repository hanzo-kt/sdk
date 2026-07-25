# MeshApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**ztListMeshServices**](MeshApi.md#ztListMeshServices) | **GET** /v1/mesh/services | List the org&#39;s ZT edge services |


<a id="ztListMeshServices"></a>
# **ztListMeshServices**
> ZtListMeshServices200Response ztListMeshServices()

List the org&#39;s ZT edge services

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MeshApi()
try {
    val result : ZtListMeshServices200Response = apiInstance.ztListMeshServices()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MeshApi#ztListMeshServices")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MeshApi#ztListMeshServices")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ZtListMeshServices200Response**](ZtListMeshServices200Response.md)

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

