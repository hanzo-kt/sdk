# AuthApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**analyticsGetTelemetryScript**](AuthApi.md#analyticsGetTelemetryScript) | **GET** /v1/analytics/scripts/telemetry | Get telemetry pixel script |
| [**analyticsHeartbeat**](AuthApi.md#analyticsHeartbeat) | **GET** /v1/analytics/heartbeat | Health check |
| [**analyticsLogin**](AuthApi.md#analyticsLogin) | **POST** /v1/analytics/auth/login | Log in with username and password |
| [**analyticsLogout**](AuthApi.md#analyticsLogout) | **POST** /v1/analytics/auth/logout | Log out and invalidate token |
| [**analyticsSsoAuth**](AuthApi.md#analyticsSsoAuth) | **POST** /v1/analytics/auth/sso | Exchange SSO credentials for a session token |
| [**analyticsVerifyAuth**](AuthApi.md#analyticsVerifyAuth) | **POST** /v1/analytics/auth/verify | Verify current auth token |
| [**botAuthCallback**](AuthApi.md#botAuthCallback) | **GET** /v1/bot/auth/callback | OAuth callback - exchange code for session |
| [**botAuthLogin**](AuthApi.md#botAuthLogin) | **GET** /v1/bot/auth/login | Initiate OAuth login via Hanzo IAM |
| [**botAuthLogout**](AuthApi.md#botAuthLogout) | **POST** /v1/bot/auth/logout | Invalidate current session |
| [**botAuthMe**](AuthApi.md#botAuthMe) | **GET** /v1/bot/auth/me | Get current authenticated user |
| [**botWhoami**](AuthApi.md#botWhoami) | **GET** /v1/bot/whoami | CLI alias for /v1/bot/auth/me |
| [**chatGetAuth2faEnable**](AuthApi.md#chatGetAuth2faEnable) | **GET** /v1/chat/auth/2fa/enable | Enable 2FA |
| [**chatGetAuthGraphToken**](AuthApi.md#chatGetAuthGraphToken) | **GET** /v1/chat/auth/graph-token | Get Microsoft Graph token |
| [**chatPostAuth2faBackupRegenerate**](AuthApi.md#chatPostAuth2faBackupRegenerate) | **POST** /v1/chat/auth/2fa/backup/regenerate | Regenerate 2FA backup codes |
| [**chatPostAuth2faConfirm**](AuthApi.md#chatPostAuth2faConfirm) | **POST** /v1/chat/auth/2fa/confirm | Confirm 2FA activation |
| [**chatPostAuth2faDisable**](AuthApi.md#chatPostAuth2faDisable) | **POST** /v1/chat/auth/2fa/disable | Disable 2FA |
| [**chatPostAuth2faVerify**](AuthApi.md#chatPostAuth2faVerify) | **POST** /v1/chat/auth/2fa/verify | Verify 2FA setup |
| [**chatPostAuth2faVerifyTemp**](AuthApi.md#chatPostAuth2faVerifyTemp) | **POST** /v1/chat/auth/2fa/verify-temp | Verify 2FA with temporary token |
| [**chatPostAuthLogin**](AuthApi.md#chatPostAuthLogin) | **POST** /v1/chat/auth/login | Login |
| [**chatPostAuthLogout**](AuthApi.md#chatPostAuthLogout) | **POST** /v1/chat/auth/logout | Logout |
| [**chatPostAuthRefresh**](AuthApi.md#chatPostAuthRefresh) | **POST** /v1/chat/auth/refresh | Refresh token |
| [**chatPostAuthRegister**](AuthApi.md#chatPostAuthRegister) | **POST** /v1/chat/auth/register | Register a new user |
| [**chatPostAuthRequestpasswordreset**](AuthApi.md#chatPostAuthRequestpasswordreset) | **POST** /v1/chat/auth/requestPasswordReset | Request password reset email |
| [**chatPostAuthResetpassword**](AuthApi.md#chatPostAuthResetpassword) | **POST** /v1/chat/auth/resetPassword | Reset password with token |
| [**commerceAuthenticate**](AuthApi.md#commerceAuthenticate) | **POST** /v1/commerce/auth | Authenticate user (OAuth2) |
| [**kmsLogin1**](AuthApi.md#kmsLogin1) | **POST** /v1/kms/auth/login1 | Login step 1 - SRP init |
| [**kmsRenewAccessToken**](AuthApi.md#kmsRenewAccessToken) | **POST** /v1/kms/auth/token/renew | Renew access token |
| [**paasGetCurrentUser**](AuthApi.md#paasGetCurrentUser) | **GET** /v1/paas/auth/me | Get current user |
| [**paasLogin**](AuthApi.md#paasLogin) | **POST** /v1/paas/auth/login | Login via IAM |


<a id="analyticsGetTelemetryScript"></a>
# **analyticsGetTelemetryScript**
> kotlin.String analyticsGetTelemetryScript()

Get telemetry pixel script

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
try {
    val result : kotlin.String = apiInstance.analyticsGetTelemetryScript()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#analyticsGetTelemetryScript")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#analyticsGetTelemetryScript")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

**kotlin.String**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="analyticsHeartbeat"></a>
# **analyticsHeartbeat**
> AnalyticsHeartbeat200Response analyticsHeartbeat()

Health check

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
try {
    val result : AnalyticsHeartbeat200Response = apiInstance.analyticsHeartbeat()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#analyticsHeartbeat")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#analyticsHeartbeat")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AnalyticsHeartbeat200Response**](AnalyticsHeartbeat200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="analyticsLogin"></a>
# **analyticsLogin**
> AnalyticsLogin200Response analyticsLogin(analyticsLoginRequest)

Log in with username and password

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
val analyticsLoginRequest : AnalyticsLoginRequest =  // AnalyticsLoginRequest | 
try {
    val result : AnalyticsLogin200Response = apiInstance.analyticsLogin(analyticsLoginRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#analyticsLogin")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#analyticsLogin")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **analyticsLoginRequest** | [**AnalyticsLoginRequest**](AnalyticsLoginRequest.md)|  | |

### Return type

[**AnalyticsLogin200Response**](AnalyticsLogin200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="analyticsLogout"></a>
# **analyticsLogout**
> kotlin.Any analyticsLogout()

Log out and invalidate token

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
try {
    val result : kotlin.Any = apiInstance.analyticsLogout()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#analyticsLogout")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#analyticsLogout")
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

<a id="analyticsSsoAuth"></a>
# **analyticsSsoAuth**
> AnalyticsSsoAuth200Response analyticsSsoAuth()

Exchange SSO credentials for a session token

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
try {
    val result : AnalyticsSsoAuth200Response = apiInstance.analyticsSsoAuth()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#analyticsSsoAuth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#analyticsSsoAuth")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AnalyticsSsoAuth200Response**](AnalyticsSsoAuth200Response.md)

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

<a id="analyticsVerifyAuth"></a>
# **analyticsVerifyAuth**
> AnalyticsUser analyticsVerifyAuth()

Verify current auth token

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
try {
    val result : AnalyticsUser = apiInstance.analyticsVerifyAuth()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#analyticsVerifyAuth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#analyticsVerifyAuth")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AnalyticsUser**](AnalyticsUser.md)

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

<a id="botAuthCallback"></a>
# **botAuthCallback**
> botAuthCallback(code, state, error)

OAuth callback - exchange code for session

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
val code : kotlin.String = code_example // kotlin.String | Authorization code from IAM
val state : kotlin.String = state_example // kotlin.String | 
val error : kotlin.String = error_example // kotlin.String | 
try {
    apiInstance.botAuthCallback(code, state, error)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#botAuthCallback")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#botAuthCallback")
    e.printStackTrace()
}
```

### Parameters
| **code** | **kotlin.String**| Authorization code from IAM | |
| **state** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **error** | **kotlin.String**|  | [optional] |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="botAuthLogin"></a>
# **botAuthLogin**
> botAuthLogin(redirectUri, state)

Initiate OAuth login via Hanzo IAM

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
val redirectUri : java.net.URI = redirectUri_example // java.net.URI | Override callback URL
val state : kotlin.String = state_example // kotlin.String | Opaque state for CSRF protection
try {
    apiInstance.botAuthLogin(redirectUri, state)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#botAuthLogin")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#botAuthLogin")
    e.printStackTrace()
}
```

### Parameters
| **redirectUri** | **java.net.URI**| Override callback URL | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **state** | **kotlin.String**| Opaque state for CSRF protection | [optional] |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="botAuthLogout"></a>
# **botAuthLogout**
> AnalyticsHeartbeat200Response botAuthLogout()

Invalidate current session

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
try {
    val result : AnalyticsHeartbeat200Response = apiInstance.botAuthLogout()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#botAuthLogout")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#botAuthLogout")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AnalyticsHeartbeat200Response**](AnalyticsHeartbeat200Response.md)

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

<a id="botAuthMe"></a>
# **botAuthMe**
> BotUser botAuthMe()

Get current authenticated user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
try {
    val result : BotUser = apiInstance.botAuthMe()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#botAuthMe")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#botAuthMe")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**BotUser**](BotUser.md)

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

<a id="botWhoami"></a>
# **botWhoami**
> BotUser botWhoami()

CLI alias for /v1/bot/auth/me

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
try {
    val result : BotUser = apiInstance.botWhoami()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#botWhoami")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#botWhoami")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**BotUser**](BotUser.md)

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

<a id="chatGetAuth2faEnable"></a>
# **chatGetAuth2faEnable**
> ChatGetAuth2faEnable200Response chatGetAuth2faEnable()

Enable 2FA

Generate a TOTP secret and QR code for 2FA setup.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
try {
    val result : ChatGetAuth2faEnable200Response = apiInstance.chatGetAuth2faEnable()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#chatGetAuth2faEnable")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#chatGetAuth2faEnable")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ChatGetAuth2faEnable200Response**](ChatGetAuth2faEnable200Response.md)

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

<a id="chatGetAuthGraphToken"></a>
# **chatGetAuthGraphToken**
> kotlin.Any chatGetAuthGraphToken()

Get Microsoft Graph token

Returns a Microsoft Graph API token for SharePoint integration.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
try {
    val result : kotlin.Any = apiInstance.chatGetAuthGraphToken()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#chatGetAuthGraphToken")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#chatGetAuthGraphToken")
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

<a id="chatPostAuth2faBackupRegenerate"></a>
# **chatPostAuth2faBackupRegenerate**
> ChatPostAuth2faBackupRegenerate200Response chatPostAuth2faBackupRegenerate(chatPostAuth2faBackupRegenerateRequest)

Regenerate 2FA backup codes

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
val chatPostAuth2faBackupRegenerateRequest : ChatPostAuth2faBackupRegenerateRequest =  // ChatPostAuth2faBackupRegenerateRequest | 
try {
    val result : ChatPostAuth2faBackupRegenerate200Response = apiInstance.chatPostAuth2faBackupRegenerate(chatPostAuth2faBackupRegenerateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#chatPostAuth2faBackupRegenerate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#chatPostAuth2faBackupRegenerate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostAuth2faBackupRegenerateRequest** | [**ChatPostAuth2faBackupRegenerateRequest**](ChatPostAuth2faBackupRegenerateRequest.md)|  | |

### Return type

[**ChatPostAuth2faBackupRegenerate200Response**](ChatPostAuth2faBackupRegenerate200Response.md)

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

<a id="chatPostAuth2faConfirm"></a>
# **chatPostAuth2faConfirm**
> ChatPostAuth2faBackupRegenerate200Response chatPostAuth2faConfirm(chatPostAuth2faBackupRegenerateRequest)

Confirm 2FA activation

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
val chatPostAuth2faBackupRegenerateRequest : ChatPostAuth2faBackupRegenerateRequest =  // ChatPostAuth2faBackupRegenerateRequest | 
try {
    val result : ChatPostAuth2faBackupRegenerate200Response = apiInstance.chatPostAuth2faConfirm(chatPostAuth2faBackupRegenerateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#chatPostAuth2faConfirm")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#chatPostAuth2faConfirm")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostAuth2faBackupRegenerateRequest** | [**ChatPostAuth2faBackupRegenerateRequest**](ChatPostAuth2faBackupRegenerateRequest.md)|  | |

### Return type

[**ChatPostAuth2faBackupRegenerate200Response**](ChatPostAuth2faBackupRegenerate200Response.md)

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

<a id="chatPostAuth2faDisable"></a>
# **chatPostAuth2faDisable**
> kotlin.Any chatPostAuth2faDisable(chatPostAuth2faBackupRegenerateRequest)

Disable 2FA

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
val chatPostAuth2faBackupRegenerateRequest : ChatPostAuth2faBackupRegenerateRequest =  // ChatPostAuth2faBackupRegenerateRequest | 
try {
    val result : kotlin.Any = apiInstance.chatPostAuth2faDisable(chatPostAuth2faBackupRegenerateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#chatPostAuth2faDisable")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#chatPostAuth2faDisable")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostAuth2faBackupRegenerateRequest** | [**ChatPostAuth2faBackupRegenerateRequest**](ChatPostAuth2faBackupRegenerateRequest.md)|  | |

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

<a id="chatPostAuth2faVerify"></a>
# **chatPostAuth2faVerify**
> kotlin.Any chatPostAuth2faVerify(chatPostAuth2faBackupRegenerateRequest)

Verify 2FA setup

Verify TOTP code during 2FA setup.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
val chatPostAuth2faBackupRegenerateRequest : ChatPostAuth2faBackupRegenerateRequest =  // ChatPostAuth2faBackupRegenerateRequest | 
try {
    val result : kotlin.Any = apiInstance.chatPostAuth2faVerify(chatPostAuth2faBackupRegenerateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#chatPostAuth2faVerify")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#chatPostAuth2faVerify")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostAuth2faBackupRegenerateRequest** | [**ChatPostAuth2faBackupRegenerateRequest**](ChatPostAuth2faBackupRegenerateRequest.md)|  | |

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

<a id="chatPostAuth2faVerifyTemp"></a>
# **chatPostAuth2faVerifyTemp**
> ChatAuthResponse chatPostAuth2faVerifyTemp(chatPostAuth2faVerifyTempRequest)

Verify 2FA with temporary token

Verify 2FA code during login using a temporary token.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
val chatPostAuth2faVerifyTempRequest : ChatPostAuth2faVerifyTempRequest =  // ChatPostAuth2faVerifyTempRequest | 
try {
    val result : ChatAuthResponse = apiInstance.chatPostAuth2faVerifyTemp(chatPostAuth2faVerifyTempRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#chatPostAuth2faVerifyTemp")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#chatPostAuth2faVerifyTemp")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostAuth2faVerifyTempRequest** | [**ChatPostAuth2faVerifyTempRequest**](ChatPostAuth2faVerifyTempRequest.md)|  | |

### Return type

[**ChatAuthResponse**](ChatAuthResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="chatPostAuthLogin"></a>
# **chatPostAuthLogin**
> ChatAuthResponse chatPostAuthLogin(chatPostAuthLoginRequest)

Login

Authenticate with email and password (or LDAP).

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
val chatPostAuthLoginRequest : ChatPostAuthLoginRequest =  // ChatPostAuthLoginRequest | 
try {
    val result : ChatAuthResponse = apiInstance.chatPostAuthLogin(chatPostAuthLoginRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#chatPostAuthLogin")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#chatPostAuthLogin")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostAuthLoginRequest** | [**ChatPostAuthLoginRequest**](ChatPostAuthLoginRequest.md)|  | |

### Return type

[**ChatAuthResponse**](ChatAuthResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="chatPostAuthLogout"></a>
# **chatPostAuthLogout**
> kotlin.Any chatPostAuthLogout()

Logout

Invalidate the current session.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
try {
    val result : kotlin.Any = apiInstance.chatPostAuthLogout()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#chatPostAuthLogout")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#chatPostAuthLogout")
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

<a id="chatPostAuthRefresh"></a>
# **chatPostAuthRefresh**
> ChatAuthResponse chatPostAuthRefresh(chatPostAuthRefreshRequest)

Refresh token

Exchange a refresh token for a new access token.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
val chatPostAuthRefreshRequest : ChatPostAuthRefreshRequest =  // ChatPostAuthRefreshRequest | 
try {
    val result : ChatAuthResponse = apiInstance.chatPostAuthRefresh(chatPostAuthRefreshRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#chatPostAuthRefresh")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#chatPostAuthRefresh")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostAuthRefreshRequest** | [**ChatPostAuthRefreshRequest**](ChatPostAuthRefreshRequest.md)|  | [optional] |

### Return type

[**ChatAuthResponse**](ChatAuthResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="chatPostAuthRegister"></a>
# **chatPostAuthRegister**
> kotlin.Any chatPostAuthRegister(chatPostAuthRegisterRequest)

Register a new user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
val chatPostAuthRegisterRequest : ChatPostAuthRegisterRequest =  // ChatPostAuthRegisterRequest | 
try {
    val result : kotlin.Any = apiInstance.chatPostAuthRegister(chatPostAuthRegisterRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#chatPostAuthRegister")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#chatPostAuthRegister")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostAuthRegisterRequest** | [**ChatPostAuthRegisterRequest**](ChatPostAuthRegisterRequest.md)|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="chatPostAuthRequestpasswordreset"></a>
# **chatPostAuthRequestpasswordreset**
> kotlin.Any chatPostAuthRequestpasswordreset(chatPostAuthRequestpasswordresetRequest)

Request password reset email

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
val chatPostAuthRequestpasswordresetRequest : ChatPostAuthRequestpasswordresetRequest =  // ChatPostAuthRequestpasswordresetRequest | 
try {
    val result : kotlin.Any = apiInstance.chatPostAuthRequestpasswordreset(chatPostAuthRequestpasswordresetRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#chatPostAuthRequestpasswordreset")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#chatPostAuthRequestpasswordreset")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostAuthRequestpasswordresetRequest** | [**ChatPostAuthRequestpasswordresetRequest**](ChatPostAuthRequestpasswordresetRequest.md)|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="chatPostAuthResetpassword"></a>
# **chatPostAuthResetpassword**
> kotlin.Any chatPostAuthResetpassword(chatPostAuthResetpasswordRequest)

Reset password with token

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
val chatPostAuthResetpasswordRequest : ChatPostAuthResetpasswordRequest =  // ChatPostAuthResetpasswordRequest | 
try {
    val result : kotlin.Any = apiInstance.chatPostAuthResetpassword(chatPostAuthResetpasswordRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#chatPostAuthResetpassword")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#chatPostAuthResetpassword")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostAuthResetpasswordRequest** | [**ChatPostAuthResetpasswordRequest**](ChatPostAuthResetpasswordRequest.md)|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="commerceAuthenticate"></a>
# **commerceAuthenticate**
> CommerceOAuthResponse commerceAuthenticate(commerceOAuthRequest)

Authenticate user (OAuth2)

OAuth2 token endpoint supporting password and refresh_token grant types. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
val commerceOAuthRequest : CommerceOAuthRequest =  // CommerceOAuthRequest | 
try {
    val result : CommerceOAuthResponse = apiInstance.commerceAuthenticate(commerceOAuthRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#commerceAuthenticate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#commerceAuthenticate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceOAuthRequest** | [**CommerceOAuthRequest**](CommerceOAuthRequest.md)|  | |

### Return type

[**CommerceOAuthResponse**](CommerceOAuthResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="kmsLogin1"></a>
# **kmsLogin1**
> KmsLoginResponse kmsLogin1(kmsLoginRequest)

Login step 1 - SRP init

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
val kmsLoginRequest : KmsLoginRequest =  // KmsLoginRequest | 
try {
    val result : KmsLoginResponse = apiInstance.kmsLogin1(kmsLoginRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#kmsLogin1")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#kmsLogin1")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsLoginRequest** | [**KmsLoginRequest**](KmsLoginRequest.md)|  | |

### Return type

[**KmsLoginResponse**](KmsLoginResponse.md)

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

<a id="kmsRenewAccessToken"></a>
# **kmsRenewAccessToken**
> KmsTokenResponse kmsRenewAccessToken()

Renew access token

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
try {
    val result : KmsTokenResponse = apiInstance.kmsRenewAccessToken()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#kmsRenewAccessToken")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#kmsRenewAccessToken")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**KmsTokenResponse**](KmsTokenResponse.md)

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

<a id="paasGetCurrentUser"></a>
# **paasGetCurrentUser**
> kotlin.Any paasGetCurrentUser()

Get current user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
try {
    val result : kotlin.Any = apiInstance.paasGetCurrentUser()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#paasGetCurrentUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#paasGetCurrentUser")
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

<a id="paasLogin"></a>
# **paasLogin**
> PaasLogin200Response paasLogin(paasLoginRequest)

Login via IAM

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthApi()
val paasLoginRequest : PaasLoginRequest =  // PaasLoginRequest | 
try {
    val result : PaasLogin200Response = apiInstance.paasLogin(paasLoginRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#paasLogin")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#paasLogin")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **paasLoginRequest** | [**PaasLoginRequest**](PaasLoginRequest.md)|  | [optional] |

### Return type

[**PaasLogin200Response**](PaasLogin200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

