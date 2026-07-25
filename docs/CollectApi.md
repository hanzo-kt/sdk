# CollectApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**analyticsBatch**](CollectApi.md#analyticsBatch) | **POST** /v1/analytics/batch | Send a batch of events |
| [**analyticsSend**](CollectApi.md#analyticsSend) | **POST** /v1/analytics/send | Send a single event or identify payload |


<a id="analyticsBatch"></a>
# **analyticsBatch**
> AnalyticsBatch200Response analyticsBatch(analyticsSendPayload)

Send a batch of events

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CollectApi()
val analyticsSendPayload : kotlin.collections.List<AnalyticsSendPayload> =  // kotlin.collections.List<AnalyticsSendPayload> | 
try {
    val result : AnalyticsBatch200Response = apiInstance.analyticsBatch(analyticsSendPayload)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CollectApi#analyticsBatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CollectApi#analyticsBatch")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **analyticsSendPayload** | [**kotlin.collections.List&lt;AnalyticsSendPayload&gt;**](AnalyticsSendPayload.md)|  | |

### Return type

[**AnalyticsBatch200Response**](AnalyticsBatch200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="analyticsSend"></a>
# **analyticsSend**
> AnalyticsSend200Response analyticsSend(analyticsSendPayload)

Send a single event or identify payload

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CollectApi()
val analyticsSendPayload : AnalyticsSendPayload =  // AnalyticsSendPayload | 
try {
    val result : AnalyticsSend200Response = apiInstance.analyticsSend(analyticsSendPayload)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CollectApi#analyticsSend")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CollectApi#analyticsSend")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **analyticsSendPayload** | [**AnalyticsSendPayload**](AnalyticsSendPayload.md)|  | |

### Return type

[**AnalyticsSend200Response**](AnalyticsSend200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

