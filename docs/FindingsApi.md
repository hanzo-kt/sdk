# FindingsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**securitySecurityGetFinding**](FindingsApi.md#securitySecurityGetFinding) | **GET** /v1/security/findings/{id} | Get a finding |
| [**securitySecurityListFindings**](FindingsApi.md#securitySecurityListFindings) | **GET** /v1/security/findings | List findings |


<a id="securitySecurityGetFinding"></a>
# **securitySecurityGetFinding**
> SecurityFinding securitySecurityGetFinding(id)

Get a finding

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FindingsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : SecurityFinding = apiInstance.securitySecurityGetFinding(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FindingsApi#securitySecurityGetFinding")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FindingsApi#securitySecurityGetFinding")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**SecurityFinding**](SecurityFinding.md)

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

<a id="securitySecurityListFindings"></a>
# **securitySecurityListFindings**
> SecuritySecurityListFindings200Response securitySecurityListFindings(scanId, minSeverity, limit)

List findings

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FindingsApi()
val scanId : kotlin.String = scanId_example // kotlin.String | 
val minSeverity : kotlin.String = minSeverity_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : SecuritySecurityListFindings200Response = apiInstance.securitySecurityListFindings(scanId, minSeverity, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FindingsApi#securitySecurityListFindings")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FindingsApi#securitySecurityListFindings")
    e.printStackTrace()
}
```

### Parameters
| **scanId** | **kotlin.String**|  | [optional] |
| **minSeverity** | **kotlin.String**|  | [optional] [enum: critical, high, medium, low] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] |

### Return type

[**SecuritySecurityListFindings200Response**](SecuritySecurityListFindings200Response.md)

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

