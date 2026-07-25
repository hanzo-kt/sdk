# AccessTokensApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**commerceCreateAccessToken**](AccessTokensApi.md#commerceCreateAccessToken) | **POST** /v1/commerce/access/{mode}/{id} | Create or delete access token |
| [**commerceDeleteAccessToken**](AccessTokensApi.md#commerceDeleteAccessToken) | **DELETE** /v1/commerce/access/{mode}/{id} | Delete access token |
| [**commerceGetAccessToken**](AccessTokensApi.md#commerceGetAccessToken) | **GET** /v1/commerce/access/{mode}/{id} | Get access token |


<a id="commerceCreateAccessToken"></a>
# **commerceCreateAccessToken**
> kotlin.Any commerceCreateAccessToken(mode, id)

Create or delete access token

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AccessTokensApi()
val mode : kotlin.String = mode_example // kotlin.String | 
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.commerceCreateAccessToken(mode, id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccessTokensApi#commerceCreateAccessToken")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccessTokensApi#commerceCreateAccessToken")
    e.printStackTrace()
}
```

### Parameters
| **mode** | **kotlin.String**|  | [enum: live, test] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

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

<a id="commerceDeleteAccessToken"></a>
# **commerceDeleteAccessToken**
> commerceDeleteAccessToken(mode, id)

Delete access token

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AccessTokensApi()
val mode : kotlin.String = mode_example // kotlin.String | 
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.commerceDeleteAccessToken(mode, id)
} catch (e: ClientException) {
    println("4xx response calling AccessTokensApi#commerceDeleteAccessToken")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccessTokensApi#commerceDeleteAccessToken")
    e.printStackTrace()
}
```

### Parameters
| **mode** | **kotlin.String**|  | [enum: live, test] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

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
 - **Accept**: application/json

<a id="commerceGetAccessToken"></a>
# **commerceGetAccessToken**
> CommerceAccessToken commerceGetAccessToken(mode, id, email, password)

Get access token

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AccessTokensApi()
val mode : kotlin.String = mode_example // kotlin.String | 
val id : kotlin.String = id_example // kotlin.String | 
val email : kotlin.String = email_example // kotlin.String | 
val password : kotlin.String = password_example // kotlin.String | 
try {
    val result : CommerceAccessToken = apiInstance.commerceGetAccessToken(mode, id, email, password)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccessTokensApi#commerceGetAccessToken")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccessTokensApi#commerceGetAccessToken")
    e.printStackTrace()
}
```

### Parameters
| **mode** | **kotlin.String**|  | [enum: live, test] |
| **id** | **kotlin.String**|  | |
| **email** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **password** | **kotlin.String**|  | [optional] |

### Return type

[**CommerceAccessToken**](CommerceAccessToken.md)

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

