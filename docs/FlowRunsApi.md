# FlowRunsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoGetFlowRun**](FlowRunsApi.md#autoGetFlowRun) | **GET** /v1/auto/flow-runs/{id} | Get a flow run by id |
| [**autoListFlowRuns**](FlowRunsApi.md#autoListFlowRuns) | **GET** /v1/auto/flow-runs | List flow runs |
| [**autoResumeFlowRun**](FlowRunsApi.md#autoResumeFlowRun) | **POST** /v1/auto/flow-runs/{id}/requests/{requestId} | Resume a paused flow run with human input |
| [**autoRetryFlowRun**](FlowRunsApi.md#autoRetryFlowRun) | **POST** /v1/auto/flow-runs/{id}/retry | Retry a failed flow run |
| [**flowBulkCancelFlowRuns**](FlowRunsApi.md#flowBulkCancelFlowRuns) | **POST** /v1/flow/flow-runs/bulk/cancel | Bulk cancel running flow runs |
| [**flowGetFlowRun**](FlowRunsApi.md#flowGetFlowRun) | **GET** /v1/flow/flow-runs/{id} | Get a flow run by id |
| [**flowListFlowRuns**](FlowRunsApi.md#flowListFlowRuns) | **GET** /v1/flow/flow-runs | List flow runs |
| [**flowResumeFlowRun**](FlowRunsApi.md#flowResumeFlowRun) | **POST** /v1/flow/flow-runs/{id}/requests/{requestId} | Resume a paused flow run with human input |
| [**flowRetryFlowRun**](FlowRunsApi.md#flowRetryFlowRun) | **POST** /v1/flow/flow-runs/{id}/retry | Retry a failed flow run |


<a id="autoGetFlowRun"></a>
# **autoGetFlowRun**
> AutoFlowRun autoGetFlowRun(id)

Get a flow run by id

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowRunsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : AutoFlowRun = apiInstance.autoGetFlowRun(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowRunsApi#autoGetFlowRun")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowRunsApi#autoGetFlowRun")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**AutoFlowRun**](AutoFlowRun.md)

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

<a id="autoListFlowRuns"></a>
# **autoListFlowRuns**
> AutoListFlowRuns200Response autoListFlowRuns(flowId, status, cursor, limit, createdAfter, createdBefore)

List flow runs

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowRunsApi()
val flowId : kotlin.String = flowId_example // kotlin.String | 
val status : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val cursor : kotlin.String = cursor_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val createdAfter : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
val createdBefore : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
try {
    val result : AutoListFlowRuns200Response = apiInstance.autoListFlowRuns(flowId, status, cursor, limit, createdAfter, createdBefore)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowRunsApi#autoListFlowRuns")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowRunsApi#autoListFlowRuns")
    e.printStackTrace()
}
```

### Parameters
| **flowId** | **kotlin.String**|  | [optional] |
| **status** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional] [enum: RUNNING, SUCCEEDED, FAILED, TIMEOUT, PAUSED, STOPPED] |
| **cursor** | **kotlin.String**|  | [optional] |
| **limit** | **kotlin.Int**|  | [optional] [default to 10] |
| **createdAfter** | **java.time.OffsetDateTime**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createdBefore** | **java.time.OffsetDateTime**|  | [optional] |

### Return type

[**AutoListFlowRuns200Response**](AutoListFlowRuns200Response.md)

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

<a id="autoResumeFlowRun"></a>
# **autoResumeFlowRun**
> kotlin.Any autoResumeFlowRun(id, requestId, body)

Resume a paused flow run with human input

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowRunsApi()
val id : kotlin.String = id_example // kotlin.String | 
val requestId : kotlin.String = requestId_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.autoResumeFlowRun(id, requestId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowRunsApi#autoResumeFlowRun")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowRunsApi#autoResumeFlowRun")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| **requestId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | [optional] |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="autoRetryFlowRun"></a>
# **autoRetryFlowRun**
> kotlin.Any autoRetryFlowRun(id)

Retry a failed flow run

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowRunsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.autoRetryFlowRun(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowRunsApi#autoRetryFlowRun")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowRunsApi#autoRetryFlowRun")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

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

<a id="flowBulkCancelFlowRuns"></a>
# **flowBulkCancelFlowRuns**
> kotlin.Any flowBulkCancelFlowRuns(flowBulkCancelFlowRunsRequest)

Bulk cancel running flow runs

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowRunsApi()
val flowBulkCancelFlowRunsRequest : FlowBulkCancelFlowRunsRequest =  // FlowBulkCancelFlowRunsRequest | 
try {
    val result : kotlin.Any = apiInstance.flowBulkCancelFlowRuns(flowBulkCancelFlowRunsRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowRunsApi#flowBulkCancelFlowRuns")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowRunsApi#flowBulkCancelFlowRuns")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **flowBulkCancelFlowRunsRequest** | [**FlowBulkCancelFlowRunsRequest**](FlowBulkCancelFlowRunsRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="flowGetFlowRun"></a>
# **flowGetFlowRun**
> FlowFlowRun flowGetFlowRun(id)

Get a flow run by id

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowRunsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : FlowFlowRun = apiInstance.flowGetFlowRun(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowRunsApi#flowGetFlowRun")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowRunsApi#flowGetFlowRun")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**FlowFlowRun**](FlowFlowRun.md)

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

<a id="flowListFlowRuns"></a>
# **flowListFlowRuns**
> FlowListFlowRuns200Response flowListFlowRuns(flowId, status, tags, cursor, limit, createdAfter, createdBefore)

List flow runs

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowRunsApi()
val flowId : kotlin.String = flowId_example // kotlin.String | 
val status : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val tags : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val cursor : kotlin.String = cursor_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val createdAfter : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
val createdBefore : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
try {
    val result : FlowListFlowRuns200Response = apiInstance.flowListFlowRuns(flowId, status, tags, cursor, limit, createdAfter, createdBefore)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowRunsApi#flowListFlowRuns")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowRunsApi#flowListFlowRuns")
    e.printStackTrace()
}
```

### Parameters
| **flowId** | **kotlin.String**|  | [optional] |
| **status** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional] [enum: RUNNING, SUCCEEDED, FAILED, TIMEOUT, PAUSED, STOPPED] |
| **tags** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional] |
| **cursor** | **kotlin.String**|  | [optional] |
| **limit** | **kotlin.Int**|  | [optional] [default to 10] |
| **createdAfter** | **java.time.OffsetDateTime**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createdBefore** | **java.time.OffsetDateTime**|  | [optional] |

### Return type

[**FlowListFlowRuns200Response**](FlowListFlowRuns200Response.md)

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

<a id="flowResumeFlowRun"></a>
# **flowResumeFlowRun**
> kotlin.Any flowResumeFlowRun(id, requestId, body)

Resume a paused flow run with human input

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowRunsApi()
val id : kotlin.String = id_example // kotlin.String | 
val requestId : kotlin.String = requestId_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.flowResumeFlowRun(id, requestId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowRunsApi#flowResumeFlowRun")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowRunsApi#flowResumeFlowRun")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| **requestId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | [optional] |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="flowRetryFlowRun"></a>
# **flowRetryFlowRun**
> FlowFlowRun flowRetryFlowRun(id, flowRetryFlowRunRequest)

Retry a failed flow run

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowRunsApi()
val id : kotlin.String = id_example // kotlin.String | 
val flowRetryFlowRunRequest : FlowRetryFlowRunRequest =  // FlowRetryFlowRunRequest | 
try {
    val result : FlowFlowRun = apiInstance.flowRetryFlowRun(id, flowRetryFlowRunRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowRunsApi#flowRetryFlowRun")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowRunsApi#flowRetryFlowRun")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **flowRetryFlowRunRequest** | [**FlowRetryFlowRunRequest**](FlowRetryFlowRunRequest.md)|  | [optional] |

### Return type

[**FlowFlowRun**](FlowFlowRun.md)

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

