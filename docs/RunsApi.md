# RunsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**automationsGetRun**](RunsApi.md#automationsGetRun) | **GET** /v1/automations/runs/{id} | Get a run (non-terminal status is refreshed from the engine) |
| [**automationsListRuns**](RunsApi.md#automationsListRuns) | **GET** /v1/automations/runs | List runs |
| [**automationsResumeRun**](RunsApi.md#automationsResumeRun) | **POST** /v1/automations/runs/{id}/resume | Resume a paused run |
| [**automationsRunFlow**](RunsApi.md#automationsRunFlow) | **POST** /v1/automations/flows/{id}/run | Start a durable run of a flow&#39;s runnable version |
| [**evalsGetV1EvalsHealth**](RunsApi.md#evalsGetV1EvalsHealth) | **GET** /v1/evals/health | Health check |
| [**evalsPostV1EvalsRuns**](RunsApi.md#evalsPostV1EvalsRuns) | **POST** /v1/evals/runs | Run a dataset against a model with an LLM-as-a-Judge |


<a id="automationsGetRun"></a>
# **automationsGetRun**
> AutomationsFlowRun automationsGetRun(id)

Get a run (non-terminal status is refreshed from the engine)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RunsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : AutomationsFlowRun = apiInstance.automationsGetRun(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RunsApi#automationsGetRun")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RunsApi#automationsGetRun")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**AutomationsFlowRun**](AutomationsFlowRun.md)

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

<a id="automationsListRuns"></a>
# **automationsListRuns**
> AutomationsListRuns200Response automationsListRuns(flowId, limit)

List runs

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RunsApi()
val flowId : kotlin.String = flowId_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : AutomationsListRuns200Response = apiInstance.automationsListRuns(flowId, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RunsApi#automationsListRuns")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RunsApi#automationsListRuns")
    e.printStackTrace()
}
```

### Parameters
| **flowId** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] [default to 200] |

### Return type

[**AutomationsListRuns200Response**](AutomationsListRuns200Response.md)

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

<a id="automationsResumeRun"></a>
# **automationsResumeRun**
> AutomationsResumeRun200Response automationsResumeRun(id, body)

Resume a paused run

The JSON body (max 64 KiB) is delivered verbatim as the waitpoint&#39;s output.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RunsApi()
val id : kotlin.String = id_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : AutomationsResumeRun200Response = apiInstance.automationsResumeRun(id, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RunsApi#automationsResumeRun")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RunsApi#automationsResumeRun")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | [optional] |

### Return type

[**AutomationsResumeRun200Response**](AutomationsResumeRun200Response.md)

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

<a id="automationsRunFlow"></a>
# **automationsRunFlow**
> AutomationsFlowRun automationsRunFlow(id)

Start a durable run of a flow&#39;s runnable version

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RunsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : AutomationsFlowRun = apiInstance.automationsRunFlow(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RunsApi#automationsRunFlow")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RunsApi#automationsRunFlow")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**AutomationsFlowRun**](AutomationsFlowRun.md)

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

<a id="evalsGetV1EvalsHealth"></a>
# **evalsGetV1EvalsHealth**
> EvalsGetV1EvalsHealth200Response evalsGetV1EvalsHealth()

Health check

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RunsApi()
try {
    val result : EvalsGetV1EvalsHealth200Response = apiInstance.evalsGetV1EvalsHealth()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RunsApi#evalsGetV1EvalsHealth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RunsApi#evalsGetV1EvalsHealth")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**EvalsGetV1EvalsHealth200Response**](EvalsGetV1EvalsHealth200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="evalsPostV1EvalsRuns"></a>
# **evalsPostV1EvalsRuns**
> EvalsRunSummary evalsPostV1EvalsRuns(evalsRunRequest)

Run a dataset against a model with an LLM-as-a-Judge

For each dataset item: calls the model-under-test through the Hanzo gateway, records a trace, then scores the output with the judge model against the criteria/metrics. Returns a per-item + aggregate summary with score, rationale, latency, tokens, and cost. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RunsApi()
val evalsRunRequest : EvalsRunRequest =  // EvalsRunRequest | 
try {
    val result : EvalsRunSummary = apiInstance.evalsPostV1EvalsRuns(evalsRunRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RunsApi#evalsPostV1EvalsRuns")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RunsApi#evalsPostV1EvalsRuns")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **evalsRunRequest** | [**EvalsRunRequest**](EvalsRunRequest.md)|  | |

### Return type

[**EvalsRunSummary**](EvalsRunSummary.md)

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

