# LogsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**edgeGetFunctionLogs**](LogsApi.md#edgeGetFunctionLogs) | **GET** /v1/edge/functions/{slug}/logs | Get function logs |
| [**observeGetLogs**](LogsApi.md#observeGetLogs) | **GET** /v1/o11y/logs | Live org-scoped log stream for a product |
| [**paasGetContainerLogs**](LogsApi.md#paasGetContainerLogs) | **GET** /v1/paas/org/{orgId}/project/{projectId}/env/{envId}/containers/{containerId}/logs | Get container logs |
| [**searchGetStderrLogs**](LogsApi.md#searchGetStderrLogs) | **GET** /v1/search/logs/stderr | Get stderr log configuration |
| [**searchResetStderrLogs**](LogsApi.md#searchResetStderrLogs) | **DELETE** /v1/search/logs/stderr | Reset stderr log level to default |
| [**searchStreamLogs**](LogsApi.md#searchStreamLogs) | **POST** /v1/search/logs/stream | Stream logs |
| [**searchUpdateStderrLogs**](LogsApi.md#searchUpdateStderrLogs) | **PUT** /v1/search/logs/stderr | Update stderr log level |


<a id="edgeGetFunctionLogs"></a>
# **edgeGetFunctionLogs**
> kotlin.collections.List&lt;EdgeLogEntry&gt; edgeGetFunctionLogs(slug, since, until, level, limit)

Get function logs

Returns function execution logs. Supports SSE streaming via Accept: text/event-stream header for live tailing. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = LogsApi()
val slug : kotlin.String = slug_example // kotlin.String | 
val since : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | Return logs after this timestamp
val until : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
val level : kotlin.String = level_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : kotlin.collections.List<EdgeLogEntry> = apiInstance.edgeGetFunctionLogs(slug, since, until, level, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LogsApi#edgeGetFunctionLogs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LogsApi#edgeGetFunctionLogs")
    e.printStackTrace()
}
```

### Parameters
| **slug** | **kotlin.String**|  | |
| **since** | **java.time.OffsetDateTime**| Return logs after this timestamp | [optional] |
| **until** | **java.time.OffsetDateTime**|  | [optional] |
| **level** | **kotlin.String**|  | [optional] [enum: info, warn, error, debug] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] [default to 100] |

### Return type

[**kotlin.collections.List&lt;EdgeLogEntry&gt;**](EdgeLogEntry.md)

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

<a id="observeGetLogs"></a>
# **observeGetLogs**
> ObserveLogsResponse observeGetLogs(product, sinceNs, window, limit)

Live org-scoped log stream for a product

Returns a live, org-scoped log stream for a product. The admin org (&#x60;IAM_ADMIN_ORG&#x60;) receives the product&#39;s raw infra stdout stream (&#x60;view: infra&#x60;); every other org receives its OWN request log stream derived from org-tagged spans (&#x60;view: request&#x60;). Live-tail by polling with &#x60;sinceNs&#x60; set to the prior response&#39;s &#x60;nextCursor&#x60;; absent a cursor, the last &#x60;window&#x60; seconds are returned. Every query is LIMIT-bounded. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = LogsApi()
val product : kotlin.String = product_example // kotlin.String | Console product slug. Must match `^[a-z0-9][a-z0-9._-]{0,62}$`.
val sinceNs : kotlin.Long = 789 // kotlin.Long | Nanosecond cursor from the prior response's `nextCursor`; 0/absent starts a fresh window.
val window : kotlin.Int = 56 // kotlin.Int | Initial look-back window in seconds when no cursor is supplied (default 900, max 86400).
val limit : kotlin.Int = 56 // kotlin.Int | Max lines returned (default 200, max 1000).
try {
    val result : ObserveLogsResponse = apiInstance.observeGetLogs(product, sinceNs, window, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LogsApi#observeGetLogs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LogsApi#observeGetLogs")
    e.printStackTrace()
}
```

### Parameters
| **product** | **kotlin.String**| Console product slug. Must match &#x60;^[a-z0-9][a-z0-9._-]{0,62}$&#x60;. | |
| **sinceNs** | **kotlin.Long**| Nanosecond cursor from the prior response&#39;s &#x60;nextCursor&#x60;; 0/absent starts a fresh window. | [optional] |
| **window** | **kotlin.Int**| Initial look-back window in seconds when no cursor is supplied (default 900, max 86400). | [optional] [default to 900] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**| Max lines returned (default 200, max 1000). | [optional] [default to 200] |

### Return type

[**ObserveLogsResponse**](ObserveLogsResponse.md)

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

<a id="paasGetContainerLogs"></a>
# **paasGetContainerLogs**
> kotlin.String paasGetContainerLogs(orgId, projectId, envId, containerId, tail, follow)

Get container logs

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = LogsApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
val projectId : kotlin.String = projectId_example // kotlin.String | 
val envId : kotlin.String = envId_example // kotlin.String | 
val containerId : kotlin.String = containerId_example // kotlin.String | 
val tail : kotlin.Int = 56 // kotlin.Int | 
val follow : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : kotlin.String = apiInstance.paasGetContainerLogs(orgId, projectId, envId, containerId, tail, follow)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LogsApi#paasGetContainerLogs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LogsApi#paasGetContainerLogs")
    e.printStackTrace()
}
```

### Parameters
| **orgId** | **kotlin.String**|  | |
| **projectId** | **kotlin.String**|  | |
| **envId** | **kotlin.String**|  | |
| **containerId** | **kotlin.String**|  | |
| **tail** | **kotlin.Int**|  | [optional] [default to 100] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **follow** | **kotlin.Boolean**|  | [optional] [default to false] |

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
 - **Accept**: text/plain

<a id="searchGetStderrLogs"></a>
# **searchGetStderrLogs**
> SearchGetStderrLogs200Response searchGetStderrLogs()

Get stderr log configuration

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = LogsApi()
try {
    val result : SearchGetStderrLogs200Response = apiInstance.searchGetStderrLogs()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LogsApi#searchGetStderrLogs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LogsApi#searchGetStderrLogs")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**SearchGetStderrLogs200Response**](SearchGetStderrLogs200Response.md)

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

<a id="searchResetStderrLogs"></a>
# **searchResetStderrLogs**
> SearchGetStderrLogs200Response searchResetStderrLogs()

Reset stderr log level to default

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = LogsApi()
try {
    val result : SearchGetStderrLogs200Response = apiInstance.searchResetStderrLogs()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LogsApi#searchResetStderrLogs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LogsApi#searchResetStderrLogs")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**SearchGetStderrLogs200Response**](SearchGetStderrLogs200Response.md)

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

<a id="searchStreamLogs"></a>
# **searchStreamLogs**
> kotlin.String searchStreamLogs(searchStreamLogsRequest)

Stream logs

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = LogsApi()
val searchStreamLogsRequest : SearchStreamLogsRequest =  // SearchStreamLogsRequest | 
try {
    val result : kotlin.String = apiInstance.searchStreamLogs(searchStreamLogsRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LogsApi#searchStreamLogs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LogsApi#searchStreamLogs")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **searchStreamLogsRequest** | [**SearchStreamLogsRequest**](SearchStreamLogsRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: text/plain

<a id="searchUpdateStderrLogs"></a>
# **searchUpdateStderrLogs**
> SearchGetStderrLogs200Response searchUpdateStderrLogs(searchUpdateStderrLogsRequest)

Update stderr log level

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = LogsApi()
val searchUpdateStderrLogsRequest : SearchUpdateStderrLogsRequest =  // SearchUpdateStderrLogsRequest | 
try {
    val result : SearchGetStderrLogs200Response = apiInstance.searchUpdateStderrLogs(searchUpdateStderrLogsRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LogsApi#searchUpdateStderrLogs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LogsApi#searchUpdateStderrLogs")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **searchUpdateStderrLogsRequest** | [**SearchUpdateStderrLogsRequest**](SearchUpdateStderrLogsRequest.md)|  | |

### Return type

[**SearchGetStderrLogs200Response**](SearchGetStderrLogs200Response.md)

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

