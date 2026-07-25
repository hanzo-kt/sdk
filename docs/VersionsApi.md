# VersionsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**edgeListFunctionVersions**](VersionsApi.md#edgeListFunctionVersions) | **GET** /v1/edge/functions/{slug}/versions | List function versions |
| [**edgeRollbackFunction**](VersionsApi.md#edgeRollbackFunction) | **POST** /v1/edge/functions/{slug}/rollback | Rollback to version |


<a id="edgeListFunctionVersions"></a>
# **edgeListFunctionVersions**
> kotlin.collections.List&lt;EdgeFunctionVersion&gt; edgeListFunctionVersions(slug)

List function versions

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VersionsApi()
val slug : kotlin.String = slug_example // kotlin.String | 
try {
    val result : kotlin.collections.List<EdgeFunctionVersion> = apiInstance.edgeListFunctionVersions(slug)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VersionsApi#edgeListFunctionVersions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VersionsApi#edgeListFunctionVersions")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **slug** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.List&lt;EdgeFunctionVersion&gt;**](EdgeFunctionVersion.md)

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

<a id="edgeRollbackFunction"></a>
# **edgeRollbackFunction**
> EdgeFunction edgeRollbackFunction(slug, edgeRollbackFunctionRequest)

Rollback to version

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VersionsApi()
val slug : kotlin.String = slug_example // kotlin.String | 
val edgeRollbackFunctionRequest : EdgeRollbackFunctionRequest =  // EdgeRollbackFunctionRequest | 
try {
    val result : EdgeFunction = apiInstance.edgeRollbackFunction(slug, edgeRollbackFunctionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VersionsApi#edgeRollbackFunction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VersionsApi#edgeRollbackFunction")
    e.printStackTrace()
}
```

### Parameters
| **slug** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **edgeRollbackFunctionRequest** | [**EdgeRollbackFunctionRequest**](EdgeRollbackFunctionRequest.md)|  | |

### Return type

[**EdgeFunction**](EdgeFunction.md)

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

