# ZonesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**dnsCreateZone**](ZonesApi.md#dnsCreateZone) | **POST** /v1/dns/zones | Create zone |
| [**dnsDeleteZone**](ZonesApi.md#dnsDeleteZone) | **DELETE** /v1/dns/zones/{zone} | Delete zone |
| [**dnsExportZone**](ZonesApi.md#dnsExportZone) | **GET** /v1/dns/zones/{zone}/export | Export zone file |
| [**dnsGetZone**](ZonesApi.md#dnsGetZone) | **GET** /v1/dns/zones/{zone} | Get zone |
| [**dnsImportZone**](ZonesApi.md#dnsImportZone) | **POST** /v1/dns/zones/{zone}/import | Import zone file |
| [**dnsListZones**](ZonesApi.md#dnsListZones) | **GET** /v1/dns/zones | List zones |
| [**dnsUpdateZone**](ZonesApi.md#dnsUpdateZone) | **PUT** /v1/dns/zones/{zone} | Update zone |


<a id="dnsCreateZone"></a>
# **dnsCreateZone**
> DnsZone dnsCreateZone(dnsZoneCreate)

Create zone

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ZonesApi()
val dnsZoneCreate : DnsZoneCreate =  // DnsZoneCreate | 
try {
    val result : DnsZone = apiInstance.dnsCreateZone(dnsZoneCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ZonesApi#dnsCreateZone")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ZonesApi#dnsCreateZone")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **dnsZoneCreate** | [**DnsZoneCreate**](DnsZoneCreate.md)|  | |

### Return type

[**DnsZone**](DnsZone.md)

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

<a id="dnsDeleteZone"></a>
# **dnsDeleteZone**
> kotlin.Any dnsDeleteZone(zone)

Delete zone

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ZonesApi()
val zone : kotlin.String = zone_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.dnsDeleteZone(zone)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ZonesApi#dnsDeleteZone")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ZonesApi#dnsDeleteZone")
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

<a id="dnsExportZone"></a>
# **dnsExportZone**
> kotlin.String dnsExportZone(zone)

Export zone file

Export zone as a BIND-format zone file.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ZonesApi()
val zone : kotlin.String = zone_example // kotlin.String | 
try {
    val result : kotlin.String = apiInstance.dnsExportZone(zone)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ZonesApi#dnsExportZone")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ZonesApi#dnsExportZone")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **zone** | **kotlin.String**|  | |

### Return type

**kotlin.String**

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
 - **Accept**: text/plain, application/json

<a id="dnsGetZone"></a>
# **dnsGetZone**
> DnsZone dnsGetZone(zone)

Get zone

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ZonesApi()
val zone : kotlin.String = zone_example // kotlin.String | 
try {
    val result : DnsZone = apiInstance.dnsGetZone(zone)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ZonesApi#dnsGetZone")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ZonesApi#dnsGetZone")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **zone** | **kotlin.String**|  | |

### Return type

[**DnsZone**](DnsZone.md)

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

<a id="dnsImportZone"></a>
# **dnsImportZone**
> DnsImportZone200Response dnsImportZone(zone, body)

Import zone file

Import DNS records from a BIND-format zone file.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ZonesApi()
val zone : kotlin.String = zone_example // kotlin.String | 
val body : kotlin.String = body_example // kotlin.String | 
try {
    val result : DnsImportZone200Response = apiInstance.dnsImportZone(zone, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ZonesApi#dnsImportZone")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ZonesApi#dnsImportZone")
    e.printStackTrace()
}
```

### Parameters
| **zone** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.String**|  | |

### Return type

[**DnsImportZone200Response**](DnsImportZone200Response.md)

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

 - **Content-Type**: text/plain
 - **Accept**: application/json

<a id="dnsListZones"></a>
# **dnsListZones**
> DnsListZones200Response dnsListZones(status, name, page, pageSize)

List zones

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ZonesApi()
val status : kotlin.String = status_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | Filter by zone name (substring match)
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : DnsListZones200Response = apiInstance.dnsListZones(status, name, page, pageSize)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ZonesApi#dnsListZones")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ZonesApi#dnsListZones")
    e.printStackTrace()
}
```

### Parameters
| **status** | **kotlin.String**|  | [optional] [enum: active, pending, disabled] |
| **name** | **kotlin.String**| Filter by zone name (substring match) | [optional] |
| **page** | **kotlin.Int**|  | [optional] [default to 1] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **pageSize** | **kotlin.Int**|  | [optional] [default to 20] |

### Return type

[**DnsListZones200Response**](DnsListZones200Response.md)

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

<a id="dnsUpdateZone"></a>
# **dnsUpdateZone**
> DnsZone dnsUpdateZone(zone, dnsUpdateZoneRequest)

Update zone

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ZonesApi()
val zone : kotlin.String = zone_example // kotlin.String | 
val dnsUpdateZoneRequest : DnsUpdateZoneRequest =  // DnsUpdateZoneRequest | 
try {
    val result : DnsZone = apiInstance.dnsUpdateZone(zone, dnsUpdateZoneRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ZonesApi#dnsUpdateZone")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ZonesApi#dnsUpdateZone")
    e.printStackTrace()
}
```

### Parameters
| **zone** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **dnsUpdateZoneRequest** | [**DnsUpdateZoneRequest**](DnsUpdateZoneRequest.md)|  | |

### Return type

[**DnsZone**](DnsZone.md)

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

