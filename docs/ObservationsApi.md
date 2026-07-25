# ObservationsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**consoleGetObservation**](ObservationsApi.md#consoleGetObservation) | **GET** /v1/console/observations/{observationId} | Get an observation by ID |
| [**consoleListObservations**](ObservationsApi.md#consoleListObservations) | **GET** /v1/console/observations | Get a list of observations |


<a id="consoleGetObservation"></a>
# **consoleGetObservation**
> ConsoleObservation consoleGetObservation(observationId)

Get an observation by ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ObservationsApi()
val observationId : kotlin.String = observationId_example // kotlin.String | 
try {
    val result : ConsoleObservation = apiInstance.consoleGetObservation(observationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ObservationsApi#consoleGetObservation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ObservationsApi#consoleGetObservation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **observationId** | **kotlin.String**|  | |

### Return type

[**ConsoleObservation**](ConsoleObservation.md)

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

<a id="consoleListObservations"></a>
# **consoleListObservations**
> ConsoleListObservations200Response consoleListObservations(page, limit, name, userId, type, traceId, level, parentObservationId, environment, fromStartTime, toStartTime, version)

Get a list of observations

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ObservationsApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val name : kotlin.String = name_example // kotlin.String | 
val userId : kotlin.String = userId_example // kotlin.String | 
val type : kotlin.String = type_example // kotlin.String | 
val traceId : kotlin.String = traceId_example // kotlin.String | 
val level : kotlin.String = level_example // kotlin.String | 
val parentObservationId : kotlin.String = parentObservationId_example // kotlin.String | 
val environment : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val fromStartTime : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
val toStartTime : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
val version : kotlin.String = version_example // kotlin.String | 
try {
    val result : ConsoleListObservations200Response = apiInstance.consoleListObservations(page, limit, name, userId, type, traceId, level, parentObservationId, environment, fromStartTime, toStartTime, version)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ObservationsApi#consoleListObservations")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ObservationsApi#consoleListObservations")
    e.printStackTrace()
}
```

### Parameters
| **page** | **kotlin.Int**|  | [optional] [default to 1] |
| **limit** | **kotlin.Int**|  | [optional] [default to 50] |
| **name** | **kotlin.String**|  | [optional] |
| **userId** | **kotlin.String**|  | [optional] |
| **type** | **kotlin.String**|  | [optional] |
| **traceId** | **kotlin.String**|  | [optional] |
| **level** | **kotlin.String**|  | [optional] [enum: DEBUG, DEFAULT, WARNING, ERROR] |
| **parentObservationId** | **kotlin.String**|  | [optional] |
| **environment** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional] |
| **fromStartTime** | **java.time.OffsetDateTime**|  | [optional] |
| **toStartTime** | **java.time.OffsetDateTime**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **version** | **kotlin.String**|  | [optional] |

### Return type

[**ConsoleListObservations200Response**](ConsoleListObservations200Response.md)

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

