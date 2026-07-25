# ListApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**kvListPop**](ListApi.md#kvListPop) | **POST** /v1/kv/list/{key}/pop | Pop from list |
| [**kvListPush**](ListApi.md#kvListPush) | **POST** /v1/kv/list/{key}/push | Push to list |
| [**kvListRange**](ListApi.md#kvListRange) | **GET** /v1/kv/list/{key} | Get list range |


<a id="kvListPop"></a>
# **kvListPop**
> KvListPop200Response kvListPop(key, namespace, kvListPopRequest)

Pop from list

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ListApi()
val key : kotlin.String = key_example // kotlin.String | 
val namespace : kotlin.String = namespace_example // kotlin.String | 
val kvListPopRequest : KvListPopRequest =  // KvListPopRequest | 
try {
    val result : KvListPop200Response = apiInstance.kvListPop(key, namespace, kvListPopRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ListApi#kvListPop")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ListApi#kvListPop")
    e.printStackTrace()
}
```

### Parameters
| **key** | **kotlin.String**|  | |
| **namespace** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kvListPopRequest** | [**KvListPopRequest**](KvListPopRequest.md)|  | [optional] |

### Return type

[**KvListPop200Response**](KvListPop200Response.md)

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

<a id="kvListPush"></a>
# **kvListPush**
> KvListPush200Response kvListPush(key, kvListPushRequest, namespace)

Push to list

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ListApi()
val key : kotlin.String = key_example // kotlin.String | 
val kvListPushRequest : KvListPushRequest =  // KvListPushRequest | 
val namespace : kotlin.String = namespace_example // kotlin.String | 
try {
    val result : KvListPush200Response = apiInstance.kvListPush(key, kvListPushRequest, namespace)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ListApi#kvListPush")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ListApi#kvListPush")
    e.printStackTrace()
}
```

### Parameters
| **key** | **kotlin.String**|  | |
| **kvListPushRequest** | [**KvListPushRequest**](KvListPushRequest.md)|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **namespace** | **kotlin.String**|  | [optional] |

### Return type

[**KvListPush200Response**](KvListPush200Response.md)

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

<a id="kvListRange"></a>
# **kvListRange**
> KvListRange200Response kvListRange(key, start, stop, namespace)

Get list range

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ListApi()
val key : kotlin.String = key_example // kotlin.String | 
val start : kotlin.Int = 56 // kotlin.Int | 
val stop : kotlin.Int = 56 // kotlin.Int | 
val namespace : kotlin.String = namespace_example // kotlin.String | 
try {
    val result : KvListRange200Response = apiInstance.kvListRange(key, start, stop, namespace)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ListApi#kvListRange")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ListApi#kvListRange")
    e.printStackTrace()
}
```

### Parameters
| **key** | **kotlin.String**|  | |
| **start** | **kotlin.Int**|  | [optional] [default to 0] |
| **stop** | **kotlin.Int**|  | [optional] [default to -1] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **namespace** | **kotlin.String**|  | [optional] |

### Return type

[**KvListRange200Response**](KvListRange200Response.md)

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

