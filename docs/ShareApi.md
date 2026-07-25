# ShareApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**analyticsGetSharedWebsite**](ShareApi.md#analyticsGetSharedWebsite) | **GET** /v1/analytics/share/{shareId} | Get a shared website by share ID (no auth required) |
| [**chatDeleteShareByshareid**](ShareApi.md#chatDeleteShareByshareid) | **DELETE** /v1/chat/share/{shareId} | Delete a shared link |
| [**chatGetShare**](ShareApi.md#chatGetShare) | **GET** /v1/chat/share | List shared links |
| [**chatGetShareByshareid**](ShareApi.md#chatGetShareByshareid) | **GET** /v1/chat/share/{shareId} | Get shared conversation messages |
| [**chatGetShareLinkByconversationid**](ShareApi.md#chatGetShareLinkByconversationid) | **GET** /v1/chat/share/link/{conversationId} | Get shared link for a conversation |
| [**chatPatchShareByshareid**](ShareApi.md#chatPatchShareByshareid) | **PATCH** /v1/chat/share/{shareId} | Update a shared link |
| [**chatPostShareByconversationid**](ShareApi.md#chatPostShareByconversationid) | **POST** /v1/chat/share/{conversationId} | Create a shared link |


<a id="analyticsGetSharedWebsite"></a>
# **analyticsGetSharedWebsite**
> AnalyticsGetSharedWebsite200Response analyticsGetSharedWebsite(shareId)

Get a shared website by share ID (no auth required)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ShareApi()
val shareId : kotlin.String = shareId_example // kotlin.String | 
try {
    val result : AnalyticsGetSharedWebsite200Response = apiInstance.analyticsGetSharedWebsite(shareId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShareApi#analyticsGetSharedWebsite")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShareApi#analyticsGetSharedWebsite")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shareId** | **kotlin.String**|  | |

### Return type

[**AnalyticsGetSharedWebsite200Response**](AnalyticsGetSharedWebsite200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="chatDeleteShareByshareid"></a>
# **chatDeleteShareByshareid**
> kotlin.Any chatDeleteShareByshareid(shareId)

Delete a shared link

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ShareApi()
val shareId : kotlin.String = shareId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatDeleteShareByshareid(shareId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShareApi#chatDeleteShareByshareid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShareApi#chatDeleteShareByshareid")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shareId** | **kotlin.String**|  | |

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

<a id="chatGetShare"></a>
# **chatGetShare**
> ChatGetShare200Response chatGetShare(cursor, pageSize, isPublic, sortBy, sortDirection, search)

List shared links

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ShareApi()
val cursor : kotlin.String = cursor_example // kotlin.String | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val isPublic : kotlin.String = isPublic_example // kotlin.String | 
val sortBy : kotlin.String = sortBy_example // kotlin.String | 
val sortDirection : kotlin.String = sortDirection_example // kotlin.String | 
val search : kotlin.String = search_example // kotlin.String | 
try {
    val result : ChatGetShare200Response = apiInstance.chatGetShare(cursor, pageSize, isPublic, sortBy, sortDirection, search)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShareApi#chatGetShare")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShareApi#chatGetShare")
    e.printStackTrace()
}
```

### Parameters
| **cursor** | **kotlin.String**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] [default to 10] |
| **isPublic** | **kotlin.String**|  | [optional] |
| **sortBy** | **kotlin.String**|  | [optional] [default to &quot;createdAt&quot;] |
| **sortDirection** | **kotlin.String**|  | [optional] [default to &quot;desc&quot;] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **search** | **kotlin.String**|  | [optional] |

### Return type

[**ChatGetShare200Response**](ChatGetShare200Response.md)

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

<a id="chatGetShareByshareid"></a>
# **chatGetShareByshareid**
> kotlin.Any chatGetShareByshareid(shareId)

Get shared conversation messages

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ShareApi()
val shareId : kotlin.String = shareId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatGetShareByshareid(shareId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShareApi#chatGetShareByshareid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShareApi#chatGetShareByshareid")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shareId** | **kotlin.String**|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="chatGetShareLinkByconversationid"></a>
# **chatGetShareLinkByconversationid**
> ChatGetShareLinkByconversationid200Response chatGetShareLinkByconversationid(conversationId)

Get shared link for a conversation

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ShareApi()
val conversationId : kotlin.String = conversationId_example // kotlin.String | 
try {
    val result : ChatGetShareLinkByconversationid200Response = apiInstance.chatGetShareLinkByconversationid(conversationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShareApi#chatGetShareLinkByconversationid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShareApi#chatGetShareLinkByconversationid")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **conversationId** | **kotlin.String**|  | |

### Return type

[**ChatGetShareLinkByconversationid200Response**](ChatGetShareLinkByconversationid200Response.md)

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

<a id="chatPatchShareByshareid"></a>
# **chatPatchShareByshareid**
> kotlin.Any chatPatchShareByshareid(shareId)

Update a shared link

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ShareApi()
val shareId : kotlin.String = shareId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatPatchShareByshareid(shareId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShareApi#chatPatchShareByshareid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShareApi#chatPatchShareByshareid")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shareId** | **kotlin.String**|  | |

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

<a id="chatPostShareByconversationid"></a>
# **chatPostShareByconversationid**
> kotlin.Any chatPostShareByconversationid(conversationId, chatPostShareByconversationidRequest)

Create a shared link

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ShareApi()
val conversationId : kotlin.String = conversationId_example // kotlin.String | 
val chatPostShareByconversationidRequest : ChatPostShareByconversationidRequest =  // ChatPostShareByconversationidRequest | 
try {
    val result : kotlin.Any = apiInstance.chatPostShareByconversationid(conversationId, chatPostShareByconversationidRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShareApi#chatPostShareByconversationid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShareApi#chatPostShareByconversationid")
    e.printStackTrace()
}
```

### Parameters
| **conversationId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostShareByconversationidRequest** | [**ChatPostShareByconversationidRequest**](ChatPostShareByconversationidRequest.md)|  | [optional] |

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

