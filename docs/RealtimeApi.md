# RealtimeApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**analyticsGetRealtimeData**](RealtimeApi.md#analyticsGetRealtimeData) | **GET** /v1/analytics/realtime/{websiteId} | Get realtime visitor data for the last 30 minutes |


<a id="analyticsGetRealtimeData"></a>
# **analyticsGetRealtimeData**
> kotlin.Any analyticsGetRealtimeData(websiteId, timezone)

Get realtime visitor data for the last 30 minutes

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RealtimeApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val timezone : kotlin.String = America/Los_Angeles // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.analyticsGetRealtimeData(websiteId, timezone)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RealtimeApi#analyticsGetRealtimeData")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RealtimeApi#analyticsGetRealtimeData")
    e.printStackTrace()
}
```

### Parameters
| **websiteId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **timezone** | **kotlin.String**|  | [optional] |

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

