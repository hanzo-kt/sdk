# IntelApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**worldWorldModelChanges**](IntelApi.md#worldWorldModelChanges) | **GET** /v1/world/model/changes | World model — what changed since a timestamp (the inform-our-AI hook) |
| [**worldWorldModelCountry**](IntelApi.md#worldWorldModelCountry) | **GET** /v1/world/model/country/{iso} | World model — one country&#39;s full state vector + recent deltas |
| [**worldWorldModelState**](IntelApi.md#worldWorldModelState) | **GET** /v1/world/model/state | World model — full compact world-state snapshot (all entities, instability-ranked) |
| [**worldWorldModelStream**](IntelApi.md#worldWorldModelStream) | **GET** /v1/world/model/stream | World model — SSE stream of state deltas as folds land |
| [**worldWorldModelTop**](IntelApi.md#worldWorldModelTop) | **GET** /v1/world/model/top | World model — top entities by metric |
| [**worldWorldPizzintDashboardData**](IntelApi.md#worldWorldPizzintDashboardData) | **GET** /v1/world/pizzint/dashboard-data | PIZZINT dashboard aggregate |
| [**worldWorldPizzintGdeltBatch**](IntelApi.md#worldWorldPizzintGdeltBatch) | **GET** /v1/world/pizzint/gdelt/batch | PIZZINT GDELT batch |
| [**worldWorldRiskScores**](IntelApi.md#worldWorldRiskScores) | **GET** /v1/world/risk-scores | Country risk scores |
| [**worldWorldServiceStatus**](IntelApi.md#worldWorldServiceStatus) | **GET** /v1/world/service-status | Upstream data-source status |
| [**worldWorldTemporalBaseline**](IntelApi.md#worldWorldTemporalBaseline) | **GET** /v1/world/temporal-baseline | Temporal baseline metrics |
| [**worldWorldTheaterPosture**](IntelApi.md#worldWorldTheaterPosture) | **GET** /v1/world/theater-posture | Strategic theater posture |


<a id="worldWorldModelChanges"></a>
# **worldWorldModelChanges**
> kotlin.Any worldWorldModelChanges(since)

World model — what changed since a timestamp (the inform-our-AI hook)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IntelApi()
val since : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
try {
    val result : kotlin.Any = apiInstance.worldWorldModelChanges(since)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IntelApi#worldWorldModelChanges")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IntelApi#worldWorldModelChanges")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **since** | **java.time.OffsetDateTime**|  | [optional] |

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

<a id="worldWorldModelCountry"></a>
# **worldWorldModelCountry**
> kotlin.Any worldWorldModelCountry(iso)

World model — one country&#39;s full state vector + recent deltas

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IntelApi()
val iso : kotlin.String = iso_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.worldWorldModelCountry(iso)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IntelApi#worldWorldModelCountry")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IntelApi#worldWorldModelCountry")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iso** | **kotlin.String**|  | |

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

<a id="worldWorldModelState"></a>
# **worldWorldModelState**
> kotlin.Any worldWorldModelState(kind)

World model — full compact world-state snapshot (all entities, instability-ranked)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IntelApi()
val kind : kotlin.String = kind_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.worldWorldModelState(kind)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IntelApi#worldWorldModelState")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IntelApi#worldWorldModelState")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kind** | **kotlin.String**|  | [optional] [enum: country, theater, market] |

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

<a id="worldWorldModelStream"></a>
# **worldWorldModelStream**
> kotlin.String worldWorldModelStream()

World model — SSE stream of state deltas as folds land

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IntelApi()
try {
    val result : kotlin.String = apiInstance.worldWorldModelStream()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IntelApi#worldWorldModelStream")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IntelApi#worldWorldModelStream")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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
 - **Accept**: Not defined

<a id="worldWorldModelTop"></a>
# **worldWorldModelTop**
> kotlin.Any worldWorldModelTop(metric, kind, n)

World model — top entities by metric

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IntelApi()
val metric : kotlin.String = metric_example // kotlin.String | 
val kind : kotlin.String = kind_example // kotlin.String | 
val n : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : kotlin.Any = apiInstance.worldWorldModelTop(metric, kind, n)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IntelApi#worldWorldModelTop")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IntelApi#worldWorldModelTop")
    e.printStackTrace()
}
```

### Parameters
| **metric** | **kotlin.String**|  | [optional] [enum: instability, velocity, sentiment] |
| **kind** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **n** | **kotlin.Int**|  | [optional] |

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

<a id="worldWorldPizzintDashboardData"></a>
# **worldWorldPizzintDashboardData**
> kotlin.Any worldWorldPizzintDashboardData()

PIZZINT dashboard aggregate

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IntelApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldPizzintDashboardData()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IntelApi#worldWorldPizzintDashboardData")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IntelApi#worldWorldPizzintDashboardData")
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

<a id="worldWorldPizzintGdeltBatch"></a>
# **worldWorldPizzintGdeltBatch**
> kotlin.Any worldWorldPizzintGdeltBatch()

PIZZINT GDELT batch

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IntelApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldPizzintGdeltBatch()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IntelApi#worldWorldPizzintGdeltBatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IntelApi#worldWorldPizzintGdeltBatch")
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

<a id="worldWorldRiskScores"></a>
# **worldWorldRiskScores**
> kotlin.Any worldWorldRiskScores()

Country risk scores

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IntelApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldRiskScores()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IntelApi#worldWorldRiskScores")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IntelApi#worldWorldRiskScores")
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

<a id="worldWorldServiceStatus"></a>
# **worldWorldServiceStatus**
> kotlin.Any worldWorldServiceStatus()

Upstream data-source status

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IntelApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldServiceStatus()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IntelApi#worldWorldServiceStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IntelApi#worldWorldServiceStatus")
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

<a id="worldWorldTemporalBaseline"></a>
# **worldWorldTemporalBaseline**
> kotlin.Any worldWorldTemporalBaseline()

Temporal baseline metrics

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IntelApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldTemporalBaseline()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IntelApi#worldWorldTemporalBaseline")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IntelApi#worldWorldTemporalBaseline")
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

<a id="worldWorldTheaterPosture"></a>
# **worldWorldTheaterPosture**
> kotlin.Any worldWorldTheaterPosture()

Strategic theater posture

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IntelApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldTheaterPosture()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IntelApi#worldWorldTheaterPosture")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IntelApi#worldWorldTheaterPosture")
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

