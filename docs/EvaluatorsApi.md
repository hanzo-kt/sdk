# EvaluatorsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**evalsPostV1EvalsEvaluators**](EvaluatorsApi.md#evalsPostV1EvalsEvaluators) | **POST** /v1/evals/evaluators | Register an evaluator (pre-built metric or custom rubric) |


<a id="evalsPostV1EvalsEvaluators"></a>
# **evalsPostV1EvalsEvaluators**
> evalsPostV1EvalsEvaluators(evalsEvaluator)

Register an evaluator (pre-built metric or custom rubric)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EvaluatorsApi()
val evalsEvaluator : EvalsEvaluator =  // EvalsEvaluator | 
try {
    apiInstance.evalsPostV1EvalsEvaluators(evalsEvaluator)
} catch (e: ClientException) {
    println("4xx response calling EvaluatorsApi#evalsPostV1EvalsEvaluators")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EvaluatorsApi#evalsPostV1EvalsEvaluators")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **evalsEvaluator** | [**EvalsEvaluator**](EvalsEvaluator.md)|  | |

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
 - **Accept**: application/json

