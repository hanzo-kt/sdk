# AdminAuthApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatGetAdminOauthOpenid**](AdminAuthApi.md#chatGetAdminOauthOpenid) | **GET** /v1/chat/admin/oauth/openid | Initiate admin OpenID login |
| [**chatGetAdminOauthOpenidCallback**](AdminAuthApi.md#chatGetAdminOauthOpenidCallback) | **GET** /v1/chat/admin/oauth/openid/callback | Admin OpenID callback |
| [**chatGetAdminOauthOpenidCheck**](AdminAuthApi.md#chatGetAdminOauthOpenidCheck) | **GET** /v1/chat/admin/oauth/openid/check | Check if OpenID is configured for admin |
| [**chatGetAdminVerify**](AdminAuthApi.md#chatGetAdminVerify) | **GET** /v1/chat/admin/verify | Verify admin session |
| [**chatPostAdminLoginLocal**](AdminAuthApi.md#chatPostAdminLoginLocal) | **POST** /v1/chat/admin/login/local | Admin local login |
| [**chatPostAdminOauthExchange**](AdminAuthApi.md#chatPostAdminOauthExchange) | **POST** /v1/chat/admin/oauth/exchange | Exchange OAuth code for admin tokens |


<a id="chatGetAdminOauthOpenid"></a>
# **chatGetAdminOauthOpenid**
> chatGetAdminOauthOpenid()

Initiate admin OpenID login

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminAuthApi()
try {
    apiInstance.chatGetAdminOauthOpenid()
} catch (e: ClientException) {
    println("4xx response calling AdminAuthApi#chatGetAdminOauthOpenid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminAuthApi#chatGetAdminOauthOpenid")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="chatGetAdminOauthOpenidCallback"></a>
# **chatGetAdminOauthOpenidCallback**
> chatGetAdminOauthOpenidCallback()

Admin OpenID callback

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminAuthApi()
try {
    apiInstance.chatGetAdminOauthOpenidCallback()
} catch (e: ClientException) {
    println("4xx response calling AdminAuthApi#chatGetAdminOauthOpenidCallback")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminAuthApi#chatGetAdminOauthOpenidCallback")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="chatGetAdminOauthOpenidCheck"></a>
# **chatGetAdminOauthOpenidCheck**
> kotlin.Any chatGetAdminOauthOpenidCheck()

Check if OpenID is configured for admin

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminAuthApi()
try {
    val result : kotlin.Any = apiInstance.chatGetAdminOauthOpenidCheck()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminAuthApi#chatGetAdminOauthOpenidCheck")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminAuthApi#chatGetAdminOauthOpenidCheck")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="chatGetAdminVerify"></a>
# **chatGetAdminVerify**
> ChatGetAdminVerify200Response chatGetAdminVerify()

Verify admin session

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminAuthApi()
try {
    val result : ChatGetAdminVerify200Response = apiInstance.chatGetAdminVerify()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminAuthApi#chatGetAdminVerify")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminAuthApi#chatGetAdminVerify")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ChatGetAdminVerify200Response**](ChatGetAdminVerify200Response.md)

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

<a id="chatPostAdminLoginLocal"></a>
# **chatPostAdminLoginLocal**
> kotlin.Any chatPostAdminLoginLocal(chatPostAdminLoginLocalRequest)

Admin local login

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminAuthApi()
val chatPostAdminLoginLocalRequest : ChatPostAdminLoginLocalRequest =  // ChatPostAdminLoginLocalRequest | 
try {
    val result : kotlin.Any = apiInstance.chatPostAdminLoginLocal(chatPostAdminLoginLocalRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminAuthApi#chatPostAdminLoginLocal")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminAuthApi#chatPostAdminLoginLocal")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostAdminLoginLocalRequest** | [**ChatPostAdminLoginLocalRequest**](ChatPostAdminLoginLocalRequest.md)|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="chatPostAdminOauthExchange"></a>
# **chatPostAdminOauthExchange**
> ChatPostAdminOauthExchange200Response chatPostAdminOauthExchange(chatPostAdminOauthExchangeRequest)

Exchange OAuth code for admin tokens

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminAuthApi()
val chatPostAdminOauthExchangeRequest : ChatPostAdminOauthExchangeRequest =  // ChatPostAdminOauthExchangeRequest | 
try {
    val result : ChatPostAdminOauthExchange200Response = apiInstance.chatPostAdminOauthExchange(chatPostAdminOauthExchangeRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminAuthApi#chatPostAdminOauthExchange")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminAuthApi#chatPostAdminOauthExchange")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostAdminOauthExchangeRequest** | [**ChatPostAdminOauthExchangeRequest**](ChatPostAdminOauthExchangeRequest.md)|  | |

### Return type

[**ChatPostAdminOauthExchange200Response**](ChatPostAdminOauthExchange200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

