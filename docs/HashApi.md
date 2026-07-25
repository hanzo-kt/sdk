# HashApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**kvHashDeleteField**](HashApi.md#kvHashDeleteField) | **DELETE** /v1/kv/hash/{key}/{field} | Delete hash field |
| [**kvHashGetAll**](HashApi.md#kvHashGetAll) | **GET** /v1/kv/hash/{key} | Get all hash fields |
| [**kvHashGetField**](HashApi.md#kvHashGetField) | **GET** /v1/kv/hash/{key}/{field} | Get hash field |
| [**kvHashSet**](HashApi.md#kvHashSet) | **PUT** /v1/kv/hash/{key} | Set hash fields |


<a id="kvHashDeleteField"></a>
# **kvHashDeleteField**
> kotlin.Any kvHashDeleteField(key, `field`, namespace)

Delete hash field

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = HashApi()
val key : kotlin.String = key_example // kotlin.String | 
val `field` : kotlin.String = `field`_example // kotlin.String | 
val namespace : kotlin.String = namespace_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.kvHashDeleteField(key, `field`, namespace)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling HashApi#kvHashDeleteField")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HashApi#kvHashDeleteField")
    e.printStackTrace()
}
```

### Parameters
| **key** | **kotlin.String**|  | |
| **&#x60;field&#x60;** | **kotlin.String**|  | |
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

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="kvHashGetAll"></a>
# **kvHashGetAll**
> kotlin.collections.Map&lt;kotlin.String, kotlin.String&gt; kvHashGetAll(key, namespace)

Get all hash fields

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = HashApi()
val key : kotlin.String = key_example // kotlin.String | 
val namespace : kotlin.String = namespace_example // kotlin.String | 
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.String> = apiInstance.kvHashGetAll(key, namespace)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling HashApi#kvHashGetAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HashApi#kvHashGetAll")
    e.printStackTrace()
}
```

### Parameters
| **key** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **namespace** | **kotlin.String**|  | [optional] |

### Return type

**kotlin.collections.Map&lt;kotlin.String, kotlin.String&gt;**

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

<a id="kvHashGetField"></a>
# **kvHashGetField**
> KmsKmsGetOrgSecret200ResponseSecret kvHashGetField(key, `field`, namespace)

Get hash field

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = HashApi()
val key : kotlin.String = key_example // kotlin.String | 
val `field` : kotlin.String = `field`_example // kotlin.String | 
val namespace : kotlin.String = namespace_example // kotlin.String | 
try {
    val result : KmsKmsGetOrgSecret200ResponseSecret = apiInstance.kvHashGetField(key, `field`, namespace)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling HashApi#kvHashGetField")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HashApi#kvHashGetField")
    e.printStackTrace()
}
```

### Parameters
| **key** | **kotlin.String**|  | |
| **&#x60;field&#x60;** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **namespace** | **kotlin.String**|  | [optional] |

### Return type

[**KmsKmsGetOrgSecret200ResponseSecret**](KmsKmsGetOrgSecret200ResponseSecret.md)

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

<a id="kvHashSet"></a>
# **kvHashSet**
> kotlin.Any kvHashSet(key, requestBody, namespace)

Set hash fields

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = HashApi()
val key : kotlin.String = key_example // kotlin.String | 
val requestBody : kotlin.collections.Map<kotlin.String, kotlin.String> = Object // kotlin.collections.Map<kotlin.String, kotlin.String> | 
val namespace : kotlin.String = namespace_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.kvHashSet(key, requestBody, namespace)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling HashApi#kvHashSet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HashApi#kvHashSet")
    e.printStackTrace()
}
```

### Parameters
| **key** | **kotlin.String**|  | |
| **requestBody** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.String&gt;**](kotlin.String.md)|  | |
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

