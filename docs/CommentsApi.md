# CommentsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**consoleCreateComment**](CommentsApi.md#consoleCreateComment) | **POST** /v1/console/comments | Create a comment |
| [**consoleGetComment**](CommentsApi.md#consoleGetComment) | **GET** /v1/console/comments/{commentId} | Get a comment by ID |
| [**consoleListComments**](CommentsApi.md#consoleListComments) | **GET** /v1/console/comments | Get all comments |


<a id="consoleCreateComment"></a>
# **consoleCreateComment**
> ConsoleCreateComment200Response consoleCreateComment(consoleCreateCommentRequest)

Create a comment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CommentsApi()
val consoleCreateCommentRequest : ConsoleCreateCommentRequest =  // ConsoleCreateCommentRequest | 
try {
    val result : ConsoleCreateComment200Response = apiInstance.consoleCreateComment(consoleCreateCommentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CommentsApi#consoleCreateComment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CommentsApi#consoleCreateComment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **consoleCreateCommentRequest** | [**ConsoleCreateCommentRequest**](ConsoleCreateCommentRequest.md)|  | |

### Return type

[**ConsoleCreateComment200Response**](ConsoleCreateComment200Response.md)

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

<a id="consoleGetComment"></a>
# **consoleGetComment**
> ConsoleComment consoleGetComment(commentId)

Get a comment by ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CommentsApi()
val commentId : kotlin.String = commentId_example // kotlin.String | 
try {
    val result : ConsoleComment = apiInstance.consoleGetComment(commentId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CommentsApi#consoleGetComment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CommentsApi#consoleGetComment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commentId** | **kotlin.String**|  | |

### Return type

[**ConsoleComment**](ConsoleComment.md)

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

<a id="consoleListComments"></a>
# **consoleListComments**
> ConsoleListComments200Response consoleListComments(page, limit, objectType, objectId, authorUserId)

Get all comments

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CommentsApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val objectType : kotlin.String = objectType_example // kotlin.String | Filter by object type (trace, observation, session, prompt)
val objectId : kotlin.String = objectId_example // kotlin.String | 
val authorUserId : kotlin.String = authorUserId_example // kotlin.String | 
try {
    val result : ConsoleListComments200Response = apiInstance.consoleListComments(page, limit, objectType, objectId, authorUserId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CommentsApi#consoleListComments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CommentsApi#consoleListComments")
    e.printStackTrace()
}
```

### Parameters
| **page** | **kotlin.Int**|  | [optional] |
| **limit** | **kotlin.Int**|  | [optional] |
| **objectType** | **kotlin.String**| Filter by object type (trace, observation, session, prompt) | [optional] |
| **objectId** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **authorUserId** | **kotlin.String**|  | [optional] |

### Return type

[**ConsoleListComments200Response**](ConsoleListComments200Response.md)

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

