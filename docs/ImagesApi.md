# ImagesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatPostFilesImages**](ImagesApi.md#chatPostFilesImages) | **POST** /v1/chat/files/images | Upload an image |


<a id="chatPostFilesImages"></a>
# **chatPostFilesImages**
> kotlin.Any chatPostFilesImages(file)

Upload an image

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ImagesApi()
val file : java.io.File = BINARY_DATA_HERE // java.io.File | 
try {
    val result : kotlin.Any = apiInstance.chatPostFilesImages(file)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ImagesApi#chatPostFilesImages")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ImagesApi#chatPostFilesImages")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **file** | **java.io.File**|  | |

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

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

