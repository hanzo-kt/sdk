# TracesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**consoleDeleteTrace**](TracesApi.md#consoleDeleteTrace) | **DELETE** /v1/console/traces/{traceId} | Delete a specific trace |
| [**consoleDeleteTraces**](TracesApi.md#consoleDeleteTraces) | **DELETE** /v1/console/traces | Delete multiple traces |
| [**consoleGetTrace**](TracesApi.md#consoleGetTrace) | **GET** /v1/console/traces/{traceId} | Get a specific trace with full details |
| [**consoleListTraces**](TracesApi.md#consoleListTraces) | **GET** /v1/console/traces | Get list of traces |


<a id="consoleDeleteTrace"></a>
# **consoleDeleteTrace**
> ConsoleDeleteDatasetItem200Response consoleDeleteTrace(traceId)

Delete a specific trace

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TracesApi()
val traceId : kotlin.String = traceId_example // kotlin.String | 
try {
    val result : ConsoleDeleteDatasetItem200Response = apiInstance.consoleDeleteTrace(traceId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TracesApi#consoleDeleteTrace")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TracesApi#consoleDeleteTrace")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **traceId** | **kotlin.String**|  | |

### Return type

[**ConsoleDeleteDatasetItem200Response**](ConsoleDeleteDatasetItem200Response.md)

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

<a id="consoleDeleteTraces"></a>
# **consoleDeleteTraces**
> ConsoleDeleteDatasetItem200Response consoleDeleteTraces(consoleDeleteTracesRequest)

Delete multiple traces

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TracesApi()
val consoleDeleteTracesRequest : ConsoleDeleteTracesRequest =  // ConsoleDeleteTracesRequest | 
try {
    val result : ConsoleDeleteDatasetItem200Response = apiInstance.consoleDeleteTraces(consoleDeleteTracesRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TracesApi#consoleDeleteTraces")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TracesApi#consoleDeleteTraces")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **consoleDeleteTracesRequest** | [**ConsoleDeleteTracesRequest**](ConsoleDeleteTracesRequest.md)|  | |

### Return type

[**ConsoleDeleteDatasetItem200Response**](ConsoleDeleteDatasetItem200Response.md)

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

<a id="consoleGetTrace"></a>
# **consoleGetTrace**
> ConsoleTraceWithFullDetails consoleGetTrace(traceId)

Get a specific trace with full details

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TracesApi()
val traceId : kotlin.String = traceId_example // kotlin.String | 
try {
    val result : ConsoleTraceWithFullDetails = apiInstance.consoleGetTrace(traceId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TracesApi#consoleGetTrace")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TracesApi#consoleGetTrace")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **traceId** | **kotlin.String**|  | |

### Return type

[**ConsoleTraceWithFullDetails**](ConsoleTraceWithFullDetails.md)

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

<a id="consoleListTraces"></a>
# **consoleListTraces**
> ConsoleListTraces200Response consoleListTraces(page, limit, userId, name, sessionId, fromTimestamp, toTimestamp, orderBy, tags, version, release, environment, filter)

Get list of traces

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TracesApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val userId : kotlin.String = userId_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val sessionId : kotlin.String = sessionId_example // kotlin.String | 
val fromTimestamp : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
val toTimestamp : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
val orderBy : kotlin.String = orderBy_example // kotlin.String | Format: field.asc|desc (e.g., timestamp.desc)
val tags : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val version : kotlin.String = version_example // kotlin.String | 
val release : kotlin.String = release_example // kotlin.String | 
val environment : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val filter : kotlin.String = filter_example // kotlin.String | JSON array of filter conditions (overrides other filters when provided)
try {
    val result : ConsoleListTraces200Response = apiInstance.consoleListTraces(page, limit, userId, name, sessionId, fromTimestamp, toTimestamp, orderBy, tags, version, release, environment, filter)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TracesApi#consoleListTraces")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TracesApi#consoleListTraces")
    e.printStackTrace()
}
```

### Parameters
| **page** | **kotlin.Int**|  | [optional] [default to 1] |
| **limit** | **kotlin.Int**|  | [optional] [default to 50] |
| **userId** | **kotlin.String**|  | [optional] |
| **name** | **kotlin.String**|  | [optional] |
| **sessionId** | **kotlin.String**|  | [optional] |
| **fromTimestamp** | **java.time.OffsetDateTime**|  | [optional] |
| **toTimestamp** | **java.time.OffsetDateTime**|  | [optional] |
| **orderBy** | **kotlin.String**| Format: field.asc|desc (e.g., timestamp.desc) | [optional] |
| **tags** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional] |
| **version** | **kotlin.String**|  | [optional] |
| **release** | **kotlin.String**|  | [optional] |
| **environment** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **filter** | **kotlin.String**| JSON array of filter conditions (overrides other filters when provided) | [optional] |

### Return type

[**ConsoleListTraces200Response**](ConsoleListTraces200Response.md)

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

