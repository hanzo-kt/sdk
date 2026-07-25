# CDNApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**gatewayGetCDNAnalytics**](CDNApi.md#gatewayGetCDNAnalytics) | **GET** /v1/gateway/cdn/analytics | CDN cache analytics |
| [**gatewayPurgeCDNCache**](CDNApi.md#gatewayPurgeCDNCache) | **POST** /v1/gateway/cdn/purge | Purge CDN cache |


<a id="gatewayGetCDNAnalytics"></a>
# **gatewayGetCDNAnalytics**
> GatewayGetCDNAnalytics200Response gatewayGetCDNAnalytics(startDate, endDate, granularity)

CDN cache analytics

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CDNApi()
val startDate : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | 
val endDate : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | 
val granularity : kotlin.String = granularity_example // kotlin.String | 
try {
    val result : GatewayGetCDNAnalytics200Response = apiInstance.gatewayGetCDNAnalytics(startDate, endDate, granularity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CDNApi#gatewayGetCDNAnalytics")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CDNApi#gatewayGetCDNAnalytics")
    e.printStackTrace()
}
```

### Parameters
| **startDate** | **java.time.LocalDate**|  | [optional] |
| **endDate** | **java.time.LocalDate**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **granularity** | **kotlin.String**|  | [optional] [default to Granularity.hour] [enum: minute, hour, day] |

### Return type

[**GatewayGetCDNAnalytics200Response**](GatewayGetCDNAnalytics200Response.md)

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

<a id="gatewayPurgeCDNCache"></a>
# **gatewayPurgeCDNCache**
> GatewayPurgeCDNCache200Response gatewayPurgeCDNCache(gatewayCDNPurgeRequest)

Purge CDN cache

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CDNApi()
val gatewayCDNPurgeRequest : GatewayCDNPurgeRequest =  // GatewayCDNPurgeRequest | 
try {
    val result : GatewayPurgeCDNCache200Response = apiInstance.gatewayPurgeCDNCache(gatewayCDNPurgeRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CDNApi#gatewayPurgeCDNCache")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CDNApi#gatewayPurgeCDNCache")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **gatewayCDNPurgeRequest** | [**GatewayCDNPurgeRequest**](GatewayCDNPurgeRequest.md)|  | |

### Return type

[**GatewayPurgeCDNCache200Response**](GatewayPurgeCDNCache200Response.md)

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

