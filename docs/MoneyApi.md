# MoneyApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**adminAdminAnalytics**](MoneyApi.md#adminAdminAnalytics) | **GET** /v1/admin/analytics | Native SaaS analytics (retention/growth/churn) |
| [**adminAdminFinance**](MoneyApi.md#adminAdminFinance) | **GET** /v1/admin/finance | COGS / gross-margin / runway dashboard |
| [**adminAdminRevenue**](MoneyApi.md#adminAdminRevenue) | **GET** /v1/admin/revenue | Fleet revenue aggregate |


<a id="adminAdminAnalytics"></a>
# **adminAdminAnalytics**
> AdminAdminAnalytics200Response adminAdminAnalytics(range)

Native SaaS analytics (retention/growth/churn)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MoneyApi()
val range : kotlin.String = range_example // kotlin.String | 
try {
    val result : AdminAdminAnalytics200Response = apiInstance.adminAdminAnalytics(range)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MoneyApi#adminAdminAnalytics")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MoneyApi#adminAdminAnalytics")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **range** | **kotlin.String**|  | [optional] [default to Range._30d] [enum: 7d, 30d, 90d, all] |

### Return type

[**AdminAdminAnalytics200Response**](AdminAdminAnalytics200Response.md)

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

<a id="adminAdminFinance"></a>
# **adminAdminFinance**
> AdminAdminFinance200Response adminAdminFinance()

COGS / gross-margin / runway dashboard

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MoneyApi()
try {
    val result : AdminAdminFinance200Response = apiInstance.adminAdminFinance()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MoneyApi#adminAdminFinance")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MoneyApi#adminAdminFinance")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AdminAdminFinance200Response**](AdminAdminFinance200Response.md)

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

<a id="adminAdminRevenue"></a>
# **adminAdminRevenue**
> AdminAdminRevenue200Response adminAdminRevenue()

Fleet revenue aggregate

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MoneyApi()
try {
    val result : AdminAdminRevenue200Response = apiInstance.adminAdminRevenue()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MoneyApi#adminAdminRevenue")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MoneyApi#adminAdminRevenue")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AdminAdminRevenue200Response**](AdminAdminRevenue200Response.md)

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

