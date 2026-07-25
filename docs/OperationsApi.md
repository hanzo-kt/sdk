# OperationsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**dbListOperations**](OperationsApi.md#dbListOperations) | **GET** /v1/db/projects/{id}/operations | List operations |


<a id="dbListOperations"></a>
# **dbListOperations**
> DbListOperations200Response dbListOperations(id, cursor, limit)

List operations

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OperationsApi()
val id : kotlin.String = id_example // kotlin.String | 
val cursor : kotlin.String = cursor_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : DbListOperations200Response = apiInstance.dbListOperations(id, cursor, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OperationsApi#dbListOperations")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OperationsApi#dbListOperations")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| **cursor** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] [default to 10] |

### Return type

[**DbListOperations200Response**](DbListOperations200Response.md)

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

