# SampleDataApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoGetSampleData**](SampleDataApi.md#autoGetSampleData) | **GET** /v1/auto/sample-data | Get sample data for a flow step |
| [**flowGetSampleData**](SampleDataApi.md#flowGetSampleData) | **GET** /v1/flow/sample-data | Get sample data for a flow step |
| [**flowSaveSampleData**](SampleDataApi.md#flowSaveSampleData) | **POST** /v1/flow/sample-data | Save sample data for a flow step |


<a id="autoGetSampleData"></a>
# **autoGetSampleData**
> kotlin.Any autoGetSampleData(flowId, flowVersionId, stepName)

Get sample data for a flow step

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SampleDataApi()
val flowId : kotlin.String = flowId_example // kotlin.String | 
val flowVersionId : kotlin.String = flowVersionId_example // kotlin.String | 
val stepName : kotlin.String = stepName_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.autoGetSampleData(flowId, flowVersionId, stepName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SampleDataApi#autoGetSampleData")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SampleDataApi#autoGetSampleData")
    e.printStackTrace()
}
```

### Parameters
| **flowId** | **kotlin.String**|  | |
| **flowVersionId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stepName** | **kotlin.String**|  | |

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

<a id="flowGetSampleData"></a>
# **flowGetSampleData**
> kotlin.Any flowGetSampleData(flowId, flowVersionId, stepName)

Get sample data for a flow step

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SampleDataApi()
val flowId : kotlin.String = flowId_example // kotlin.String | 
val flowVersionId : kotlin.String = flowVersionId_example // kotlin.String | 
val stepName : kotlin.String = stepName_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.flowGetSampleData(flowId, flowVersionId, stepName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SampleDataApi#flowGetSampleData")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SampleDataApi#flowGetSampleData")
    e.printStackTrace()
}
```

### Parameters
| **flowId** | **kotlin.String**|  | |
| **flowVersionId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stepName** | **kotlin.String**|  | |

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

<a id="flowSaveSampleData"></a>
# **flowSaveSampleData**
> kotlin.Any flowSaveSampleData(flowSaveSampleDataRequest)

Save sample data for a flow step

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SampleDataApi()
val flowSaveSampleDataRequest : FlowSaveSampleDataRequest =  // FlowSaveSampleDataRequest | 
try {
    val result : kotlin.Any = apiInstance.flowSaveSampleData(flowSaveSampleDataRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SampleDataApi#flowSaveSampleData")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SampleDataApi#flowSaveSampleData")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **flowSaveSampleDataRequest** | [**FlowSaveSampleDataRequest**](FlowSaveSampleDataRequest.md)|  | |

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

