# JobsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**engineCancelJob**](JobsApi.md#engineCancelJob) | **POST** /v1/engine/jobs/{id}/cancel | Cancel job |
| [**engineDeleteJob**](JobsApi.md#engineDeleteJob) | **DELETE** /v1/engine/jobs/{id} | Delete job |
| [**engineGetJob**](JobsApi.md#engineGetJob) | **GET** /v1/engine/jobs/{id} | Get job |
| [**engineGetJobLogs**](JobsApi.md#engineGetJobLogs) | **GET** /v1/engine/jobs/{id}/logs | Get job logs |
| [**engineGetJobMetrics**](JobsApi.md#engineGetJobMetrics) | **GET** /v1/engine/jobs/{id}/metrics | Get job metrics |
| [**engineListJobs**](JobsApi.md#engineListJobs) | **GET** /v1/engine/jobs | List jobs |
| [**engineSubmitJob**](JobsApi.md#engineSubmitJob) | **POST** /v1/engine/jobs | Submit job |


<a id="engineCancelJob"></a>
# **engineCancelJob**
> EngineJob engineCancelJob(id)

Cancel job

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = JobsApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : EngineJob = apiInstance.engineCancelJob(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling JobsApi#engineCancelJob")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling JobsApi#engineCancelJob")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**EngineJob**](EngineJob.md)

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

<a id="engineDeleteJob"></a>
# **engineDeleteJob**
> kotlin.Any engineDeleteJob(id)

Delete job

Deletes a completed or cancelled job and its artifacts.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = JobsApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.engineDeleteJob(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling JobsApi#engineDeleteJob")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling JobsApi#engineDeleteJob")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

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

<a id="engineGetJob"></a>
# **engineGetJob**
> EngineJob engineGetJob(id)

Get job

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = JobsApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : EngineJob = apiInstance.engineGetJob(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling JobsApi#engineGetJob")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling JobsApi#engineGetJob")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**EngineJob**](EngineJob.md)

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

<a id="engineGetJobLogs"></a>
# **engineGetJobLogs**
> kotlin.String engineGetJobLogs(id, tail, follow)

Get job logs

Returns job logs. Use Accept text/event-stream for streaming.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = JobsApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val tail : kotlin.Int = 56 // kotlin.Int | Number of lines from the end
val follow : kotlin.Boolean = true // kotlin.Boolean | Stream logs in real time
try {
    val result : kotlin.String = apiInstance.engineGetJobLogs(id, tail, follow)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling JobsApi#engineGetJobLogs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling JobsApi#engineGetJobLogs")
    e.printStackTrace()
}
```

### Parameters
| **id** | **java.util.UUID**|  | |
| **tail** | **kotlin.Int**| Number of lines from the end | [optional] [default to 100] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **follow** | **kotlin.Boolean**| Stream logs in real time | [optional] [default to false] |

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

<a id="engineGetJobMetrics"></a>
# **engineGetJobMetrics**
> EngineJobMetrics engineGetJobMetrics(id)

Get job metrics

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = JobsApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : EngineJobMetrics = apiInstance.engineGetJobMetrics(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling JobsApi#engineGetJobMetrics")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling JobsApi#engineGetJobMetrics")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**EngineJobMetrics**](EngineJobMetrics.md)

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

<a id="engineListJobs"></a>
# **engineListJobs**
> EngineListJobs200Response engineListJobs(status, type, clusterId, page, pageSize)

List jobs

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = JobsApi()
val status : kotlin.String = status_example // kotlin.String | 
val type : kotlin.String = type_example // kotlin.String | 
val clusterId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : EngineListJobs200Response = apiInstance.engineListJobs(status, type, clusterId, page, pageSize)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling JobsApi#engineListJobs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling JobsApi#engineListJobs")
    e.printStackTrace()
}
```

### Parameters
| **status** | **kotlin.String**|  | [optional] [enum: pending, scheduling, running, succeeded, failed, cancelled] |
| **type** | **kotlin.String**|  | [optional] [enum: training, inference, fine_tune, evaluation] |
| **clusterId** | **java.util.UUID**|  | [optional] |
| **page** | **kotlin.Int**|  | [optional] [default to 1] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **pageSize** | **kotlin.Int**|  | [optional] [default to 20] |

### Return type

[**EngineListJobs200Response**](EngineListJobs200Response.md)

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

<a id="engineSubmitJob"></a>
# **engineSubmitJob**
> EngineJob engineSubmitJob(engineJobCreate)

Submit job

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = JobsApi()
val engineJobCreate : EngineJobCreate =  // EngineJobCreate | 
try {
    val result : EngineJob = apiInstance.engineSubmitJob(engineJobCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling JobsApi#engineSubmitJob")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling JobsApi#engineSubmitJob")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **engineJobCreate** | [**EngineJobCreate**](EngineJobCreate.md)|  | |

### Return type

[**EngineJob**](EngineJob.md)

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

