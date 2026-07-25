# AnalyticsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**dnsGetZoneAnalytics**](AnalyticsApi.md#dnsGetZoneAnalytics) | **GET** /v1/dns/zones/{zone}/analytics | Get query analytics |


<a id="dnsGetZoneAnalytics"></a>
# **dnsGetZoneAnalytics**
> DnsQueryAnalytics dnsGetZoneAnalytics(zone, from, to, granularity)

Get query analytics

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AnalyticsApi()
val zone : kotlin.String = zone_example // kotlin.String | 
val from : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
val to : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
val granularity : kotlin.String = granularity_example // kotlin.String | 
try {
    val result : DnsQueryAnalytics = apiInstance.dnsGetZoneAnalytics(zone, from, to, granularity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AnalyticsApi#dnsGetZoneAnalytics")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AnalyticsApi#dnsGetZoneAnalytics")
    e.printStackTrace()
}
```

### Parameters
| **zone** | **kotlin.String**|  | |
| **from** | **java.time.OffsetDateTime**|  | [optional] |
| **to** | **java.time.OffsetDateTime**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **granularity** | **kotlin.String**|  | [optional] [default to Granularity.day] [enum: hour, day, week] |

### Return type

[**DnsQueryAnalytics**](DnsQueryAnalytics.md)

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

