# GeoApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**worldWorldAisSnapshot**](GeoApi.md#worldWorldAisSnapshot) | **GET** /v1/world/ais-snapshot | AIS vessel snapshot (requires WS_RELAY_URL) |
| [**worldWorldClimateAnomalies**](GeoApi.md#worldWorldClimateAnomalies) | **GET** /v1/world/climate-anomalies | Climate anomaly feed |
| [**worldWorldCloudflareOutages**](GeoApi.md#worldWorldCloudflareOutages) | **GET** /v1/world/cloudflare-outages | Cloudflare internet outages |
| [**worldWorldEarthquakes**](GeoApi.md#worldWorldEarthquakes) | **GET** /v1/world/earthquakes | USGS earthquake feed |
| [**worldWorldFaaStatus**](GeoApi.md#worldWorldFaaStatus) | **GET** /v1/world/faa-status | FAA airport status |
| [**worldWorldFirmsFires**](GeoApi.md#worldWorldFirmsFires) | **GET** /v1/world/firms-fires | NASA FIRMS active fires (requires NASA_FIRMS_API_KEY) |
| [**worldWorldNgaWarnings**](GeoApi.md#worldWorldNgaWarnings) | **GET** /v1/world/nga-warnings | NGA maritime safety warnings |
| [**worldWorldOpensky**](GeoApi.md#worldWorldOpensky) | **GET** /v1/world/opensky | OpenSky flight states |
| [**worldWorldWingbits**](GeoApi.md#worldWorldWingbits) | **GET** /v1/world/wingbits | Wingbits ADS-B (requires WINGBITS_API_KEY) |
| [**worldWorldWorldpopExposure**](GeoApi.md#worldWorldWorldpopExposure) | **GET** /v1/world/worldpop-exposure | Population exposure model |


<a id="worldWorldAisSnapshot"></a>
# **worldWorldAisSnapshot**
> kotlin.Any worldWorldAisSnapshot()

AIS vessel snapshot (requires WS_RELAY_URL)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GeoApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldAisSnapshot()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GeoApi#worldWorldAisSnapshot")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GeoApi#worldWorldAisSnapshot")
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

<a id="worldWorldClimateAnomalies"></a>
# **worldWorldClimateAnomalies**
> kotlin.Any worldWorldClimateAnomalies()

Climate anomaly feed

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GeoApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldClimateAnomalies()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GeoApi#worldWorldClimateAnomalies")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GeoApi#worldWorldClimateAnomalies")
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

<a id="worldWorldCloudflareOutages"></a>
# **worldWorldCloudflareOutages**
> kotlin.Any worldWorldCloudflareOutages()

Cloudflare internet outages

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GeoApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldCloudflareOutages()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GeoApi#worldWorldCloudflareOutages")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GeoApi#worldWorldCloudflareOutages")
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

<a id="worldWorldEarthquakes"></a>
# **worldWorldEarthquakes**
> kotlin.Any worldWorldEarthquakes()

USGS earthquake feed

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GeoApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldEarthquakes()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GeoApi#worldWorldEarthquakes")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GeoApi#worldWorldEarthquakes")
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

<a id="worldWorldFaaStatus"></a>
# **worldWorldFaaStatus**
> kotlin.Any worldWorldFaaStatus()

FAA airport status

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GeoApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldFaaStatus()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GeoApi#worldWorldFaaStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GeoApi#worldWorldFaaStatus")
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

<a id="worldWorldFirmsFires"></a>
# **worldWorldFirmsFires**
> kotlin.Any worldWorldFirmsFires()

NASA FIRMS active fires (requires NASA_FIRMS_API_KEY)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GeoApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldFirmsFires()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GeoApi#worldWorldFirmsFires")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GeoApi#worldWorldFirmsFires")
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

<a id="worldWorldNgaWarnings"></a>
# **worldWorldNgaWarnings**
> kotlin.Any worldWorldNgaWarnings()

NGA maritime safety warnings

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GeoApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldNgaWarnings()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GeoApi#worldWorldNgaWarnings")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GeoApi#worldWorldNgaWarnings")
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

<a id="worldWorldOpensky"></a>
# **worldWorldOpensky**
> kotlin.Any worldWorldOpensky()

OpenSky flight states

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GeoApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldOpensky()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GeoApi#worldWorldOpensky")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GeoApi#worldWorldOpensky")
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

<a id="worldWorldWingbits"></a>
# **worldWorldWingbits**
> kotlin.Any worldWorldWingbits()

Wingbits ADS-B (requires WINGBITS_API_KEY)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GeoApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldWingbits()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GeoApi#worldWorldWingbits")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GeoApi#worldWorldWingbits")
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

<a id="worldWorldWorldpopExposure"></a>
# **worldWorldWorldpopExposure**
> kotlin.Any worldWorldWorldpopExposure(area)

Population exposure model

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GeoApi()
val area : kotlin.String = area_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.worldWorldWorldpopExposure(area)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GeoApi#worldWorldWorldpopExposure")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GeoApi#worldWorldWorldpopExposure")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **area** | **kotlin.String**|  | [optional] |

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

