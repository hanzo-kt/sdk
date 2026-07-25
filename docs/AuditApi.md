# AuditApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**adminAdminListAudit**](AuditApi.md#adminAdminListAudit) | **GET** /v1/admin/audit | Query the tamper-evident audit trail |
| [**adminAdminVerifyAudit**](AuditApi.md#adminAdminVerifyAudit) | **GET** /v1/admin/audit/verify | Verify audit-chain integrity |
| [**guardGetAuditLog**](AuditApi.md#guardGetAuditLog) | **GET** /v1/guard/audit | Get audit log |


<a id="adminAdminListAudit"></a>
# **adminAdminListAudit**
> AdminAdminListAudit200Response adminAdminListAudit(org, sub, action, resource, result, since, until, pageSize, p)

Query the tamper-evident audit trail

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuditApi()
val org : kotlin.String = org_example // kotlin.String | 
val sub : kotlin.String = sub_example // kotlin.String | 
val action : kotlin.String = action_example // kotlin.String | 
val resource : kotlin.String = resource_example // kotlin.String | 
val result : kotlin.String = result_example // kotlin.String | 
val since : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
val until : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val p : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : AdminAdminListAudit200Response = apiInstance.adminAdminListAudit(org, sub, action, resource, result, since, until, pageSize, p)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuditApi#adminAdminListAudit")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuditApi#adminAdminListAudit")
    e.printStackTrace()
}
```

### Parameters
| **org** | **kotlin.String**|  | [optional] |
| **sub** | **kotlin.String**|  | [optional] |
| **action** | **kotlin.String**|  | [optional] |
| **resource** | **kotlin.String**|  | [optional] |
| **result** | **kotlin.String**|  | [optional] |
| **since** | **java.time.OffsetDateTime**|  | [optional] |
| **until** | **java.time.OffsetDateTime**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] [default to 100] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **p** | **kotlin.Int**|  | [optional] [default to 1] |

### Return type

[**AdminAdminListAudit200Response**](AdminAdminListAudit200Response.md)

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

<a id="adminAdminVerifyAudit"></a>
# **adminAdminVerifyAudit**
> AdminAdminVerifyAudit200Response adminAdminVerifyAudit()

Verify audit-chain integrity

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuditApi()
try {
    val result : AdminAdminVerifyAudit200Response = apiInstance.adminAdminVerifyAudit()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuditApi#adminAdminVerifyAudit")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuditApi#adminAdminVerifyAudit")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AdminAdminVerifyAudit200Response**](AdminAdminVerifyAudit200Response.md)

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

<a id="guardGetAuditLog"></a>
# **guardGetAuditLog**
> GuardGetAuditLog200Response guardGetAuditLog(userId, sessionId, result, since, until, limit)

Get audit log

Retrieve audit log entries in JSONL format.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuditApi()
val userId : kotlin.String = userId_example // kotlin.String | Filter by user ID
val sessionId : kotlin.String = sessionId_example // kotlin.String | Filter by session ID
val result : kotlin.String = result_example // kotlin.String | Filter by result type
val since : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | Entries after this timestamp
val until : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | Entries before this timestamp
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : GuardGetAuditLog200Response = apiInstance.guardGetAuditLog(userId, sessionId, result, since, until, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuditApi#guardGetAuditLog")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuditApi#guardGetAuditLog")
    e.printStackTrace()
}
```

### Parameters
| **userId** | **kotlin.String**| Filter by user ID | [optional] |
| **sessionId** | **kotlin.String**| Filter by session ID | [optional] |
| **result** | **kotlin.String**| Filter by result type | [optional] [enum: clean, redacted, blocked] |
| **since** | **java.time.OffsetDateTime**| Entries after this timestamp | [optional] |
| **until** | **java.time.OffsetDateTime**| Entries before this timestamp | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] [default to 100] |

### Return type

[**GuardGetAuditLog200Response**](GuardGetAuditLog200Response.md)

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

