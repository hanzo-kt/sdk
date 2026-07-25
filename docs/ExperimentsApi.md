# ExperimentsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**mlCreateExperiment**](ExperimentsApi.md#mlCreateExperiment) | **POST** /v1/ml/experiments | Create an experiment |
| [**mlGetRunMetrics**](ExperimentsApi.md#mlGetRunMetrics) | **GET** /v1/ml/experiments/{experiment_id}/runs/{run_id}/metrics | Get run metrics |
| [**mlListExperimentRuns**](ExperimentsApi.md#mlListExperimentRuns) | **GET** /v1/ml/experiments/{experiment_id}/runs | List experiment runs |
| [**mlListExperiments**](ExperimentsApi.md#mlListExperiments) | **GET** /v1/ml/experiments | List experiments |
| [**mlLogMetrics**](ExperimentsApi.md#mlLogMetrics) | **POST** /v1/ml/experiments/{experiment_id}/runs/{run_id}/metrics | Log metrics |
| [**mlStartExperimentRun**](ExperimentsApi.md#mlStartExperimentRun) | **POST** /v1/ml/experiments/{experiment_id}/runs | Start an experiment run |


<a id="mlCreateExperiment"></a>
# **mlCreateExperiment**
> MlExperiment mlCreateExperiment(mlCreateExperimentRequest)

Create an experiment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ExperimentsApi()
val mlCreateExperimentRequest : MlCreateExperimentRequest =  // MlCreateExperimentRequest | 
try {
    val result : MlExperiment = apiInstance.mlCreateExperiment(mlCreateExperimentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ExperimentsApi#mlCreateExperiment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ExperimentsApi#mlCreateExperiment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **mlCreateExperimentRequest** | [**MlCreateExperimentRequest**](MlCreateExperimentRequest.md)|  | |

### Return type

[**MlExperiment**](MlExperiment.md)

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

<a id="mlGetRunMetrics"></a>
# **mlGetRunMetrics**
> MlGetRunMetrics200Response mlGetRunMetrics(experimentId, runId)

Get run metrics

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ExperimentsApi()
val experimentId : kotlin.String = experimentId_example // kotlin.String | 
val runId : kotlin.String = runId_example // kotlin.String | 
try {
    val result : MlGetRunMetrics200Response = apiInstance.mlGetRunMetrics(experimentId, runId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ExperimentsApi#mlGetRunMetrics")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ExperimentsApi#mlGetRunMetrics")
    e.printStackTrace()
}
```

### Parameters
| **experimentId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **runId** | **kotlin.String**|  | |

### Return type

[**MlGetRunMetrics200Response**](MlGetRunMetrics200Response.md)

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

<a id="mlListExperimentRuns"></a>
# **mlListExperimentRuns**
> MlListExperimentRuns200Response mlListExperimentRuns(experimentId)

List experiment runs

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ExperimentsApi()
val experimentId : kotlin.String = experimentId_example // kotlin.String | 
try {
    val result : MlListExperimentRuns200Response = apiInstance.mlListExperimentRuns(experimentId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ExperimentsApi#mlListExperimentRuns")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ExperimentsApi#mlListExperimentRuns")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **experimentId** | **kotlin.String**|  | |

### Return type

[**MlListExperimentRuns200Response**](MlListExperimentRuns200Response.md)

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

<a id="mlListExperiments"></a>
# **mlListExperiments**
> MlListExperiments200Response mlListExperiments()

List experiments

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ExperimentsApi()
try {
    val result : MlListExperiments200Response = apiInstance.mlListExperiments()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ExperimentsApi#mlListExperiments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ExperimentsApi#mlListExperiments")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**MlListExperiments200Response**](MlListExperiments200Response.md)

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

<a id="mlLogMetrics"></a>
# **mlLogMetrics**
> mlLogMetrics(experimentId, runId, requestBody)

Log metrics

Log metrics for a running experiment.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ExperimentsApi()
val experimentId : kotlin.String = experimentId_example // kotlin.String | 
val runId : kotlin.String = runId_example // kotlin.String | 
val requestBody : kotlin.collections.Map<kotlin.String, java.math.BigDecimal> = Object // kotlin.collections.Map<kotlin.String, java.math.BigDecimal> | 
try {
    apiInstance.mlLogMetrics(experimentId, runId, requestBody)
} catch (e: ClientException) {
    println("4xx response calling ExperimentsApi#mlLogMetrics")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ExperimentsApi#mlLogMetrics")
    e.printStackTrace()
}
```

### Parameters
| **experimentId** | **kotlin.String**|  | |
| **runId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **requestBody** | [**kotlin.collections.Map&lt;kotlin.String, java.math.BigDecimal&gt;**](java.math.BigDecimal.md)|  | |

### Return type

null (empty response body)

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
 - **Accept**: Not defined

<a id="mlStartExperimentRun"></a>
# **mlStartExperimentRun**
> MlExperimentRun mlStartExperimentRun(experimentId, mlStartExperimentRunRequest)

Start an experiment run

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ExperimentsApi()
val experimentId : kotlin.String = experimentId_example // kotlin.String | 
val mlStartExperimentRunRequest : MlStartExperimentRunRequest =  // MlStartExperimentRunRequest | 
try {
    val result : MlExperimentRun = apiInstance.mlStartExperimentRun(experimentId, mlStartExperimentRunRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ExperimentsApi#mlStartExperimentRun")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ExperimentsApi#mlStartExperimentRun")
    e.printStackTrace()
}
```

### Parameters
| **experimentId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **mlStartExperimentRunRequest** | [**MlStartExperimentRunRequest**](MlStartExperimentRunRequest.md)|  | |

### Return type

[**MlExperimentRun**](MlExperimentRun.md)

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

