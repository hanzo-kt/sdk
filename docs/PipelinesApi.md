# PipelinesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**engineCreatePipeline**](PipelinesApi.md#engineCreatePipeline) | **POST** /v1/engine/pipelines | Create ML pipeline |
| [**engineCreatePipelineRun**](PipelinesApi.md#engineCreatePipelineRun) | **POST** /v1/engine/pipelines/{id}/runs | Create pipeline run |
| [**engineDeletePipeline**](PipelinesApi.md#engineDeletePipeline) | **DELETE** /v1/engine/pipelines/{id} | Delete pipeline |
| [**engineGetPipeline**](PipelinesApi.md#engineGetPipeline) | **GET** /v1/engine/pipelines/{id} | Get pipeline |
| [**engineGetPipelineRun**](PipelinesApi.md#engineGetPipelineRun) | **GET** /v1/engine/pipelines/{id}/runs/{run_id} | Get pipeline run |
| [**engineListPipelineRuns**](PipelinesApi.md#engineListPipelineRuns) | **GET** /v1/engine/pipelines/{id}/runs | List pipeline runs |
| [**engineListPipelines**](PipelinesApi.md#engineListPipelines) | **GET** /v1/engine/pipelines | List ML pipelines |
| [**mlCreatePipeline**](PipelinesApi.md#mlCreatePipeline) | **POST** /v1/ml/pipelines | Create a pipeline |
| [**mlGetPipeline**](PipelinesApi.md#mlGetPipeline) | **GET** /v1/ml/pipelines/{pipeline_id} | Get pipeline details |
| [**mlListPipelineRuns**](PipelinesApi.md#mlListPipelineRuns) | **GET** /v1/ml/pipelines/{pipeline_id}/runs | List pipeline runs |
| [**mlListPipelines**](PipelinesApi.md#mlListPipelines) | **GET** /v1/ml/pipelines | List pipelines |
| [**mlStartPipelineRun**](PipelinesApi.md#mlStartPipelineRun) | **POST** /v1/ml/pipelines/{pipeline_id}/runs | Start a pipeline run |


<a id="engineCreatePipeline"></a>
# **engineCreatePipeline**
> EnginePipeline engineCreatePipeline(enginePipelineCreate)

Create ML pipeline

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PipelinesApi()
val enginePipelineCreate : EnginePipelineCreate =  // EnginePipelineCreate | 
try {
    val result : EnginePipeline = apiInstance.engineCreatePipeline(enginePipelineCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PipelinesApi#engineCreatePipeline")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PipelinesApi#engineCreatePipeline")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **enginePipelineCreate** | [**EnginePipelineCreate**](EnginePipelineCreate.md)|  | |

### Return type

[**EnginePipeline**](EnginePipeline.md)

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

<a id="engineCreatePipelineRun"></a>
# **engineCreatePipelineRun**
> EnginePipelineRun engineCreatePipelineRun(id, enginePipelineRunCreate)

Create pipeline run

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PipelinesApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val enginePipelineRunCreate : EnginePipelineRunCreate =  // EnginePipelineRunCreate | 
try {
    val result : EnginePipelineRun = apiInstance.engineCreatePipelineRun(id, enginePipelineRunCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PipelinesApi#engineCreatePipelineRun")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PipelinesApi#engineCreatePipelineRun")
    e.printStackTrace()
}
```

### Parameters
| **id** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **enginePipelineRunCreate** | [**EnginePipelineRunCreate**](EnginePipelineRunCreate.md)|  | [optional] |

### Return type

[**EnginePipelineRun**](EnginePipelineRun.md)

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

<a id="engineDeletePipeline"></a>
# **engineDeletePipeline**
> kotlin.Any engineDeletePipeline(id)

Delete pipeline

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PipelinesApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.engineDeletePipeline(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PipelinesApi#engineDeletePipeline")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PipelinesApi#engineDeletePipeline")
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

<a id="engineGetPipeline"></a>
# **engineGetPipeline**
> EnginePipeline engineGetPipeline(id)

Get pipeline

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PipelinesApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : EnginePipeline = apiInstance.engineGetPipeline(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PipelinesApi#engineGetPipeline")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PipelinesApi#engineGetPipeline")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**EnginePipeline**](EnginePipeline.md)

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

<a id="engineGetPipelineRun"></a>
# **engineGetPipelineRun**
> EnginePipelineRun engineGetPipelineRun(id, runId)

Get pipeline run

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PipelinesApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val runId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : EnginePipelineRun = apiInstance.engineGetPipelineRun(id, runId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PipelinesApi#engineGetPipelineRun")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PipelinesApi#engineGetPipelineRun")
    e.printStackTrace()
}
```

### Parameters
| **id** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **runId** | **java.util.UUID**|  | |

### Return type

[**EnginePipelineRun**](EnginePipelineRun.md)

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

<a id="engineListPipelineRuns"></a>
# **engineListPipelineRuns**
> EngineListPipelineRuns200Response engineListPipelineRuns(id, status, page, pageSize)

List pipeline runs

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PipelinesApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val status : kotlin.String = status_example // kotlin.String | 
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : EngineListPipelineRuns200Response = apiInstance.engineListPipelineRuns(id, status, page, pageSize)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PipelinesApi#engineListPipelineRuns")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PipelinesApi#engineListPipelineRuns")
    e.printStackTrace()
}
```

### Parameters
| **id** | **java.util.UUID**|  | |
| **status** | **kotlin.String**|  | [optional] [enum: pending, running, succeeded, failed, cancelled] |
| **page** | **kotlin.Int**|  | [optional] [default to 1] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **pageSize** | **kotlin.Int**|  | [optional] [default to 20] |

### Return type

[**EngineListPipelineRuns200Response**](EngineListPipelineRuns200Response.md)

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

<a id="engineListPipelines"></a>
# **engineListPipelines**
> EngineListPipelines200Response engineListPipelines(page, pageSize)

List ML pipelines

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PipelinesApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : EngineListPipelines200Response = apiInstance.engineListPipelines(page, pageSize)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PipelinesApi#engineListPipelines")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PipelinesApi#engineListPipelines")
    e.printStackTrace()
}
```

### Parameters
| **page** | **kotlin.Int**|  | [optional] [default to 1] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **pageSize** | **kotlin.Int**|  | [optional] [default to 20] |

### Return type

[**EngineListPipelines200Response**](EngineListPipelines200Response.md)

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

<a id="mlCreatePipeline"></a>
# **mlCreatePipeline**
> MlPipeline mlCreatePipeline(mlCreatePipelineRequest)

Create a pipeline

Create and optionally start a training pipeline.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PipelinesApi()
val mlCreatePipelineRequest : MlCreatePipelineRequest = {"name":"hanzo-finetune","parameters":{"base_model":"meta-llama/Llama-3.1-8B","dataset":"s3://hanzo-data/training/v2","epochs":"3","learning_rate":2.0E-5},"auto_start":true} // MlCreatePipelineRequest | 
try {
    val result : MlPipeline = apiInstance.mlCreatePipeline(mlCreatePipelineRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PipelinesApi#mlCreatePipeline")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PipelinesApi#mlCreatePipeline")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **mlCreatePipelineRequest** | [**MlCreatePipelineRequest**](MlCreatePipelineRequest.md)|  | |

### Return type

[**MlPipeline**](MlPipeline.md)

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

<a id="mlGetPipeline"></a>
# **mlGetPipeline**
> MlPipeline mlGetPipeline(pipelineId)

Get pipeline details

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PipelinesApi()
val pipelineId : kotlin.String = pipelineId_example // kotlin.String | 
try {
    val result : MlPipeline = apiInstance.mlGetPipeline(pipelineId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PipelinesApi#mlGetPipeline")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PipelinesApi#mlGetPipeline")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **pipelineId** | **kotlin.String**|  | |

### Return type

[**MlPipeline**](MlPipeline.md)

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

<a id="mlListPipelineRuns"></a>
# **mlListPipelineRuns**
> MlListPipelineRuns200Response mlListPipelineRuns(pipelineId)

List pipeline runs

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PipelinesApi()
val pipelineId : kotlin.String = pipelineId_example // kotlin.String | 
try {
    val result : MlListPipelineRuns200Response = apiInstance.mlListPipelineRuns(pipelineId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PipelinesApi#mlListPipelineRuns")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PipelinesApi#mlListPipelineRuns")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **pipelineId** | **kotlin.String**|  | |

### Return type

[**MlListPipelineRuns200Response**](MlListPipelineRuns200Response.md)

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

<a id="mlListPipelines"></a>
# **mlListPipelines**
> MlListPipelines200Response mlListPipelines(status, limit)

List pipelines

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PipelinesApi()
val status : kotlin.String = status_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : MlListPipelines200Response = apiInstance.mlListPipelines(status, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PipelinesApi#mlListPipelines")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PipelinesApi#mlListPipelines")
    e.printStackTrace()
}
```

### Parameters
| **status** | **kotlin.String**|  | [optional] [enum: pending, running, succeeded, failed, cancelled] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] [default to 50] |

### Return type

[**MlListPipelines200Response**](MlListPipelines200Response.md)

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

<a id="mlStartPipelineRun"></a>
# **mlStartPipelineRun**
> MlPipelineRun mlStartPipelineRun(pipelineId, mlStartPipelineRunRequest)

Start a pipeline run

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PipelinesApi()
val pipelineId : kotlin.String = pipelineId_example // kotlin.String | 
val mlStartPipelineRunRequest : MlStartPipelineRunRequest =  // MlStartPipelineRunRequest | 
try {
    val result : MlPipelineRun = apiInstance.mlStartPipelineRun(pipelineId, mlStartPipelineRunRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PipelinesApi#mlStartPipelineRun")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PipelinesApi#mlStartPipelineRun")
    e.printStackTrace()
}
```

### Parameters
| **pipelineId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **mlStartPipelineRunRequest** | [**MlStartPipelineRunRequest**](MlStartPipelineRunRequest.md)|  | [optional] |

### Return type

[**MlPipelineRun**](MlPipelineRun.md)

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

