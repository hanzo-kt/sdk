# O11yApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**o11yO11yDashboards**](O11yApi.md#o11yO11yDashboards) | **GET** /v1/o11y/dashboards | List dashboards |
| [**o11yO11yHealth**](O11yApi.md#o11yO11yHealth) | **GET** /v1/o11y/health | O11y health |
| [**o11yO11yIngest**](O11yApi.md#o11yO11yIngest) | **POST** /v1/o11y/ingestion | Ingest LLM-observability events |
| [**o11yO11yQuery**](O11yApi.md#o11yO11yQuery) | **POST** /v1/o11y/query | Instant builder query |
| [**o11yO11yQueryRange**](O11yApi.md#o11yO11yQueryRange) | **POST** /v1/o11y/query_range | Range builder query |
| [**o11yO11yRules**](O11yApi.md#o11yO11yRules) | **GET** /v1/o11y/rules | List alert rules |
| [**o11yO11yServices**](O11yApi.md#o11yO11yServices) | **GET** /v1/o11y/services | List traced services |
| [**o11yO11yVMQuery**](O11yApi.md#o11yO11yVMQuery) | **GET** /v1/o11y/vm/query | Platform infra health — instant VM query (SuperAdmin) |
| [**o11yO11yVMQueryRange**](O11yApi.md#o11yO11yVMQueryRange) | **GET** /v1/o11y/vm/query_range | Platform infra health — range VM query (SuperAdmin) |


<a id="o11yO11yDashboards"></a>
# **o11yO11yDashboards**
> kotlin.collections.List&lt;O11yDashboardSummary&gt; o11yO11yDashboards()

List dashboards

List dashboards from the o11y runtime.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = O11yApi()
try {
    val result : kotlin.collections.List<O11yDashboardSummary> = apiInstance.o11yO11yDashboards()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling O11yApi#o11yO11yDashboards")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling O11yApi#o11yO11yDashboards")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;O11yDashboardSummary&gt;**](O11yDashboardSummary.md)

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

<a id="o11yO11yHealth"></a>
# **o11yO11yHealth**
> O11yHealthResponse o11yO11yHealth()

O11y health

Liveness of the o11y subsystem.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = O11yApi()
try {
    val result : O11yHealthResponse = apiInstance.o11yO11yHealth()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling O11yApi#o11yO11yHealth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling O11yApi#o11yO11yHealth")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**O11yHealthResponse**](O11yHealthResponse.md)

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

<a id="o11yO11yIngest"></a>
# **o11yO11yIngest**
> O11yIngestResult o11yO11yIngest(o11yIngestBatch)

Ingest LLM-observability events

Native-Go write path for LLM-observability events (traces, observations, scores). Events arrive as a batch; the response reports how many were persisted versus dropped as an unknown type.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = O11yApi()
val o11yIngestBatch : O11yIngestBatch =  // O11yIngestBatch | 
try {
    val result : O11yIngestResult = apiInstance.o11yO11yIngest(o11yIngestBatch)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling O11yApi#o11yO11yIngest")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling O11yApi#o11yO11yIngest")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **o11yIngestBatch** | [**O11yIngestBatch**](O11yIngestBatch.md)|  | |

### Return type

[**O11yIngestResult**](O11yIngestResult.md)

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

<a id="o11yO11yQuery"></a>
# **o11yO11yQuery**
> O11yBuilderQueryResult o11yO11yQuery(o11yBuilderQuery)

Instant builder query

Evaluate a composite builder query at a single point in time. The org is pinned server-side; the internal engine version is resolved internally.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = O11yApi()
val o11yBuilderQuery : O11yBuilderQuery =  // O11yBuilderQuery | 
try {
    val result : O11yBuilderQueryResult = apiInstance.o11yO11yQuery(o11yBuilderQuery)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling O11yApi#o11yO11yQuery")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling O11yApi#o11yO11yQuery")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **o11yBuilderQuery** | [**O11yBuilderQuery**](O11yBuilderQuery.md)|  | |

### Return type

[**O11yBuilderQueryResult**](O11yBuilderQueryResult.md)

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

<a id="o11yO11yQueryRange"></a>
# **o11yO11yQueryRange**
> O11yBuilderQueryResult o11yO11yQueryRange(o11yBuilderQuery)

Range builder query

Evaluate a composite builder query over a range of time — the console composite list query. The org is pinned server-side.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = O11yApi()
val o11yBuilderQuery : O11yBuilderQuery =  // O11yBuilderQuery | 
try {
    val result : O11yBuilderQueryResult = apiInstance.o11yO11yQueryRange(o11yBuilderQuery)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling O11yApi#o11yO11yQueryRange")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling O11yApi#o11yO11yQueryRange")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **o11yBuilderQuery** | [**O11yBuilderQuery**](O11yBuilderQuery.md)|  | |

### Return type

[**O11yBuilderQueryResult**](O11yBuilderQueryResult.md)

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

<a id="o11yO11yRules"></a>
# **o11yO11yRules**
> kotlin.collections.List&lt;O11yAlertRule&gt; o11yO11yRules()

List alert rules

List alert rules from the o11y runtime.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = O11yApi()
try {
    val result : kotlin.collections.List<O11yAlertRule> = apiInstance.o11yO11yRules()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling O11yApi#o11yO11yRules")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling O11yApi#o11yO11yRules")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;O11yAlertRule&gt;**](O11yAlertRule.md)

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

<a id="o11yO11yServices"></a>
# **o11yO11yServices**
> O11yO11yServices200Response o11yO11yServices()

List traced services

List the services known to the o11y runtime.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = O11yApi()
try {
    val result : O11yO11yServices200Response = apiInstance.o11yO11yServices()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling O11yApi#o11yO11yServices")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling O11yApi#o11yO11yServices")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**O11yO11yServices200Response**](O11yO11yServices200Response.md)

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

<a id="o11yO11yVMQuery"></a>
# **o11yO11yVMQuery**
> O11yPrometheusResponse o11yO11yVMQuery(query)

Platform infra health — instant VM query (SuperAdmin)

SuperAdmin-only VictoriaMetrics instant read proxy backing the platform infrastructure-health board. The query is allowlisted to the exact set the board issues; anything else is a 400. The native Prometheus envelope is returned verbatim.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = O11yApi()
val query : kotlin.String = query_example // kotlin.String | Allowlisted PromQL. Only up, sum(up), and count(up) are permitted.
try {
    val result : O11yPrometheusResponse = apiInstance.o11yO11yVMQuery(query)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling O11yApi#o11yO11yVMQuery")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling O11yApi#o11yO11yVMQuery")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **query** | **kotlin.String**| Allowlisted PromQL. Only up, sum(up), and count(up) are permitted. | [enum: up, sum(up), count(up)] |

### Return type

[**O11yPrometheusResponse**](O11yPrometheusResponse.md)

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

<a id="o11yO11yVMQueryRange"></a>
# **o11yO11yVMQueryRange**
> O11yPrometheusResponse o11yO11yVMQueryRange(query, start, end, step)

Platform infra health — range VM query (SuperAdmin)

SuperAdmin-only VictoriaMetrics range read proxy backing the platform infrastructure-health board. The query is allowlisted; start, end, and step are validated as positive integers. The native Prometheus envelope is returned verbatim.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = O11yApi()
val query : kotlin.String = query_example // kotlin.String | Allowlisted PromQL. Only up, sum(up), and count(up) are permitted.
val start : kotlin.Long = 789 // kotlin.Long | Range start (Unix seconds, positive integer).
val end : kotlin.Long = 789 // kotlin.Long | Range end (Unix seconds, positive integer).
val step : kotlin.Int = 56 // kotlin.Int | Step resolution (seconds, positive integer).
try {
    val result : O11yPrometheusResponse = apiInstance.o11yO11yVMQueryRange(query, start, end, step)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling O11yApi#o11yO11yVMQueryRange")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling O11yApi#o11yO11yVMQueryRange")
    e.printStackTrace()
}
```

### Parameters
| **query** | **kotlin.String**| Allowlisted PromQL. Only up, sum(up), and count(up) are permitted. | [enum: up, sum(up), count(up)] |
| **start** | **kotlin.Long**| Range start (Unix seconds, positive integer). | |
| **end** | **kotlin.Long**| Range end (Unix seconds, positive integer). | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **step** | **kotlin.Int**| Step resolution (seconds, positive integer). | |

### Return type

[**O11yPrometheusResponse**](O11yPrometheusResponse.md)

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

