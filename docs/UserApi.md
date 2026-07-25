# UserApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatDeleteUserDelete**](UserApi.md#chatDeleteUserDelete) | **DELETE** /v1/chat/user/delete | Delete user account |
| [**chatGetUser**](UserApi.md#chatGetUser) | **GET** /v1/chat/user | Get current user |
| [**chatGetUserTerms**](UserApi.md#chatGetUserTerms) | **GET** /v1/chat/user/terms | Get terms acceptance status |
| [**chatPostUserPlugins**](UserApi.md#chatPostUserPlugins) | **POST** /v1/chat/user/plugins | Update user plugins |
| [**chatPostUserTermsAccept**](UserApi.md#chatPostUserTermsAccept) | **POST** /v1/chat/user/terms/accept | Accept terms of service |
| [**chatPostUserVerify**](UserApi.md#chatPostUserVerify) | **POST** /v1/chat/user/verify | Verify email with token |
| [**chatPostUserVerifyResend**](UserApi.md#chatPostUserVerifyResend) | **POST** /v1/chat/user/verify/resend | Resend verification email |
| [**platformUserAll**](UserApi.md#platformUserAll) | **GET** /v1/platform/user/all | List all users (admin only) |
| [**platformUserCreateApiKey**](UserApi.md#platformUserCreateApiKey) | **POST** /v1/platform/user/createApiKey | Create an API key |
| [**platformUserDeleteApiKey**](UserApi.md#platformUserDeleteApiKey) | **POST** /v1/platform/user/deleteApiKey | Delete an API key |
| [**platformUserGet**](UserApi.md#platformUserGet) | **GET** /v1/platform/user/get | Get current authenticated user |


<a id="chatDeleteUserDelete"></a>
# **chatDeleteUserDelete**
> kotlin.Any chatDeleteUserDelete()

Delete user account

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UserApi()
try {
    val result : kotlin.Any = apiInstance.chatDeleteUserDelete()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UserApi#chatDeleteUserDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserApi#chatDeleteUserDelete")
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

<a id="chatGetUser"></a>
# **chatGetUser**
> ChatUser chatGetUser()

Get current user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UserApi()
try {
    val result : ChatUser = apiInstance.chatGetUser()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UserApi#chatGetUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserApi#chatGetUser")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ChatUser**](ChatUser.md)

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

<a id="chatGetUserTerms"></a>
# **chatGetUserTerms**
> kotlin.Any chatGetUserTerms()

Get terms acceptance status

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UserApi()
try {
    val result : kotlin.Any = apiInstance.chatGetUserTerms()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UserApi#chatGetUserTerms")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserApi#chatGetUserTerms")
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

<a id="chatPostUserPlugins"></a>
# **chatPostUserPlugins**
> kotlin.Any chatPostUserPlugins(chatPostUserPluginsRequest)

Update user plugins

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UserApi()
val chatPostUserPluginsRequest : ChatPostUserPluginsRequest =  // ChatPostUserPluginsRequest | 
try {
    val result : kotlin.Any = apiInstance.chatPostUserPlugins(chatPostUserPluginsRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UserApi#chatPostUserPlugins")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserApi#chatPostUserPlugins")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostUserPluginsRequest** | [**ChatPostUserPluginsRequest**](ChatPostUserPluginsRequest.md)|  | |

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

<a id="chatPostUserTermsAccept"></a>
# **chatPostUserTermsAccept**
> kotlin.Any chatPostUserTermsAccept()

Accept terms of service

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UserApi()
try {
    val result : kotlin.Any = apiInstance.chatPostUserTermsAccept()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UserApi#chatPostUserTermsAccept")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserApi#chatPostUserTermsAccept")
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

<a id="chatPostUserVerify"></a>
# **chatPostUserVerify**
> kotlin.Any chatPostUserVerify(chatPostUserVerifyRequest)

Verify email with token

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UserApi()
val chatPostUserVerifyRequest : ChatPostUserVerifyRequest =  // ChatPostUserVerifyRequest | 
try {
    val result : kotlin.Any = apiInstance.chatPostUserVerify(chatPostUserVerifyRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UserApi#chatPostUserVerify")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserApi#chatPostUserVerify")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostUserVerifyRequest** | [**ChatPostUserVerifyRequest**](ChatPostUserVerifyRequest.md)|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="chatPostUserVerifyResend"></a>
# **chatPostUserVerifyResend**
> kotlin.Any chatPostUserVerifyResend(chatPostUserVerifyResendRequest)

Resend verification email

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UserApi()
val chatPostUserVerifyResendRequest : ChatPostUserVerifyResendRequest =  // ChatPostUserVerifyResendRequest | 
try {
    val result : kotlin.Any = apiInstance.chatPostUserVerifyResend(chatPostUserVerifyResendRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UserApi#chatPostUserVerifyResend")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserApi#chatPostUserVerifyResend")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostUserVerifyResendRequest** | [**ChatPostUserVerifyResendRequest**](ChatPostUserVerifyResendRequest.md)|  | [optional] |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="platformUserAll"></a>
# **platformUserAll**
> PlatformTRPCResult platformUserAll()

List all users (admin only)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UserApi()
try {
    val result : PlatformTRPCResult = apiInstance.platformUserAll()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UserApi#platformUserAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserApi#platformUserAll")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PlatformTRPCResult**](PlatformTRPCResult.md)

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

<a id="platformUserCreateApiKey"></a>
# **platformUserCreateApiKey**
> PlatformTRPCResult platformUserCreateApiKey(platformUserCreateApiKeyRequest)

Create an API key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UserApi()
val platformUserCreateApiKeyRequest : PlatformUserCreateApiKeyRequest =  // PlatformUserCreateApiKeyRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformUserCreateApiKey(platformUserCreateApiKeyRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UserApi#platformUserCreateApiKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserApi#platformUserCreateApiKey")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformUserCreateApiKeyRequest** | [**PlatformUserCreateApiKeyRequest**](PlatformUserCreateApiKeyRequest.md)|  | |

### Return type

[**PlatformTRPCResult**](PlatformTRPCResult.md)

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

<a id="platformUserDeleteApiKey"></a>
# **platformUserDeleteApiKey**
> PlatformTRPCResult platformUserDeleteApiKey(platformUserDeleteApiKeyRequest)

Delete an API key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UserApi()
val platformUserDeleteApiKeyRequest : PlatformUserDeleteApiKeyRequest =  // PlatformUserDeleteApiKeyRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformUserDeleteApiKey(platformUserDeleteApiKeyRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UserApi#platformUserDeleteApiKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserApi#platformUserDeleteApiKey")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformUserDeleteApiKeyRequest** | [**PlatformUserDeleteApiKeyRequest**](PlatformUserDeleteApiKeyRequest.md)|  | |

### Return type

[**PlatformTRPCResult**](PlatformTRPCResult.md)

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

<a id="platformUserGet"></a>
# **platformUserGet**
> PlatformTRPCResult platformUserGet()

Get current authenticated user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UserApi()
try {
    val result : PlatformTRPCResult = apiInstance.platformUserGet()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UserApi#platformUserGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserApi#platformUserGet")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PlatformTRPCResult**](PlatformTRPCResult.md)

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

