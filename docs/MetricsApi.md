# MetricsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**consoleGetDailyMetrics**](MetricsApi.md#consoleGetDailyMetrics) | **GET** /v1/console/metrics/daily | Get daily metrics |
| [**consoleGetMetrics**](MetricsApi.md#consoleGetMetrics) | **GET** /v1/console/metrics | Get metrics from the project |
| [**functionsFunctionMetrics**](MetricsApi.md#functionsFunctionMetrics) | **GET** /v1/functions/metrics | Invocation histogram + status breakdown |
| [**observeGetMetrics**](MetricsApi.md#observeGetMetrics) | **GET** /v1/o11y/metrics | Per-org RED metrics and LLM usage for a product |


<a id="consoleGetDailyMetrics"></a>
# **consoleGetDailyMetrics**
> ConsoleGetDailyMetrics200Response consoleGetDailyMetrics(page, limit, traceName, userId, tags, fromTimestamp, toTimestamp, environment)

Get daily metrics

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MetricsApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val traceName : kotlin.String = traceName_example // kotlin.String | 
val userId : kotlin.String = userId_example // kotlin.String | 
val tags : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val fromTimestamp : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
val toTimestamp : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
val environment : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
try {
    val result : ConsoleGetDailyMetrics200Response = apiInstance.consoleGetDailyMetrics(page, limit, traceName, userId, tags, fromTimestamp, toTimestamp, environment)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MetricsApi#consoleGetDailyMetrics")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MetricsApi#consoleGetDailyMetrics")
    e.printStackTrace()
}
```

### Parameters
| **page** | **kotlin.Int**|  | [optional] |
| **limit** | **kotlin.Int**|  | [optional] |
| **traceName** | **kotlin.String**|  | [optional] |
| **userId** | **kotlin.String**|  | [optional] |
| **tags** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional] |
| **fromTimestamp** | **java.time.OffsetDateTime**|  | [optional] |
| **toTimestamp** | **java.time.OffsetDateTime**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **environment** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional] |

### Return type

[**ConsoleGetDailyMetrics200Response**](ConsoleGetDailyMetrics200Response.md)

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

<a id="consoleGetMetrics"></a>
# **consoleGetMetrics**
> ConsoleGetMetrics200Response consoleGetMetrics(query)

Get metrics from the project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MetricsApi()
val query : kotlin.String = query_example // kotlin.String | JSON string containing the query parameters (view, dimensions, metrics, filters, timeDimension, fromTimestamp, toTimestamp)
try {
    val result : ConsoleGetMetrics200Response = apiInstance.consoleGetMetrics(query)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MetricsApi#consoleGetMetrics")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MetricsApi#consoleGetMetrics")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **query** | **kotlin.String**| JSON string containing the query parameters (view, dimensions, metrics, filters, timeDimension, fromTimestamp, toTimestamp) | |

### Return type

[**ConsoleGetMetrics200Response**](ConsoleGetMetrics200Response.md)

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

<a id="functionsFunctionMetrics"></a>
# **functionsFunctionMetrics**
> FunctionsMetrics functionsFunctionMetrics(range)

Invocation histogram + status breakdown

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MetricsApi()
val range : kotlin.String = range_example // kotlin.String | 
try {
    val result : FunctionsMetrics = apiInstance.functionsFunctionMetrics(range)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MetricsApi#functionsFunctionMetrics")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MetricsApi#functionsFunctionMetrics")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **range** | **kotlin.String**|  | [optional] [default to Range._24H] [enum: 24H, 7D, 30D] |

### Return type

[**FunctionsMetrics**](FunctionsMetrics.md)

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

<a id="observeGetMetrics"></a>
# **observeGetMetrics**
> ObserveMetricsResponse observeGetMetrics(product, range, stepSec)

Per-org RED metrics and LLM usage for a product

Returns REAL per-org RED (rate / errors / latency) series for a product from org-tagged request spans, plus the org&#39;s LLM usage (calls / tokens / cost) from the usage ledger. The bucket width is &#x60;stepSec&#x60; (explicit or derived as ~60 buckets across the range, clamped to [30, 3600]). Usage is a secondary signal — its absence never fails the response. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MetricsApi()
val product : kotlin.String = product_example // kotlin.String | Console product slug. Must match `^[a-z0-9][a-z0-9._-]{0,62}$`.
val range : kotlin.Int = 56 // kotlin.Int | Look-back range in seconds (default 3600, max 604800).
val stepSec : kotlin.Int = 56 // kotlin.Int | Explicit bucket width in seconds (clamped to [30, 3600]). Omit to auto-derive.
try {
    val result : ObserveMetricsResponse = apiInstance.observeGetMetrics(product, range, stepSec)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MetricsApi#observeGetMetrics")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MetricsApi#observeGetMetrics")
    e.printStackTrace()
}
```

### Parameters
| **product** | **kotlin.String**| Console product slug. Must match &#x60;^[a-z0-9][a-z0-9._-]{0,62}$&#x60;. | |
| **range** | **kotlin.Int**| Look-back range in seconds (default 3600, max 604800). | [optional] [default to 3600] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stepSec** | **kotlin.Int**| Explicit bucket width in seconds (clamped to [30, 3600]). Omit to auto-derive. | [optional] |

### Return type

[**ObserveMetricsResponse**](ObserveMetricsResponse.md)

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

