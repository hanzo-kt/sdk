# TriggersApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoListTriggerEvents**](TriggersApi.md#autoListTriggerEvents) | **GET** /v1/auto/trigger-events | List trigger events for a flow |
| [**autoListTriggerRuns**](TriggersApi.md#autoListTriggerRuns) | **GET** /v1/auto/trigger-runs | List trigger run history |
| [**autoTestTrigger**](TriggersApi.md#autoTestTrigger) | **POST** /v1/auto/test-trigger | Test a trigger and get sample data |
| [**flowHandleAppEvent**](TriggersApi.md#flowHandleAppEvent) | **POST** /v1/flow/app-events/{pieceUrl} | Handle incoming app event for trigger routing |
| [**flowListTriggerEvents**](TriggersApi.md#flowListTriggerEvents) | **GET** /v1/flow/trigger-events | List trigger events for a flow |
| [**flowListTriggerRuns**](TriggersApi.md#flowListTriggerRuns) | **GET** /v1/flow/trigger-runs | List trigger run history |
| [**flowTestTrigger**](TriggersApi.md#flowTestTrigger) | **POST** /v1/flow/test-trigger | Test a trigger and get sample data |


<a id="autoListTriggerEvents"></a>
# **autoListTriggerEvents**
> kotlin.Any autoListTriggerEvents(flowId)

List trigger events for a flow

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TriggersApi()
val flowId : kotlin.String = flowId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.autoListTriggerEvents(flowId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TriggersApi#autoListTriggerEvents")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TriggersApi#autoListTriggerEvents")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **flowId** | **kotlin.String**|  | |

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

<a id="autoListTriggerRuns"></a>
# **autoListTriggerRuns**
> kotlin.Any autoListTriggerRuns(flowId)

List trigger run history

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TriggersApi()
val flowId : kotlin.String = flowId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.autoListTriggerRuns(flowId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TriggersApi#autoListTriggerRuns")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TriggersApi#autoListTriggerRuns")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **flowId** | **kotlin.String**|  | [optional] |

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

<a id="autoTestTrigger"></a>
# **autoTestTrigger**
> kotlin.Any autoTestTrigger(autoTestTriggerRequest)

Test a trigger and get sample data

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TriggersApi()
val autoTestTriggerRequest : AutoTestTriggerRequest =  // AutoTestTriggerRequest | 
try {
    val result : kotlin.Any = apiInstance.autoTestTrigger(autoTestTriggerRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TriggersApi#autoTestTrigger")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TriggersApi#autoTestTrigger")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoTestTriggerRequest** | [**AutoTestTriggerRequest**](AutoTestTriggerRequest.md)|  | |

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

<a id="flowHandleAppEvent"></a>
# **flowHandleAppEvent**
> kotlin.Any flowHandleAppEvent(pieceUrl, body)

Handle incoming app event for trigger routing

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TriggersApi()
val pieceUrl : kotlin.String = pieceUrl_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.flowHandleAppEvent(pieceUrl, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TriggersApi#flowHandleAppEvent")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TriggersApi#flowHandleAppEvent")
    e.printStackTrace()
}
```

### Parameters
| **pieceUrl** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | [optional] |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="flowListTriggerEvents"></a>
# **flowListTriggerEvents**
> kotlin.Any flowListTriggerEvents(flowId)

List trigger events for a flow

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TriggersApi()
val flowId : kotlin.String = flowId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.flowListTriggerEvents(flowId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TriggersApi#flowListTriggerEvents")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TriggersApi#flowListTriggerEvents")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **flowId** | **kotlin.String**|  | |

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

<a id="flowListTriggerRuns"></a>
# **flowListTriggerRuns**
> kotlin.Any flowListTriggerRuns(flowId, cursor, limit)

List trigger run history

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TriggersApi()
val flowId : kotlin.String = flowId_example // kotlin.String | 
val cursor : kotlin.String = cursor_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : kotlin.Any = apiInstance.flowListTriggerRuns(flowId, cursor, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TriggersApi#flowListTriggerRuns")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TriggersApi#flowListTriggerRuns")
    e.printStackTrace()
}
```

### Parameters
| **flowId** | **kotlin.String**|  | [optional] |
| **cursor** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] |

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

<a id="flowTestTrigger"></a>
# **flowTestTrigger**
> kotlin.Any flowTestTrigger(autoTestTriggerRequest)

Test a trigger and get sample data

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TriggersApi()
val autoTestTriggerRequest : AutoTestTriggerRequest =  // AutoTestTriggerRequest | 
try {
    val result : kotlin.Any = apiInstance.flowTestTrigger(autoTestTriggerRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TriggersApi#flowTestTrigger")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TriggersApi#flowTestTrigger")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoTestTriggerRequest** | [**AutoTestTriggerRequest**](AutoTestTriggerRequest.md)|  | |

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

