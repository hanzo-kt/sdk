# ConsumptionApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**dbGetConsumption**](ConsumptionApi.md#dbGetConsumption) | **GET** /v1/db/consumption | Get usage metrics |


<a id="dbGetConsumption"></a>
# **dbGetConsumption**
> DbGetConsumption200Response dbGetConsumption(from, to, projectId, granularity)

Get usage metrics

Returns compute, storage, and data transfer usage metrics. Used for billing calculations. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConsumptionApi()
val from : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
val to : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
val projectId : kotlin.String = projectId_example // kotlin.String | Filter by project (omit for all projects)
val granularity : kotlin.String = granularity_example // kotlin.String | 
try {
    val result : DbGetConsumption200Response = apiInstance.dbGetConsumption(from, to, projectId, granularity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConsumptionApi#dbGetConsumption")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConsumptionApi#dbGetConsumption")
    e.printStackTrace()
}
```

### Parameters
| **from** | **java.time.OffsetDateTime**|  | |
| **to** | **java.time.OffsetDateTime**|  | |
| **projectId** | **kotlin.String**| Filter by project (omit for all projects) | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **granularity** | **kotlin.String**|  | [optional] [default to Granularity.hourly] [enum: hourly, daily, monthly] |

### Return type

[**DbGetConsumption200Response**](DbGetConsumption200Response.md)

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

