# DNSSECApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**dnsDisableDnssec**](DNSSECApi.md#dnsDisableDnssec) | **DELETE** /v1/dns/zones/{zone}/dnssec | Disable DNSSEC |
| [**dnsEnableDnssec**](DNSSECApi.md#dnsEnableDnssec) | **POST** /v1/dns/zones/{zone}/dnssec/enable | Enable DNSSEC |
| [**dnsGetDnssecStatus**](DNSSECApi.md#dnsGetDnssecStatus) | **GET** /v1/dns/zones/{zone}/dnssec | Get DNSSEC status |


<a id="dnsDisableDnssec"></a>
# **dnsDisableDnssec**
> kotlin.Any dnsDisableDnssec(zone)

Disable DNSSEC

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DNSSECApi()
val zone : kotlin.String = zone_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.dnsDisableDnssec(zone)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DNSSECApi#dnsDisableDnssec")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DNSSECApi#dnsDisableDnssec")
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

<a id="dnsEnableDnssec"></a>
# **dnsEnableDnssec**
> DnsDNSSECStatus dnsEnableDnssec(zone)

Enable DNSSEC

Enables DNSSEC signing for the zone. Returns the DS record that must be added at the domain registrar. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DNSSECApi()
val zone : kotlin.String = zone_example // kotlin.String | 
try {
    val result : DnsDNSSECStatus = apiInstance.dnsEnableDnssec(zone)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DNSSECApi#dnsEnableDnssec")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DNSSECApi#dnsEnableDnssec")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **zone** | **kotlin.String**|  | |

### Return type

[**DnsDNSSECStatus**](DnsDNSSECStatus.md)

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

<a id="dnsGetDnssecStatus"></a>
# **dnsGetDnssecStatus**
> DnsDNSSECStatus dnsGetDnssecStatus(zone)

Get DNSSEC status

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DNSSECApi()
val zone : kotlin.String = zone_example // kotlin.String | 
try {
    val result : DnsDNSSECStatus = apiInstance.dnsGetDnssecStatus(zone)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DNSSECApi#dnsGetDnssecStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DNSSECApi#dnsGetDnssecStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **zone** | **kotlin.String**|  | |

### Return type

[**DnsDNSSECStatus**](DnsDNSSECStatus.md)

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

