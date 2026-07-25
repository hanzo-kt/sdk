# DNSApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**gatewayListDNSRecordsProxy**](DNSApi.md#gatewayListDNSRecordsProxy) | **GET** /v1/gateway/dns/zones/{zone}/records | List DNS records (proxy to dns.hanzo.ai) |
| [**gatewayListDNSZonesProxy**](DNSApi.md#gatewayListDNSZonesProxy) | **GET** /v1/gateway/dns/zones | List DNS zones (proxy to dns.hanzo.ai) |


<a id="gatewayListDNSRecordsProxy"></a>
# **gatewayListDNSRecordsProxy**
> kotlin.Any gatewayListDNSRecordsProxy(zone)

List DNS records (proxy to dns.hanzo.ai)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DNSApi()
val zone : kotlin.String = zone_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.gatewayListDNSRecordsProxy(zone)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DNSApi#gatewayListDNSRecordsProxy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DNSApi#gatewayListDNSRecordsProxy")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **zone** | **kotlin.String**|  | |

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

<a id="gatewayListDNSZonesProxy"></a>
# **gatewayListDNSZonesProxy**
> kotlin.Any gatewayListDNSZonesProxy()

List DNS zones (proxy to dns.hanzo.ai)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DNSApi()
try {
    val result : kotlin.Any = apiInstance.gatewayListDNSZonesProxy()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DNSApi#gatewayListDNSZonesProxy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DNSApi#gatewayListDNSZonesProxy")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

