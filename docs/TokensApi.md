# TokensApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**botCreateToken**](TokensApi.md#botCreateToken) | **POST** /v1/bot/tokens | Create a new API token |
| [**botListTokens**](TokensApi.md#botListTokens) | **GET** /v1/bot/tokens | List current user&#39;s API tokens |
| [**botRevokeToken**](TokensApi.md#botRevokeToken) | **DELETE** /v1/bot/tokens/{id} | Revoke an API token |
| [**iamApiControllerAddToken**](TokensApi.md#iamApiControllerAddToken) | **POST** /v1/iam/tokens | Api Controller Add Token |
| [**iamApiControllerDeleteToken**](TokensApi.md#iamApiControllerDeleteToken) | **DELETE** /v1/iam/tokens/{id} | Api Controller Delete Token |
| [**iamApiControllerGetCaptchaStatus**](TokensApi.md#iamApiControllerGetCaptchaStatus) | **GET** /v1/iam/captcha/status | Api Controller Get Captcha Status |
| [**iamApiControllerGetOAuthToken**](TokensApi.md#iamApiControllerGetOAuthToken) | **POST** /oauth/token | Api Controller Get O Auth Token |
| [**iamApiControllerGetToken**](TokensApi.md#iamApiControllerGetToken) | **GET** /v1/iam/tokens/{id} | Api Controller Get Token |
| [**iamApiControllerGetTokens**](TokensApi.md#iamApiControllerGetTokens) | **GET** /v1/iam/tokens | Api Controller Get Tokens |
| [**iamApiControllerRefreshToken**](TokensApi.md#iamApiControllerRefreshToken) | **POST** /oauth/token/refresh | Api Controller Refresh Token |
| [**iamApiControllerUpdateToken**](TokensApi.md#iamApiControllerUpdateToken) | **PUT** /v1/iam/tokens/{id} | Api Controller Update Token |


<a id="botCreateToken"></a>
# **botCreateToken**
> BotCreateToken200Response botCreateToken(botCreateTokenRequest)

Create a new API token

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TokensApi()
val botCreateTokenRequest : BotCreateTokenRequest =  // BotCreateTokenRequest | 
try {
    val result : BotCreateToken200Response = apiInstance.botCreateToken(botCreateTokenRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TokensApi#botCreateToken")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TokensApi#botCreateToken")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **botCreateTokenRequest** | [**BotCreateTokenRequest**](BotCreateTokenRequest.md)|  | |

### Return type

[**BotCreateToken200Response**](BotCreateToken200Response.md)

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

<a id="botListTokens"></a>
# **botListTokens**
> BotListTokens200Response botListTokens()

List current user&#39;s API tokens

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TokensApi()
try {
    val result : BotListTokens200Response = apiInstance.botListTokens()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TokensApi#botListTokens")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TokensApi#botListTokens")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**BotListTokens200Response**](BotListTokens200Response.md)

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

<a id="botRevokeToken"></a>
# **botRevokeToken**
> AnalyticsHeartbeat200Response botRevokeToken(id)

Revoke an API token

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TokensApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : AnalyticsHeartbeat200Response = apiInstance.botRevokeToken(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TokensApi#botRevokeToken")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TokensApi#botRevokeToken")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

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

<a id="iamApiControllerAddToken"></a>
# **iamApiControllerAddToken**
> IamControllersResponse iamApiControllerAddToken(iamObjectToken)

Api Controller Add Token

add token

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TokensApi()
val iamObjectToken : IamObjectToken =  // IamObjectToken | Details of the token
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddToken(iamObjectToken)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TokensApi#iamApiControllerAddToken")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TokensApi#iamApiControllerAddToken")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectToken** | [**IamObjectToken**](IamObjectToken.md)| Details of the token | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerDeleteToken"></a>
# **iamApiControllerDeleteToken**
> IamControllersResponse iamApiControllerDeleteToken(id, iamObjectToken)

Api Controller Delete Token

delete token

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TokensApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectToken : IamObjectToken =  // IamObjectToken | Details of the token
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeleteToken(id, iamObjectToken)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TokensApi#iamApiControllerDeleteToken")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TokensApi#iamApiControllerDeleteToken")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectToken** | [**IamObjectToken**](IamObjectToken.md)| Details of the token | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerGetCaptchaStatus"></a>
# **iamApiControllerGetCaptchaStatus**
> IamControllersResponse iamApiControllerGetCaptchaStatus(id)

Api Controller Get Captcha Status

Get Login Error Counts

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TokensApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of user
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerGetCaptchaStatus(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TokensApi#iamApiControllerGetCaptchaStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TokensApi#iamApiControllerGetCaptchaStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of user | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerGetOAuthToken"></a>
# **iamApiControllerGetOAuthToken**
> IamObjectTokenWrapper iamApiControllerGetOAuthToken(grantType, clientId, clientSecret, code)

Api Controller Get O Auth Token

get OAuth access token

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TokensApi()
val grantType : kotlin.String = grantType_example // kotlin.String | OAuth grant type
val clientId : kotlin.String = clientId_example // kotlin.String | OAuth client id
val clientSecret : kotlin.String = clientSecret_example // kotlin.String | OAuth client secret
val code : kotlin.String = code_example // kotlin.String | OAuth code
try {
    val result : IamObjectTokenWrapper = apiInstance.iamApiControllerGetOAuthToken(grantType, clientId, clientSecret, code)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TokensApi#iamApiControllerGetOAuthToken")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TokensApi#iamApiControllerGetOAuthToken")
    e.printStackTrace()
}
```

### Parameters
| **grantType** | **kotlin.String**| OAuth grant type | |
| **clientId** | **kotlin.String**| OAuth client id | |
| **clientSecret** | **kotlin.String**| OAuth client secret | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **code** | **kotlin.String**| OAuth code | |

### Return type

[**IamObjectTokenWrapper**](IamObjectTokenWrapper.md)

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

<a id="iamApiControllerGetToken"></a>
# **iamApiControllerGetToken**
> IamObjectToken iamApiControllerGetToken(id)

Api Controller Get Token

get token

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TokensApi()
val id : kotlin.String = id_example // kotlin.String | The token ID in format: organization/token-name (e.g., built-in/token-123456)
try {
    val result : IamObjectToken = apiInstance.iamApiControllerGetToken(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TokensApi#iamApiControllerGetToken")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TokensApi#iamApiControllerGetToken")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The token ID in format: organization/token-name (e.g., built-in/token-123456) | |

### Return type

[**IamObjectToken**](IamObjectToken.md)

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

<a id="iamApiControllerGetTokens"></a>
# **iamApiControllerGetTokens**
> kotlin.collections.List&lt;IamObjectToken&gt; iamApiControllerGetTokens(owner, pageSize, p)

Api Controller Get Tokens

get tokens

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TokensApi()
val owner : kotlin.String = owner_example // kotlin.String | The organization name (e.g., built-in)
val pageSize : kotlin.String = pageSize_example // kotlin.String | The size of each page
val p : kotlin.String = p_example // kotlin.String | The number of the page
try {
    val result : kotlin.collections.List<IamObjectToken> = apiInstance.iamApiControllerGetTokens(owner, pageSize, p)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TokensApi#iamApiControllerGetTokens")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TokensApi#iamApiControllerGetTokens")
    e.printStackTrace()
}
```

### Parameters
| **owner** | **kotlin.String**| The organization name (e.g., built-in) | |
| **pageSize** | **kotlin.String**| The size of each page | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **p** | **kotlin.String**| The number of the page | |

### Return type

[**kotlin.collections.List&lt;IamObjectToken&gt;**](IamObjectToken.md)

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

<a id="iamApiControllerRefreshToken"></a>
# **iamApiControllerRefreshToken**
> IamObjectTokenWrapper iamApiControllerRefreshToken(grantType, refreshToken, scope, clientId, clientSecret)

Api Controller Refresh Token

refresh OAuth access token

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TokensApi()
val grantType : kotlin.String = grantType_example // kotlin.String | OAuth grant type
val refreshToken : kotlin.String = refreshToken_example // kotlin.String | OAuth refresh token
val scope : kotlin.String = scope_example // kotlin.String | OAuth scope
val clientId : kotlin.String = clientId_example // kotlin.String | OAuth client id
val clientSecret : kotlin.String = clientSecret_example // kotlin.String | OAuth client secret
try {
    val result : IamObjectTokenWrapper = apiInstance.iamApiControllerRefreshToken(grantType, refreshToken, scope, clientId, clientSecret)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TokensApi#iamApiControllerRefreshToken")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TokensApi#iamApiControllerRefreshToken")
    e.printStackTrace()
}
```

### Parameters
| **grantType** | **kotlin.String**| OAuth grant type | |
| **refreshToken** | **kotlin.String**| OAuth refresh token | |
| **scope** | **kotlin.String**| OAuth scope | |
| **clientId** | **kotlin.String**| OAuth client id | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **clientSecret** | **kotlin.String**| OAuth client secret | [optional] |

### Return type

[**IamObjectTokenWrapper**](IamObjectTokenWrapper.md)

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

<a id="iamApiControllerUpdateToken"></a>
# **iamApiControllerUpdateToken**
> IamControllersResponse iamApiControllerUpdateToken(id, iamObjectToken)

Api Controller Update Token

update token

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TokensApi()
val id : kotlin.String = id_example // kotlin.String | The token ID in format: organization/token-name (e.g., built-in/token-123456)
val iamObjectToken : IamObjectToken =  // IamObjectToken | Details of the token
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdateToken(id, iamObjectToken)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TokensApi#iamApiControllerUpdateToken")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TokensApi#iamApiControllerUpdateToken")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The token ID in format: organization/token-name (e.g., built-in/token-123456) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectToken** | [**IamObjectToken**](IamObjectToken.md)| Details of the token | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

