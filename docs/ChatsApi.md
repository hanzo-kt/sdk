# ChatsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**searchListChatWorkspaces**](ChatsApi.md#searchListChatWorkspaces) | **GET** /v1/search/chats | List chat workspaces (experimental) |


<a id="searchListChatWorkspaces"></a>
# **searchListChatWorkspaces**
> kotlin.Any searchListChatWorkspaces()

List chat workspaces (experimental)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ChatsApi()
try {
    val result : kotlin.Any = apiInstance.searchListChatWorkspaces()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ChatsApi#searchListChatWorkspaces")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ChatsApi#searchListChatWorkspaces")
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

