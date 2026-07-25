# ObservabilityApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**adminAdminCompute**](ObservabilityApi.md#adminAdminCompute) | **GET** /v1/admin/compute | Cross-tenant compute analytics |
| [**adminAdminO11y**](ObservabilityApi.md#adminAdminO11y) | **GET** /v1/admin/o11y | Fleet-wide observability board |


<a id="adminAdminCompute"></a>
# **adminAdminCompute**
> AdminAdminCompute200Response adminAdminCompute(kind, org, range)

Cross-tenant compute analytics

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ObservabilityApi()
val kind : kotlin.String = kind_example // kotlin.String | bot | machine | cluster | nodepool | container | function | …
val org : kotlin.String = org_example // kotlin.String | 
val range : kotlin.String = range_example // kotlin.String | 
try {
    val result : AdminAdminCompute200Response = apiInstance.adminAdminCompute(kind, org, range)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ObservabilityApi#adminAdminCompute")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ObservabilityApi#adminAdminCompute")
    e.printStackTrace()
}
```

### Parameters
| **kind** | **kotlin.String**| bot | machine | cluster | nodepool | container | function | … | [optional] |
| **org** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **range** | **kotlin.String**|  | [optional] [default to Range._30d] [enum: 24h, 7d, 30d] |

### Return type

[**AdminAdminCompute200Response**](AdminAdminCompute200Response.md)

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

<a id="adminAdminO11y"></a>
# **adminAdminO11y**
> AdminAdminO11y200Response adminAdminO11y(range)

Fleet-wide observability board

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ObservabilityApi()
val range : kotlin.String = range_example // kotlin.String | 
try {
    val result : AdminAdminO11y200Response = apiInstance.adminAdminO11y(range)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ObservabilityApi#adminAdminO11y")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ObservabilityApi#adminAdminO11y")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **range** | **kotlin.String**|  | [optional] [default to Range._30d] [enum: 24h, 7d, 30d] |

### Return type

[**AdminAdminO11y200Response**](AdminAdminO11y200Response.md)

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

