# DatasetItemsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**consoleCreateDatasetItem**](DatasetItemsApi.md#consoleCreateDatasetItem) | **POST** /v1/console/dataset-items | Create or upsert a dataset item |
| [**consoleDeleteDatasetItem**](DatasetItemsApi.md#consoleDeleteDatasetItem) | **DELETE** /v1/console/dataset-items/{id} | Delete a dataset item |
| [**consoleGetDatasetItem**](DatasetItemsApi.md#consoleGetDatasetItem) | **GET** /v1/console/dataset-items/{id} | Get a dataset item |
| [**consoleListDatasetItems**](DatasetItemsApi.md#consoleListDatasetItems) | **GET** /v1/console/dataset-items | Get dataset items |


<a id="consoleCreateDatasetItem"></a>
# **consoleCreateDatasetItem**
> ConsoleDatasetItem consoleCreateDatasetItem(consoleCreateDatasetItemRequest)

Create or upsert a dataset item

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DatasetItemsApi()
val consoleCreateDatasetItemRequest : ConsoleCreateDatasetItemRequest =  // ConsoleCreateDatasetItemRequest | 
try {
    val result : ConsoleDatasetItem = apiInstance.consoleCreateDatasetItem(consoleCreateDatasetItemRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DatasetItemsApi#consoleCreateDatasetItem")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DatasetItemsApi#consoleCreateDatasetItem")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **consoleCreateDatasetItemRequest** | [**ConsoleCreateDatasetItemRequest**](ConsoleCreateDatasetItemRequest.md)|  | |

### Return type

[**ConsoleDatasetItem**](ConsoleDatasetItem.md)

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

<a id="consoleDeleteDatasetItem"></a>
# **consoleDeleteDatasetItem**
> ConsoleDeleteDatasetItem200Response consoleDeleteDatasetItem(id)

Delete a dataset item

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DatasetItemsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : ConsoleDeleteDatasetItem200Response = apiInstance.consoleDeleteDatasetItem(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DatasetItemsApi#consoleDeleteDatasetItem")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DatasetItemsApi#consoleDeleteDatasetItem")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**ConsoleDeleteDatasetItem200Response**](ConsoleDeleteDatasetItem200Response.md)

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

<a id="consoleGetDatasetItem"></a>
# **consoleGetDatasetItem**
> ConsoleDatasetItem consoleGetDatasetItem(id)

Get a dataset item

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DatasetItemsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : ConsoleDatasetItem = apiInstance.consoleGetDatasetItem(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DatasetItemsApi#consoleGetDatasetItem")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DatasetItemsApi#consoleGetDatasetItem")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**ConsoleDatasetItem**](ConsoleDatasetItem.md)

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

<a id="consoleListDatasetItems"></a>
# **consoleListDatasetItems**
> ConsoleListDatasetItems200Response consoleListDatasetItems(datasetName, sourceTraceId, sourceObservationId, version, page, limit)

Get dataset items

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DatasetItemsApi()
val datasetName : kotlin.String = datasetName_example // kotlin.String | 
val sourceTraceId : kotlin.String = sourceTraceId_example // kotlin.String | 
val sourceObservationId : kotlin.String = sourceObservationId_example // kotlin.String | 
val version : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | ISO 8601 timestamp. Returns state of dataset at this time.
val page : kotlin.Int = 56 // kotlin.Int | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : ConsoleListDatasetItems200Response = apiInstance.consoleListDatasetItems(datasetName, sourceTraceId, sourceObservationId, version, page, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DatasetItemsApi#consoleListDatasetItems")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DatasetItemsApi#consoleListDatasetItems")
    e.printStackTrace()
}
```

### Parameters
| **datasetName** | **kotlin.String**|  | [optional] |
| **sourceTraceId** | **kotlin.String**|  | [optional] |
| **sourceObservationId** | **kotlin.String**|  | [optional] |
| **version** | **java.time.OffsetDateTime**| ISO 8601 timestamp. Returns state of dataset at this time. | [optional] |
| **page** | **kotlin.Int**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] |

### Return type

[**ConsoleListDatasetItems200Response**](ConsoleListDatasetItems200Response.md)

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

