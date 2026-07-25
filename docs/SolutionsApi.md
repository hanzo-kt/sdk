# SolutionsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**flowApplySolution**](SolutionsApi.md#flowApplySolution) | **POST** /v1/flow/solutions/{id}/apply | Apply a solution to the project (EE) |
| [**flowCreateSolution**](SolutionsApi.md#flowCreateSolution) | **POST** /v1/flow/solutions | Create a solution from flows (EE) |
| [**flowListSolutions**](SolutionsApi.md#flowListSolutions) | **GET** /v1/flow/solutions | List packaged solutions (EE) |


<a id="flowApplySolution"></a>
# **flowApplySolution**
> kotlin.Any flowApplySolution(id)

Apply a solution to the project (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SolutionsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.flowApplySolution(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SolutionsApi#flowApplySolution")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SolutionsApi#flowApplySolution")
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

<a id="flowCreateSolution"></a>
# **flowCreateSolution**
> kotlin.Any flowCreateSolution(flowCreateSolutionRequest)

Create a solution from flows (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SolutionsApi()
val flowCreateSolutionRequest : FlowCreateSolutionRequest =  // FlowCreateSolutionRequest | 
try {
    val result : kotlin.Any = apiInstance.flowCreateSolution(flowCreateSolutionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SolutionsApi#flowCreateSolution")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SolutionsApi#flowCreateSolution")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **flowCreateSolutionRequest** | [**FlowCreateSolutionRequest**](FlowCreateSolutionRequest.md)|  | |

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

<a id="flowListSolutions"></a>
# **flowListSolutions**
> kotlin.Any flowListSolutions()

List packaged solutions (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SolutionsApi()
try {
    val result : kotlin.Any = apiInstance.flowListSolutions()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SolutionsApi#flowListSolutions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SolutionsApi#flowListSolutions")
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

