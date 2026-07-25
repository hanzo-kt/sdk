# AuditLogsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**kmsListAuditLogs**](AuditLogsApi.md#kmsListAuditLogs) | **GET** /v1/kms/events | List audit log events |


<a id="kmsListAuditLogs"></a>
# **kmsListAuditLogs**
> KmsListAuditLogs200Response kmsListAuditLogs(workspaceId, eventType, actor, offset, limit)

List audit log events

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuditLogsApi()
val workspaceId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val eventType : kotlin.String = eventType_example // kotlin.String | 
val actor : kotlin.String = actor_example // kotlin.String | 
val offset : kotlin.Int = 56 // kotlin.Int | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : KmsListAuditLogs200Response = apiInstance.kmsListAuditLogs(workspaceId, eventType, actor, offset, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuditLogsApi#kmsListAuditLogs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuditLogsApi#kmsListAuditLogs")
    e.printStackTrace()
}
```

### Parameters
| **workspaceId** | **java.util.UUID**|  | [optional] |
| **eventType** | **kotlin.String**|  | [optional] |
| **actor** | **kotlin.String**|  | [optional] |
| **offset** | **kotlin.Int**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] |

### Return type

[**KmsListAuditLogs200Response**](KmsListAuditLogs200Response.md)

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

