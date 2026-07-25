# SearchAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudProductControllerChatDocs**](SearchAPIApi.md#cloudProductControllerChatDocs) | **POST** /v1/chat-docs |  |
| [**cloudProductControllerIndexDocs**](SearchAPIApi.md#cloudProductControllerIndexDocs) | **POST** /v1/index-docs |  |
| [**cloudProductControllerSearchDocs**](SearchAPIApi.md#cloudProductControllerSearchDocs) | **POST** /v1/search-docs |  |


<a id="cloudProductControllerChatDocs"></a>
# **cloudProductControllerChatDocs**
> kotlin.Any cloudProductControllerChatDocs(cloudProductControllerChatDocsRequest, store)



RAG chat — retrieves relevant context from the document index and returns a grounded answer.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SearchAPIApi()
val cloudProductControllerChatDocsRequest : CloudProductControllerChatDocsRequest =  // CloudProductControllerChatDocsRequest | 
val store : kotlin.String = store_example // kotlin.String | Optional store/index selector (e.g. bot-docs).
try {
    val result : kotlin.Any = apiInstance.cloudProductControllerChatDocs(cloudProductControllerChatDocsRequest, store)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchAPIApi#cloudProductControllerChatDocs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchAPIApi#cloudProductControllerChatDocs")
    e.printStackTrace()
}
```

### Parameters
| **cloudProductControllerChatDocsRequest** | [**CloudProductControllerChatDocsRequest**](CloudProductControllerChatDocsRequest.md)|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **store** | **kotlin.String**| Optional store/index selector (e.g. bot-docs). | [optional] |

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

<a id="cloudProductControllerIndexDocs"></a>
# **cloudProductControllerIndexDocs**
> kotlin.Any cloudProductControllerIndexDocs(cloudProductControllerIndexDocsRequest, store)



Index (upsert) documents into the search backend. Write scope required.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SearchAPIApi()
val cloudProductControllerIndexDocsRequest : CloudProductControllerIndexDocsRequest =  // CloudProductControllerIndexDocsRequest | 
val store : kotlin.String = store_example // kotlin.String | Optional store/index selector (e.g. bot-docs).
try {
    val result : kotlin.Any = apiInstance.cloudProductControllerIndexDocs(cloudProductControllerIndexDocsRequest, store)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchAPIApi#cloudProductControllerIndexDocs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchAPIApi#cloudProductControllerIndexDocs")
    e.printStackTrace()
}
```

### Parameters
| **cloudProductControllerIndexDocsRequest** | [**CloudProductControllerIndexDocsRequest**](CloudProductControllerIndexDocsRequest.md)|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **store** | **kotlin.String**| Optional store/index selector (e.g. bot-docs). | [optional] |

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

<a id="cloudProductControllerSearchDocs"></a>
# **cloudProductControllerSearchDocs**
> kotlin.collections.List&lt;kotlin.Any&gt; cloudProductControllerSearchDocs(cloudProductControllerSearchDocsRequest, store)



Hybrid full-text + vector search over an indexed document store.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SearchAPIApi()
val cloudProductControllerSearchDocsRequest : CloudProductControllerSearchDocsRequest =  // CloudProductControllerSearchDocsRequest | 
val store : kotlin.String = store_example // kotlin.String | Optional store/index selector (e.g. bot-docs).
try {
    val result : kotlin.collections.List<kotlin.Any> = apiInstance.cloudProductControllerSearchDocs(cloudProductControllerSearchDocsRequest, store)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchAPIApi#cloudProductControllerSearchDocs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchAPIApi#cloudProductControllerSearchDocs")
    e.printStackTrace()
}
```

### Parameters
| **cloudProductControllerSearchDocsRequest** | [**CloudProductControllerSearchDocsRequest**](CloudProductControllerSearchDocsRequest.md)|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **store** | **kotlin.String**| Optional store/index selector (e.g. bot-docs). | [optional] |

### Return type

[**kotlin.collections.List&lt;kotlin.Any&gt;**](kotlin.Any.md)

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

