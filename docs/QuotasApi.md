# QuotasApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**registryListQuotas**](QuotasApi.md#registryListQuotas) | **GET** /v1/registry/quotas | List storage quotas |


<a id="registryListQuotas"></a>
# **registryListQuotas**
> kotlin.collections.List&lt;RegistryQuota&gt; registryListQuotas(page, pageSize, sort)

List storage quotas

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = QuotasApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val sort : kotlin.String = sort_example // kotlin.String | 
try {
    val result : kotlin.collections.List<RegistryQuota> = apiInstance.registryListQuotas(page, pageSize, sort)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling QuotasApi#registryListQuotas")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling QuotasApi#registryListQuotas")
    e.printStackTrace()
}
```

### Parameters
| **page** | **kotlin.Int**|  | [optional] [default to 1] |
| **pageSize** | **kotlin.Int**|  | [optional] [default to 10] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sort** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;RegistryQuota&gt;**](RegistryQuota.md)

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

