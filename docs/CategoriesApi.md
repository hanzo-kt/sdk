# CategoriesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatGetCategories**](CategoriesApi.md#chatGetCategories) | **GET** /v1/chat/categories | Get all categories |


<a id="chatGetCategories"></a>
# **chatGetCategories**
> kotlin.collections.List&lt;ChatCategory&gt; chatGetCategories()

Get all categories

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CategoriesApi()
try {
    val result : kotlin.collections.List<ChatCategory> = apiInstance.chatGetCategories()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CategoriesApi#chatGetCategories")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CategoriesApi#chatGetCategories")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;ChatCategory&gt;**](ChatCategory.md)

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

