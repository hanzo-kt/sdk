# DatasetRunItemsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**consoleCreateDatasetRunItem**](DatasetRunItemsApi.md#consoleCreateDatasetRunItem) | **POST** /v1/console/dataset-run-items | Create a dataset run item |


<a id="consoleCreateDatasetRunItem"></a>
# **consoleCreateDatasetRunItem**
> ConsoleDatasetRunItem consoleCreateDatasetRunItem(consoleCreateDatasetRunItemRequest)

Create a dataset run item

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DatasetRunItemsApi()
val consoleCreateDatasetRunItemRequest : ConsoleCreateDatasetRunItemRequest =  // ConsoleCreateDatasetRunItemRequest | 
try {
    val result : ConsoleDatasetRunItem = apiInstance.consoleCreateDatasetRunItem(consoleCreateDatasetRunItemRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DatasetRunItemsApi#consoleCreateDatasetRunItem")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DatasetRunItemsApi#consoleCreateDatasetRunItem")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **consoleCreateDatasetRunItemRequest** | [**ConsoleCreateDatasetRunItemRequest**](ConsoleCreateDatasetRunItemRequest.md)|  | |

### Return type

[**ConsoleDatasetRunItem**](ConsoleDatasetRunItem.md)

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

