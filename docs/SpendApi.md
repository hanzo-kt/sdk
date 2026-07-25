# SpendApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**gatewayCalculateSpend**](SpendApi.md#gatewayCalculateSpend) | **POST** /v1/gateway/spend/calculate | Calculate spend for request |
| [**gatewayGetSpendLogs**](SpendApi.md#gatewayGetSpendLogs) | **GET** /v1/gateway/spend/logs | Get spend logs |


<a id="gatewayCalculateSpend"></a>
# **gatewayCalculateSpend**
> GatewayCalculateSpend200Response gatewayCalculateSpend(gatewayCalculateSpendRequest)

Calculate spend for request

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SpendApi()
val gatewayCalculateSpendRequest : GatewayCalculateSpendRequest =  // GatewayCalculateSpendRequest | 
try {
    val result : GatewayCalculateSpend200Response = apiInstance.gatewayCalculateSpend(gatewayCalculateSpendRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SpendApi#gatewayCalculateSpend")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SpendApi#gatewayCalculateSpend")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **gatewayCalculateSpendRequest** | [**GatewayCalculateSpendRequest**](GatewayCalculateSpendRequest.md)|  | |

### Return type

[**GatewayCalculateSpend200Response**](GatewayCalculateSpend200Response.md)

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

<a id="gatewayGetSpendLogs"></a>
# **gatewayGetSpendLogs**
> kotlin.collections.List&lt;GatewayGetSpendLogs200ResponseInner&gt; gatewayGetSpendLogs(userId, teamId, startDate, endDate)

Get spend logs

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SpendApi()
val userId : kotlin.String = userId_example // kotlin.String | 
val teamId : kotlin.String = teamId_example // kotlin.String | 
val startDate : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | 
val endDate : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | 
try {
    val result : kotlin.collections.List<GatewayGetSpendLogs200ResponseInner> = apiInstance.gatewayGetSpendLogs(userId, teamId, startDate, endDate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SpendApi#gatewayGetSpendLogs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SpendApi#gatewayGetSpendLogs")
    e.printStackTrace()
}
```

### Parameters
| **userId** | **kotlin.String**|  | [optional] |
| **teamId** | **kotlin.String**|  | [optional] |
| **startDate** | **java.time.LocalDate**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **endDate** | **java.time.LocalDate**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;GatewayGetSpendLogs200ResponseInner&gt;**](GatewayGetSpendLogs200ResponseInner.md)

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

