# AuditEventsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoListAuditEvents**](AuditEventsApi.md#autoListAuditEvents) | **GET** /v1/auto/audit-events | List audit log events (EE) |
| [**flowListAuditEvents**](AuditEventsApi.md#flowListAuditEvents) | **GET** /v1/flow/audit-events | List audit log events (EE) |


<a id="autoListAuditEvents"></a>
# **autoListAuditEvents**
> kotlin.Any autoListAuditEvents(cursor, limit)

List audit log events (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuditEventsApi()
val cursor : kotlin.String = cursor_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : kotlin.Any = apiInstance.autoListAuditEvents(cursor, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuditEventsApi#autoListAuditEvents")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuditEventsApi#autoListAuditEvents")
    e.printStackTrace()
}
```

### Parameters
| **cursor** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] |

### Return type

[**kotlin.Any**](kotlin.Any.md)

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

<a id="flowListAuditEvents"></a>
# **flowListAuditEvents**
> kotlin.Any flowListAuditEvents(cursor, limit)

List audit log events (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuditEventsApi()
val cursor : kotlin.String = cursor_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : kotlin.Any = apiInstance.flowListAuditEvents(cursor, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuditEventsApi#flowListAuditEvents")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuditEventsApi#flowListAuditEvents")
    e.printStackTrace()
}
```

### Parameters
| **cursor** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] |

### Return type

[**kotlin.Any**](kotlin.Any.md)

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

