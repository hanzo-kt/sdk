# MonitoringApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**pubsubGetConnz**](MonitoringApi.md#pubsubGetConnz) | **GET** /v1/pubsub/connz | Connection details |
| [**pubsubGetGatewayz**](MonitoringApi.md#pubsubGetGatewayz) | **GET** /v1/pubsub/gatewayz | Gateway status |
| [**pubsubGetJsz**](MonitoringApi.md#pubsubGetJsz) | **GET** /v1/pubsub/jsz | JetStream info |
| [**pubsubGetLeafz**](MonitoringApi.md#pubsubGetLeafz) | **GET** /v1/pubsub/leafz | Leaf node info |
| [**pubsubGetRoutez**](MonitoringApi.md#pubsubGetRoutez) | **GET** /v1/pubsub/routez | Cluster routes |
| [**pubsubGetSubsz**](MonitoringApi.md#pubsubGetSubsz) | **GET** /v1/pubsub/subsz | Subscription info |
| [**pubsubGetVarz**](MonitoringApi.md#pubsubGetVarz) | **GET** /v1/pubsub/varz | Server statistics |


<a id="pubsubGetConnz"></a>
# **pubsubGetConnz**
> PubsubGetConnz200Response pubsubGetConnz(sort, limit)

Connection details

Active client connection information.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MonitoringApi()
val sort : kotlin.String = sort_example // kotlin.String | Sort connections by field
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : PubsubGetConnz200Response = apiInstance.pubsubGetConnz(sort, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MonitoringApi#pubsubGetConnz")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MonitoringApi#pubsubGetConnz")
    e.printStackTrace()
}
```

### Parameters
| **sort** | **kotlin.String**| Sort connections by field | [optional] [enum: cid, start, subs, pending, msgs_to, msgs_from, bytes_to, bytes_from, last, idle, uptime, stop, reason] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] [default to 1024] |

### Return type

[**PubsubGetConnz200Response**](PubsubGetConnz200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="pubsubGetGatewayz"></a>
# **pubsubGetGatewayz**
> kotlin.Any pubsubGetGatewayz()

Gateway status

Super-cluster gateway connection status.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MonitoringApi()
try {
    val result : kotlin.Any = apiInstance.pubsubGetGatewayz()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MonitoringApi#pubsubGetGatewayz")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MonitoringApi#pubsubGetGatewayz")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="pubsubGetJsz"></a>
# **pubsubGetJsz**
> PubsubJetStreamInfo pubsubGetJsz()

JetStream info

JetStream account and usage information.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MonitoringApi()
try {
    val result : PubsubJetStreamInfo = apiInstance.pubsubGetJsz()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MonitoringApi#pubsubGetJsz")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MonitoringApi#pubsubGetJsz")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PubsubJetStreamInfo**](PubsubJetStreamInfo.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="pubsubGetLeafz"></a>
# **pubsubGetLeafz**
> kotlin.Any pubsubGetLeafz()

Leaf node info

Leaf node connection details.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MonitoringApi()
try {
    val result : kotlin.Any = apiInstance.pubsubGetLeafz()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MonitoringApi#pubsubGetLeafz")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MonitoringApi#pubsubGetLeafz")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="pubsubGetRoutez"></a>
# **pubsubGetRoutez**
> kotlin.Any pubsubGetRoutez()

Cluster routes

Cluster route connection information.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MonitoringApi()
try {
    val result : kotlin.Any = apiInstance.pubsubGetRoutez()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MonitoringApi#pubsubGetRoutez")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MonitoringApi#pubsubGetRoutez")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="pubsubGetSubsz"></a>
# **pubsubGetSubsz**
> kotlin.Any pubsubGetSubsz()

Subscription info

Subscription routing tree information.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MonitoringApi()
try {
    val result : kotlin.Any = apiInstance.pubsubGetSubsz()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MonitoringApi#pubsubGetSubsz")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MonitoringApi#pubsubGetSubsz")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="pubsubGetVarz"></a>
# **pubsubGetVarz**
> PubsubServerVarz pubsubGetVarz()

Server statistics

General server information including uptime, connections, message rates.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MonitoringApi()
try {
    val result : PubsubServerVarz = apiInstance.pubsubGetVarz()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MonitoringApi#pubsubGetVarz")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MonitoringApi#pubsubGetVarz")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PubsubServerVarz**](PubsubServerVarz.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

