# AnnotationQueuesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**consoleCreateAnnotationQueue**](AnnotationQueuesApi.md#consoleCreateAnnotationQueue) | **POST** /v1/console/annotation-queues | Create an annotation queue |
| [**consoleGetAnnotationQueue**](AnnotationQueuesApi.md#consoleGetAnnotationQueue) | **GET** /v1/console/annotation-queues/{queueId} | Get an annotation queue |
| [**consoleListAnnotationQueueItems**](AnnotationQueuesApi.md#consoleListAnnotationQueueItems) | **GET** /v1/console/annotation-queues/{queueId}/items | Get items for an annotation queue |
| [**consoleListAnnotationQueues**](AnnotationQueuesApi.md#consoleListAnnotationQueues) | **GET** /v1/console/annotation-queues | Get all annotation queues |


<a id="consoleCreateAnnotationQueue"></a>
# **consoleCreateAnnotationQueue**
> ConsoleAnnotationQueue consoleCreateAnnotationQueue(consoleCreateAnnotationQueueRequest)

Create an annotation queue

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AnnotationQueuesApi()
val consoleCreateAnnotationQueueRequest : ConsoleCreateAnnotationQueueRequest =  // ConsoleCreateAnnotationQueueRequest | 
try {
    val result : ConsoleAnnotationQueue = apiInstance.consoleCreateAnnotationQueue(consoleCreateAnnotationQueueRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AnnotationQueuesApi#consoleCreateAnnotationQueue")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AnnotationQueuesApi#consoleCreateAnnotationQueue")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **consoleCreateAnnotationQueueRequest** | [**ConsoleCreateAnnotationQueueRequest**](ConsoleCreateAnnotationQueueRequest.md)|  | |

### Return type

[**ConsoleAnnotationQueue**](ConsoleAnnotationQueue.md)

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

<a id="consoleGetAnnotationQueue"></a>
# **consoleGetAnnotationQueue**
> ConsoleAnnotationQueue consoleGetAnnotationQueue(queueId)

Get an annotation queue

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AnnotationQueuesApi()
val queueId : kotlin.String = queueId_example // kotlin.String | 
try {
    val result : ConsoleAnnotationQueue = apiInstance.consoleGetAnnotationQueue(queueId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AnnotationQueuesApi#consoleGetAnnotationQueue")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AnnotationQueuesApi#consoleGetAnnotationQueue")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **queueId** | **kotlin.String**|  | |

### Return type

[**ConsoleAnnotationQueue**](ConsoleAnnotationQueue.md)

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

<a id="consoleListAnnotationQueueItems"></a>
# **consoleListAnnotationQueueItems**
> ConsoleListAnnotationQueueItems200Response consoleListAnnotationQueueItems(queueId, status, page, limit)

Get items for an annotation queue

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AnnotationQueuesApi()
val queueId : kotlin.String = queueId_example // kotlin.String | 
val status : kotlin.String = status_example // kotlin.String | 
val page : kotlin.Int = 56 // kotlin.Int | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : ConsoleListAnnotationQueueItems200Response = apiInstance.consoleListAnnotationQueueItems(queueId, status, page, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AnnotationQueuesApi#consoleListAnnotationQueueItems")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AnnotationQueuesApi#consoleListAnnotationQueueItems")
    e.printStackTrace()
}
```

### Parameters
| **queueId** | **kotlin.String**|  | |
| **status** | **kotlin.String**|  | [optional] [enum: PENDING, COMPLETED, SKIPPED] |
| **page** | **kotlin.Int**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] |

### Return type

[**ConsoleListAnnotationQueueItems200Response**](ConsoleListAnnotationQueueItems200Response.md)

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

<a id="consoleListAnnotationQueues"></a>
# **consoleListAnnotationQueues**
> ConsoleListAnnotationQueues200Response consoleListAnnotationQueues(page, limit)

Get all annotation queues

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AnnotationQueuesApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : ConsoleListAnnotationQueues200Response = apiInstance.consoleListAnnotationQueues(page, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AnnotationQueuesApi#consoleListAnnotationQueues")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AnnotationQueuesApi#consoleListAnnotationQueues")
    e.printStackTrace()
}
```

### Parameters
| **page** | **kotlin.Int**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] |

### Return type

[**ConsoleListAnnotationQueues200Response**](ConsoleListAnnotationQueues200Response.md)

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

