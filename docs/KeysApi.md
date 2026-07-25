# KeysApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatDeleteKeys**](KeysApi.md#chatDeleteKeys) | **DELETE** /v1/chat/keys | Delete all user keys |
| [**chatDeleteKeysByname**](KeysApi.md#chatDeleteKeysByname) | **DELETE** /v1/chat/keys/{name} | Delete a user key by name |
| [**chatGetKeys**](KeysApi.md#chatGetKeys) | **GET** /v1/chat/keys | Get user key expiry info |
| [**chatPutKeys**](KeysApi.md#chatPutKeys) | **PUT** /v1/chat/keys | Create or update a user API key |
| [**gatewayDeleteKey**](KeysApi.md#gatewayDeleteKey) | **POST** /v1/gateway/key/delete | Delete key |
| [**gatewayGenerateKey**](KeysApi.md#gatewayGenerateKey) | **POST** /v1/gateway/key/generate | Generate API key |
| [**gatewayGetKeyInfo**](KeysApi.md#gatewayGetKeyInfo) | **GET** /v1/gateway/key/info | Get key info |
| [**gatewayUpdateKey**](KeysApi.md#gatewayUpdateKey) | **POST** /v1/gateway/key/update | Update key |
| [**kvBatchOperation**](KeysApi.md#kvBatchOperation) | **POST** /v1/kv/batch | Batch get/set/delete |
| [**kvDeleteKey**](KeysApi.md#kvDeleteKey) | **DELETE** /v1/kv/keys/{key} | Delete key |
| [**kvGetKey**](KeysApi.md#kvGetKey) | **GET** /v1/kv/keys/{key} | Get key value |
| [**kvIncrKey**](KeysApi.md#kvIncrKey) | **POST** /v1/kv/keys/{key}/incr | Increment numeric key |
| [**kvScanKeys**](KeysApi.md#kvScanKeys) | **GET** /v1/kv/keys | Scan keys |
| [**kvSetKey**](KeysApi.md#kvSetKey) | **PUT** /v1/kv/keys/{key} | Set key value |
| [**kvSetKeyTTL**](KeysApi.md#kvSetKeyTTL) | **PUT** /v1/kv/keys/{key}/ttl | Set key TTL |
| [**searchCreateKey**](KeysApi.md#searchCreateKey) | **POST** /v1/search/keys | Create an API key |
| [**searchDeleteKey**](KeysApi.md#searchDeleteKey) | **DELETE** /v1/search/keys/{keyOrUid} | Delete an API key |
| [**searchGetKey**](KeysApi.md#searchGetKey) | **GET** /v1/search/keys/{keyOrUid} | Get an API key |
| [**searchListKeys**](KeysApi.md#searchListKeys) | **GET** /v1/search/keys | List API keys |
| [**searchUpdateKey**](KeysApi.md#searchUpdateKey) | **PATCH** /v1/search/keys/{keyOrUid} | Update an API key |


<a id="chatDeleteKeys"></a>
# **chatDeleteKeys**
> chatDeleteKeys(all)

Delete all user keys

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeysApi()
val all : kotlin.String = all_example // kotlin.String | 
try {
    apiInstance.chatDeleteKeys(all)
} catch (e: ClientException) {
    println("4xx response calling KeysApi#chatDeleteKeys")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeysApi#chatDeleteKeys")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **all** | **kotlin.String**|  | [enum: true] |

### Return type

null (empty response body)

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
 - **Accept**: Not defined

<a id="chatDeleteKeysByname"></a>
# **chatDeleteKeysByname**
> chatDeleteKeysByname(name)

Delete a user key by name

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeysApi()
val name : kotlin.String = name_example // kotlin.String | 
try {
    apiInstance.chatDeleteKeysByname(name)
} catch (e: ClientException) {
    println("4xx response calling KeysApi#chatDeleteKeysByname")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeysApi#chatDeleteKeysByname")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | |

### Return type

null (empty response body)

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
 - **Accept**: Not defined

<a id="chatGetKeys"></a>
# **chatGetKeys**
> kotlin.Any chatGetKeys(name)

Get user key expiry info

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeysApi()
val name : kotlin.String = name_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatGetKeys(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeysApi#chatGetKeys")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeysApi#chatGetKeys")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | [optional] |

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

<a id="chatPutKeys"></a>
# **chatPutKeys**
> kotlin.Any chatPutKeys(chatPutKeysRequest)

Create or update a user API key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeysApi()
val chatPutKeysRequest : ChatPutKeysRequest =  // ChatPutKeysRequest | 
try {
    val result : kotlin.Any = apiInstance.chatPutKeys(chatPutKeysRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeysApi#chatPutKeys")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeysApi#chatPutKeys")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPutKeysRequest** | [**ChatPutKeysRequest**](ChatPutKeysRequest.md)|  | |

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

<a id="gatewayDeleteKey"></a>
# **gatewayDeleteKey**
> kotlin.Any gatewayDeleteKey(gatewayDeleteKeyRequest)

Delete key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeysApi()
val gatewayDeleteKeyRequest : GatewayDeleteKeyRequest =  // GatewayDeleteKeyRequest | 
try {
    val result : kotlin.Any = apiInstance.gatewayDeleteKey(gatewayDeleteKeyRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeysApi#gatewayDeleteKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeysApi#gatewayDeleteKey")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **gatewayDeleteKeyRequest** | [**GatewayDeleteKeyRequest**](GatewayDeleteKeyRequest.md)|  | |

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

<a id="gatewayGenerateKey"></a>
# **gatewayGenerateKey**
> GatewayKey gatewayGenerateKey(gatewayGenerateKeyRequest)

Generate API key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeysApi()
val gatewayGenerateKeyRequest : GatewayGenerateKeyRequest =  // GatewayGenerateKeyRequest | 
try {
    val result : GatewayKey = apiInstance.gatewayGenerateKey(gatewayGenerateKeyRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeysApi#gatewayGenerateKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeysApi#gatewayGenerateKey")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **gatewayGenerateKeyRequest** | [**GatewayGenerateKeyRequest**](GatewayGenerateKeyRequest.md)|  | |

### Return type

[**GatewayKey**](GatewayKey.md)

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

<a id="gatewayGetKeyInfo"></a>
# **gatewayGetKeyInfo**
> GatewayKey gatewayGetKeyInfo(key)

Get key info

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeysApi()
val key : kotlin.String = key_example // kotlin.String | 
try {
    val result : GatewayKey = apiInstance.gatewayGetKeyInfo(key)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeysApi#gatewayGetKeyInfo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeysApi#gatewayGetKeyInfo")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key** | **kotlin.String**|  | [optional] |

### Return type

[**GatewayKey**](GatewayKey.md)

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

<a id="gatewayUpdateKey"></a>
# **gatewayUpdateKey**
> kotlin.Any gatewayUpdateKey(gatewayUpdateKeyRequest)

Update key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeysApi()
val gatewayUpdateKeyRequest : GatewayUpdateKeyRequest =  // GatewayUpdateKeyRequest | 
try {
    val result : kotlin.Any = apiInstance.gatewayUpdateKey(gatewayUpdateKeyRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeysApi#gatewayUpdateKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeysApi#gatewayUpdateKey")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **gatewayUpdateKeyRequest** | [**GatewayUpdateKeyRequest**](GatewayUpdateKeyRequest.md)|  | |

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

<a id="kvBatchOperation"></a>
# **kvBatchOperation**
> KvBatchOperation200Response kvBatchOperation(kvBatchOperationRequest)

Batch get/set/delete

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeysApi()
val kvBatchOperationRequest : KvBatchOperationRequest =  // KvBatchOperationRequest | 
try {
    val result : KvBatchOperation200Response = apiInstance.kvBatchOperation(kvBatchOperationRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeysApi#kvBatchOperation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeysApi#kvBatchOperation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kvBatchOperationRequest** | [**KvBatchOperationRequest**](KvBatchOperationRequest.md)|  | |

### Return type

[**KvBatchOperation200Response**](KvBatchOperation200Response.md)

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

<a id="kvDeleteKey"></a>
# **kvDeleteKey**
> KvDeleteKey200Response kvDeleteKey(key, namespace)

Delete key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeysApi()
val key : kotlin.String = key_example // kotlin.String | 
val namespace : kotlin.String = namespace_example // kotlin.String | 
try {
    val result : KvDeleteKey200Response = apiInstance.kvDeleteKey(key, namespace)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeysApi#kvDeleteKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeysApi#kvDeleteKey")
    e.printStackTrace()
}
```

### Parameters
| **key** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **namespace** | **kotlin.String**|  | [optional] |

### Return type

[**KvDeleteKey200Response**](KvDeleteKey200Response.md)

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

<a id="kvGetKey"></a>
# **kvGetKey**
> KvKeyValue kvGetKey(key, namespace)

Get key value

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeysApi()
val key : kotlin.String = key_example // kotlin.String | 
val namespace : kotlin.String = namespace_example // kotlin.String | 
try {
    val result : KvKeyValue = apiInstance.kvGetKey(key, namespace)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeysApi#kvGetKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeysApi#kvGetKey")
    e.printStackTrace()
}
```

### Parameters
| **key** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **namespace** | **kotlin.String**|  | [optional] |

### Return type

[**KvKeyValue**](KvKeyValue.md)

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

<a id="kvIncrKey"></a>
# **kvIncrKey**
> AnalyticsGetSessionStats200ResponseValue kvIncrKey(key, namespace, kvIncrKeyRequest)

Increment numeric key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeysApi()
val key : kotlin.String = key_example // kotlin.String | 
val namespace : kotlin.String = namespace_example // kotlin.String | 
val kvIncrKeyRequest : KvIncrKeyRequest =  // KvIncrKeyRequest | 
try {
    val result : AnalyticsGetSessionStats200ResponseValue = apiInstance.kvIncrKey(key, namespace, kvIncrKeyRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeysApi#kvIncrKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeysApi#kvIncrKey")
    e.printStackTrace()
}
```

### Parameters
| **key** | **kotlin.String**|  | |
| **namespace** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kvIncrKeyRequest** | [**KvIncrKeyRequest**](KvIncrKeyRequest.md)|  | [optional] |

### Return type

[**AnalyticsGetSessionStats200ResponseValue**](AnalyticsGetSessionStats200ResponseValue.md)

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

<a id="kvScanKeys"></a>
# **kvScanKeys**
> KvScanKeys200Response kvScanKeys(pattern, type, cursor, count, namespace)

Scan keys

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeysApi()
val pattern : kotlin.String = pattern_example // kotlin.String | Glob-style pattern (e.g. user:*, session:*)
val type : kotlin.String = type_example // kotlin.String | 
val cursor : kotlin.String = cursor_example // kotlin.String | 
val count : kotlin.Int = 56 // kotlin.Int | 
val namespace : kotlin.String = namespace_example // kotlin.String | 
try {
    val result : KvScanKeys200Response = apiInstance.kvScanKeys(pattern, type, cursor, count, namespace)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeysApi#kvScanKeys")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeysApi#kvScanKeys")
    e.printStackTrace()
}
```

### Parameters
| **pattern** | **kotlin.String**| Glob-style pattern (e.g. user:*, session:*) | [optional] [default to &quot;*&quot;] |
| **type** | **kotlin.String**|  | [optional] [enum: string, hash, list, set, zset, stream] |
| **cursor** | **kotlin.String**|  | [optional] [default to &quot;0&quot;] |
| **count** | **kotlin.Int**|  | [optional] [default to 100] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **namespace** | **kotlin.String**|  | [optional] |

### Return type

[**KvScanKeys200Response**](KvScanKeys200Response.md)

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

<a id="kvSetKey"></a>
# **kvSetKey**
> KvKeyValue kvSetKey(key, kvSetKeyRequest, namespace)

Set key value

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeysApi()
val key : kotlin.String = key_example // kotlin.String | 
val kvSetKeyRequest : KvSetKeyRequest =  // KvSetKeyRequest | 
val namespace : kotlin.String = namespace_example // kotlin.String | 
try {
    val result : KvKeyValue = apiInstance.kvSetKey(key, kvSetKeyRequest, namespace)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeysApi#kvSetKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeysApi#kvSetKey")
    e.printStackTrace()
}
```

### Parameters
| **key** | **kotlin.String**|  | |
| **kvSetKeyRequest** | [**KvSetKeyRequest**](KvSetKeyRequest.md)|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **namespace** | **kotlin.String**|  | [optional] |

### Return type

[**KvKeyValue**](KvKeyValue.md)

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

<a id="kvSetKeyTTL"></a>
# **kvSetKeyTTL**
> kotlin.Any kvSetKeyTTL(key, kvSetKeyTTLRequest, namespace)

Set key TTL

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeysApi()
val key : kotlin.String = key_example // kotlin.String | 
val kvSetKeyTTLRequest : KvSetKeyTTLRequest =  // KvSetKeyTTLRequest | 
val namespace : kotlin.String = namespace_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.kvSetKeyTTL(key, kvSetKeyTTLRequest, namespace)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeysApi#kvSetKeyTTL")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeysApi#kvSetKeyTTL")
    e.printStackTrace()
}
```

### Parameters
| **key** | **kotlin.String**|  | |
| **kvSetKeyTTLRequest** | [**KvSetKeyTTLRequest**](KvSetKeyTTLRequest.md)|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **namespace** | **kotlin.String**|  | [optional] |

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

<a id="searchCreateKey"></a>
# **searchCreateKey**
> SearchKeyView searchCreateKey(searchCreateApiKey)

Create an API key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeysApi()
val searchCreateApiKey : SearchCreateApiKey =  // SearchCreateApiKey | 
try {
    val result : SearchKeyView = apiInstance.searchCreateKey(searchCreateApiKey)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeysApi#searchCreateKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeysApi#searchCreateKey")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **searchCreateApiKey** | [**SearchCreateApiKey**](SearchCreateApiKey.md)|  | |

### Return type

[**SearchKeyView**](SearchKeyView.md)

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

<a id="searchDeleteKey"></a>
# **searchDeleteKey**
> searchDeleteKey(keyOrUid)

Delete an API key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeysApi()
val keyOrUid : kotlin.String = keyOrUid_example // kotlin.String | 
try {
    apiInstance.searchDeleteKey(keyOrUid)
} catch (e: ClientException) {
    println("4xx response calling KeysApi#searchDeleteKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeysApi#searchDeleteKey")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **keyOrUid** | **kotlin.String**|  | |

### Return type

null (empty response body)

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
 - **Accept**: Not defined

<a id="searchGetKey"></a>
# **searchGetKey**
> SearchKeyView searchGetKey(keyOrUid)

Get an API key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeysApi()
val keyOrUid : kotlin.String = keyOrUid_example // kotlin.String | 
try {
    val result : SearchKeyView = apiInstance.searchGetKey(keyOrUid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeysApi#searchGetKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeysApi#searchGetKey")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **keyOrUid** | **kotlin.String**|  | |

### Return type

[**SearchKeyView**](SearchKeyView.md)

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

<a id="searchListKeys"></a>
# **searchListKeys**
> SearchPaginatedKeys searchListKeys(offset, limit)

List API keys

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeysApi()
val offset : kotlin.Int = 56 // kotlin.Int | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : SearchPaginatedKeys = apiInstance.searchListKeys(offset, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeysApi#searchListKeys")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeysApi#searchListKeys")
    e.printStackTrace()
}
```

### Parameters
| **offset** | **kotlin.Int**|  | [optional] [default to 0] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] [default to 20] |

### Return type

[**SearchPaginatedKeys**](SearchPaginatedKeys.md)

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

<a id="searchUpdateKey"></a>
# **searchUpdateKey**
> SearchKeyView searchUpdateKey(keyOrUid, searchUpdateKeyRequest)

Update an API key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeysApi()
val keyOrUid : kotlin.String = keyOrUid_example // kotlin.String | 
val searchUpdateKeyRequest : SearchUpdateKeyRequest =  // SearchUpdateKeyRequest | 
try {
    val result : SearchKeyView = apiInstance.searchUpdateKey(keyOrUid, searchUpdateKeyRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeysApi#searchUpdateKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeysApi#searchUpdateKey")
    e.printStackTrace()
}
```

### Parameters
| **keyOrUid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **searchUpdateKeyRequest** | [**SearchUpdateKeyRequest**](SearchUpdateKeyRequest.md)|  | |

### Return type

[**SearchKeyView**](SearchKeyView.md)

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

