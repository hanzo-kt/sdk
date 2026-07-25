# OAuthApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatGetOauthApple**](OAuthApi.md#chatGetOauthApple) | **GET** /oauth/apple | Initiate Apple OAuth |
| [**chatGetOauthDiscord**](OAuthApi.md#chatGetOauthDiscord) | **GET** /oauth/discord | Initiate Discord OAuth |
| [**chatGetOauthDiscordCallback**](OAuthApi.md#chatGetOauthDiscordCallback) | **GET** /oauth/discord/callback | Discord OAuth callback |
| [**chatGetOauthError**](OAuthApi.md#chatGetOauthError) | **GET** /oauth/error | OAuth error handler |
| [**chatGetOauthFacebook**](OAuthApi.md#chatGetOauthFacebook) | **GET** /oauth/facebook | Initiate Facebook OAuth |
| [**chatGetOauthFacebookCallback**](OAuthApi.md#chatGetOauthFacebookCallback) | **GET** /oauth/facebook/callback | Facebook OAuth callback |
| [**chatGetOauthGithub**](OAuthApi.md#chatGetOauthGithub) | **GET** /oauth/github | Initiate GitHub OAuth |
| [**chatGetOauthGithubCallback**](OAuthApi.md#chatGetOauthGithubCallback) | **GET** /oauth/github/callback | GitHub OAuth callback |
| [**chatGetOauthGoogle**](OAuthApi.md#chatGetOauthGoogle) | **GET** /oauth/google | Initiate Google OAuth |
| [**chatGetOauthGoogleCallback**](OAuthApi.md#chatGetOauthGoogleCallback) | **GET** /oauth/google/callback | Google OAuth callback |
| [**chatGetOauthOpenid**](OAuthApi.md#chatGetOauthOpenid) | **GET** /oauth/openid | Initiate OpenID Connect login |
| [**chatGetOauthOpenidCallback**](OAuthApi.md#chatGetOauthOpenidCallback) | **GET** /oauth/openid/callback | OpenID Connect callback |
| [**chatGetOauthSaml**](OAuthApi.md#chatGetOauthSaml) | **GET** /oauth/saml | Initiate SAML login |
| [**chatPostOauthAppleCallback**](OAuthApi.md#chatPostOauthAppleCallback) | **POST** /oauth/apple/callback | Apple OAuth callback |
| [**chatPostOauthSamlCallback**](OAuthApi.md#chatPostOauthSamlCallback) | **POST** /oauth/saml/callback | SAML callback |
| [**integrationsConnectProvider**](OAuthApi.md#integrationsConnectProvider) | **POST** /v1/integrations/{provider}/connect | Begin an OAuth flow (returns the provider authorize URL) |
| [**integrationsDisconnectProvider**](OAuthApi.md#integrationsDisconnectProvider) | **POST** /v1/integrations/{provider}/disconnect | Revoke and forget an org&#39;s connection (idempotent) |
| [**integrationsProviderCallback**](OAuthApi.md#integrationsProviderCallback) | **GET** /v1/integrations/{provider}/callback | OAuth return — seal tokens and redirect to console |


<a id="chatGetOauthApple"></a>
# **chatGetOauthApple**
> chatGetOauthApple()

Initiate Apple OAuth

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OAuthApi()
try {
    apiInstance.chatGetOauthApple()
} catch (e: ClientException) {
    println("4xx response calling OAuthApi#chatGetOauthApple")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OAuthApi#chatGetOauthApple")
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

<a id="chatGetOauthDiscord"></a>
# **chatGetOauthDiscord**
> chatGetOauthDiscord()

Initiate Discord OAuth

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OAuthApi()
try {
    apiInstance.chatGetOauthDiscord()
} catch (e: ClientException) {
    println("4xx response calling OAuthApi#chatGetOauthDiscord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OAuthApi#chatGetOauthDiscord")
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

<a id="chatGetOauthDiscordCallback"></a>
# **chatGetOauthDiscordCallback**
> chatGetOauthDiscordCallback()

Discord OAuth callback

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OAuthApi()
try {
    apiInstance.chatGetOauthDiscordCallback()
} catch (e: ClientException) {
    println("4xx response calling OAuthApi#chatGetOauthDiscordCallback")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OAuthApi#chatGetOauthDiscordCallback")
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

<a id="chatGetOauthError"></a>
# **chatGetOauthError**
> chatGetOauthError()

OAuth error handler

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OAuthApi()
try {
    apiInstance.chatGetOauthError()
} catch (e: ClientException) {
    println("4xx response calling OAuthApi#chatGetOauthError")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OAuthApi#chatGetOauthError")
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

<a id="chatGetOauthFacebook"></a>
# **chatGetOauthFacebook**
> chatGetOauthFacebook()

Initiate Facebook OAuth

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OAuthApi()
try {
    apiInstance.chatGetOauthFacebook()
} catch (e: ClientException) {
    println("4xx response calling OAuthApi#chatGetOauthFacebook")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OAuthApi#chatGetOauthFacebook")
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

<a id="chatGetOauthFacebookCallback"></a>
# **chatGetOauthFacebookCallback**
> chatGetOauthFacebookCallback()

Facebook OAuth callback

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OAuthApi()
try {
    apiInstance.chatGetOauthFacebookCallback()
} catch (e: ClientException) {
    println("4xx response calling OAuthApi#chatGetOauthFacebookCallback")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OAuthApi#chatGetOauthFacebookCallback")
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

<a id="chatGetOauthGithub"></a>
# **chatGetOauthGithub**
> chatGetOauthGithub()

Initiate GitHub OAuth

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OAuthApi()
try {
    apiInstance.chatGetOauthGithub()
} catch (e: ClientException) {
    println("4xx response calling OAuthApi#chatGetOauthGithub")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OAuthApi#chatGetOauthGithub")
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

<a id="chatGetOauthGithubCallback"></a>
# **chatGetOauthGithubCallback**
> chatGetOauthGithubCallback()

GitHub OAuth callback

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OAuthApi()
try {
    apiInstance.chatGetOauthGithubCallback()
} catch (e: ClientException) {
    println("4xx response calling OAuthApi#chatGetOauthGithubCallback")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OAuthApi#chatGetOauthGithubCallback")
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

<a id="chatGetOauthGoogle"></a>
# **chatGetOauthGoogle**
> chatGetOauthGoogle()

Initiate Google OAuth

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OAuthApi()
try {
    apiInstance.chatGetOauthGoogle()
} catch (e: ClientException) {
    println("4xx response calling OAuthApi#chatGetOauthGoogle")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OAuthApi#chatGetOauthGoogle")
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

<a id="chatGetOauthGoogleCallback"></a>
# **chatGetOauthGoogleCallback**
> chatGetOauthGoogleCallback()

Google OAuth callback

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OAuthApi()
try {
    apiInstance.chatGetOauthGoogleCallback()
} catch (e: ClientException) {
    println("4xx response calling OAuthApi#chatGetOauthGoogleCallback")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OAuthApi#chatGetOauthGoogleCallback")
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

<a id="chatGetOauthOpenid"></a>
# **chatGetOauthOpenid**
> chatGetOauthOpenid()

Initiate OpenID Connect login

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OAuthApi()
try {
    apiInstance.chatGetOauthOpenid()
} catch (e: ClientException) {
    println("4xx response calling OAuthApi#chatGetOauthOpenid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OAuthApi#chatGetOauthOpenid")
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

<a id="chatGetOauthOpenidCallback"></a>
# **chatGetOauthOpenidCallback**
> chatGetOauthOpenidCallback()

OpenID Connect callback

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OAuthApi()
try {
    apiInstance.chatGetOauthOpenidCallback()
} catch (e: ClientException) {
    println("4xx response calling OAuthApi#chatGetOauthOpenidCallback")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OAuthApi#chatGetOauthOpenidCallback")
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

<a id="chatGetOauthSaml"></a>
# **chatGetOauthSaml**
> chatGetOauthSaml()

Initiate SAML login

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OAuthApi()
try {
    apiInstance.chatGetOauthSaml()
} catch (e: ClientException) {
    println("4xx response calling OAuthApi#chatGetOauthSaml")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OAuthApi#chatGetOauthSaml")
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

<a id="chatPostOauthAppleCallback"></a>
# **chatPostOauthAppleCallback**
> chatPostOauthAppleCallback()

Apple OAuth callback

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OAuthApi()
try {
    apiInstance.chatPostOauthAppleCallback()
} catch (e: ClientException) {
    println("4xx response calling OAuthApi#chatPostOauthAppleCallback")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OAuthApi#chatPostOauthAppleCallback")
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

<a id="chatPostOauthSamlCallback"></a>
# **chatPostOauthSamlCallback**
> chatPostOauthSamlCallback()

SAML callback

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OAuthApi()
try {
    apiInstance.chatPostOauthSamlCallback()
} catch (e: ClientException) {
    println("4xx response calling OAuthApi#chatPostOauthSamlCallback")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OAuthApi#chatPostOauthSamlCallback")
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

<a id="integrationsConnectProvider"></a>
# **integrationsConnectProvider**
> IntegrationsConnectProvider200Response integrationsConnectProvider(provider)

Begin an OAuth flow (returns the provider authorize URL)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OAuthApi()
val provider : kotlin.String = provider_example // kotlin.String | 
try {
    val result : IntegrationsConnectProvider200Response = apiInstance.integrationsConnectProvider(provider)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OAuthApi#integrationsConnectProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OAuthApi#integrationsConnectProvider")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **provider** | **kotlin.String**|  | |

### Return type

[**IntegrationsConnectProvider200Response**](IntegrationsConnectProvider200Response.md)

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

<a id="integrationsDisconnectProvider"></a>
# **integrationsDisconnectProvider**
> IntegrationsDisconnectProvider200Response integrationsDisconnectProvider(provider)

Revoke and forget an org&#39;s connection (idempotent)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OAuthApi()
val provider : kotlin.String = provider_example // kotlin.String | 
try {
    val result : IntegrationsDisconnectProvider200Response = apiInstance.integrationsDisconnectProvider(provider)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OAuthApi#integrationsDisconnectProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OAuthApi#integrationsDisconnectProvider")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **provider** | **kotlin.String**|  | |

### Return type

[**IntegrationsDisconnectProvider200Response**](IntegrationsDisconnectProvider200Response.md)

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

<a id="integrationsProviderCallback"></a>
# **integrationsProviderCallback**
> integrationsProviderCallback(provider, state, code, error)

OAuth return — seal tokens and redirect to console

Public, state-authed. The org comes only from the signed, single-use state. Always 302s back to the console (success or labeled failure).

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OAuthApi()
val provider : kotlin.String = provider_example // kotlin.String | 
val state : kotlin.String = state_example // kotlin.String | 
val code : kotlin.String = code_example // kotlin.String | 
val error : kotlin.String = error_example // kotlin.String | 
try {
    apiInstance.integrationsProviderCallback(provider, state, code, error)
} catch (e: ClientException) {
    println("4xx response calling OAuthApi#integrationsProviderCallback")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OAuthApi#integrationsProviderCallback")
    e.printStackTrace()
}
```

### Parameters
| **provider** | **kotlin.String**|  | |
| **state** | **kotlin.String**|  | |
| **code** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **error** | **kotlin.String**|  | [optional] |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

