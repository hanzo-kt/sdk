# AuthenticationApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoSignIn**](AuthenticationApi.md#autoSignIn) | **POST** /v1/auto/authentication/sign-in | Sign in with credentials |
| [**autoSignUp**](AuthenticationApi.md#autoSignUp) | **POST** /v1/auto/authentication/sign-up | Sign up a new user |
| [**flowFederatedClaim**](AuthenticationApi.md#flowFederatedClaim) | **POST** /v1/flow/authn/federated/claim | Complete federated authentication (EE) |
| [**flowFederatedLogin**](AuthenticationApi.md#flowFederatedLogin) | **GET** /v1/flow/authn/federated/login | Initiate federated authentication (EE) |
| [**flowSignIn**](AuthenticationApi.md#flowSignIn) | **POST** /v1/flow/authentication/sign-in | Sign in with credentials |
| [**flowSignUp**](AuthenticationApi.md#flowSignUp) | **POST** /v1/flow/authentication/sign-up | Sign up a new user |
| [**iamApiControllerCallback**](AuthenticationApi.md#iamApiControllerCallback) | **POST** /oauth/callback | Api Controller Callback |
| [**iamApiControllerDeviceAuth**](AuthenticationApi.md#iamApiControllerDeviceAuth) | **POST** /v1/iam/auth/device | Api Controller Device Auth |
| [**iamApiControllerFaceIDSigninBegin**](AuthenticationApi.md#iamApiControllerFaceIDSigninBegin) | **GET** /v1/iam/auth/faceid/begin | Api Controller Face ID Signin Begin |
| [**iamApiControllerGetApplicationLogin**](AuthenticationApi.md#iamApiControllerGetApplicationLogin) | **GET** /v1/iam/auth/app-login | Api Controller Get Application Login |
| [**iamApiControllerGetCaptcha**](AuthenticationApi.md#iamApiControllerGetCaptcha) | **GET** /v1/iam/captcha | Api Controller Get Captcha |
| [**iamApiControllerIntrospectToken**](AuthenticationApi.md#iamApiControllerIntrospectToken) | **POST** /oauth/introspect | Api Controller Introspect Token |
| [**iamApiControllerLogin**](AuthenticationApi.md#iamApiControllerLogin) | **POST** /v1/iam/auth/login | Api Controller Login |
| [**iamApiControllerLogout**](AuthenticationApi.md#iamApiControllerLogout) | **POST** /v1/iam/auth/logout | Api Controller Logout |
| [**iamApiControllerSignup**](AuthenticationApi.md#iamApiControllerSignup) | **POST** /v1/iam/auth/signup | Api Controller Signup |
| [**iamApiControllerSsoLogoutGet**](AuthenticationApi.md#iamApiControllerSsoLogoutGet) | **GET** /v1/iam/sso-logout | Api Controller Sso Logout |
| [**iamApiControllerSsoLogoutPost**](AuthenticationApi.md#iamApiControllerSsoLogoutPost) | **POST** /v1/iam/sso-logout | Api Controller Sso Logout |
| [**iamApiControllerUnlink**](AuthenticationApi.md#iamApiControllerUnlink) | **POST** /v1/iam/unlink | Api Controller Unlink |
| [**iamApiControllerWebAuthnSigninBegin**](AuthenticationApi.md#iamApiControllerWebAuthnSigninBegin) | **GET** /v1/iam/auth/webauthn/signin/begin | Api Controller Web Authn Signin Begin |
| [**iamApiControllerWebAuthnSigninFinish**](AuthenticationApi.md#iamApiControllerWebAuthnSigninFinish) | **POST** /v1/iam/auth/webauthn/signin/finish | Api Controller Web Authn Signin Finish |
| [**iamRootControllerGetJwks**](AuthenticationApi.md#iamRootControllerGetJwks) | **GET** /.well-known/jwks | Root Controller Get Jwks |
| [**iamRootControllerGetJwksByApplication**](AuthenticationApi.md#iamRootControllerGetJwksByApplication) | **GET** /.well-known/{application}/jwks | Root Controller Get Jwks By Application |
| [**iamRootControllerGetOidcDiscovery**](AuthenticationApi.md#iamRootControllerGetOidcDiscovery) | **GET** /.well-known/openid-configuration | Root Controller Get Oidc Discovery |
| [**iamRootControllerGetOidcDiscoveryByApplication**](AuthenticationApi.md#iamRootControllerGetOidcDiscoveryByApplication) | **GET** /.well-known/{application}/openid-configuration | Root Controller Get Oidc Discovery By Application |
| [**iamRootControllerGetWebFinger**](AuthenticationApi.md#iamRootControllerGetWebFinger) | **GET** /.well-known/webfinger | Root Controller Get Web Finger |
| [**iamRootControllerGetWebFingerByApplication**](AuthenticationApi.md#iamRootControllerGetWebFingerByApplication) | **GET** /.well-known/{application}/webfinger | Root Controller Get Web Finger By Application |


<a id="autoSignIn"></a>
# **autoSignIn**
> kotlin.Any autoSignIn(autoSignInRequest)

Sign in with credentials

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
val autoSignInRequest : AutoSignInRequest =  // AutoSignInRequest | 
try {
    val result : kotlin.Any = apiInstance.autoSignIn(autoSignInRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#autoSignIn")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#autoSignIn")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoSignInRequest** | [**AutoSignInRequest**](AutoSignInRequest.md)|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="autoSignUp"></a>
# **autoSignUp**
> kotlin.Any autoSignUp(autoSignUpRequest)

Sign up a new user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
val autoSignUpRequest : AutoSignUpRequest =  // AutoSignUpRequest | 
try {
    val result : kotlin.Any = apiInstance.autoSignUp(autoSignUpRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#autoSignUp")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#autoSignUp")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoSignUpRequest** | [**AutoSignUpRequest**](AutoSignUpRequest.md)|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="flowFederatedClaim"></a>
# **flowFederatedClaim**
> kotlin.Any flowFederatedClaim(body)

Complete federated authentication (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.flowFederatedClaim(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#flowFederatedClaim")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#flowFederatedClaim")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="flowFederatedLogin"></a>
# **flowFederatedLogin**
> flowFederatedLogin()

Initiate federated authentication (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
try {
    apiInstance.flowFederatedLogin()
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#flowFederatedLogin")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#flowFederatedLogin")
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

<a id="flowSignIn"></a>
# **flowSignIn**
> kotlin.Any flowSignIn(autoSignInRequest)

Sign in with credentials

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
val autoSignInRequest : AutoSignInRequest =  // AutoSignInRequest | 
try {
    val result : kotlin.Any = apiInstance.flowSignIn(autoSignInRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#flowSignIn")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#flowSignIn")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoSignInRequest** | [**AutoSignInRequest**](AutoSignInRequest.md)|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="flowSignUp"></a>
# **flowSignUp**
> kotlin.Any flowSignUp(autoSignUpRequest)

Sign up a new user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
val autoSignUpRequest : AutoSignUpRequest =  // AutoSignUpRequest | 
try {
    val result : kotlin.Any = apiInstance.flowSignUp(autoSignUpRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#flowSignUp")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#flowSignUp")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoSignUpRequest** | [**AutoSignUpRequest**](AutoSignUpRequest.md)|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="iamApiControllerCallback"></a>
# **iamApiControllerCallback**
> IamObjectUserinfo iamApiControllerCallback()

Api Controller Callback

Get Login Error Counts

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
try {
    val result : IamObjectUserinfo = apiInstance.iamApiControllerCallback()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#iamApiControllerCallback")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#iamApiControllerCallback")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**IamObjectUserinfo**](IamObjectUserinfo.md)

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

<a id="iamApiControllerDeviceAuth"></a>
# **iamApiControllerDeviceAuth**
> IamObjectDeviceAuthResponse iamApiControllerDeviceAuth()

Api Controller Device Auth

Endpoint for the device authorization flow

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
try {
    val result : IamObjectDeviceAuthResponse = apiInstance.iamApiControllerDeviceAuth()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#iamApiControllerDeviceAuth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#iamApiControllerDeviceAuth")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**IamObjectDeviceAuthResponse**](IamObjectDeviceAuthResponse.md)

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

<a id="iamApiControllerFaceIDSigninBegin"></a>
# **iamApiControllerFaceIDSigninBegin**
> IamControllersResponse iamApiControllerFaceIDSigninBegin(owner, name)

Api Controller Face ID Signin Begin

FaceId Login Flow 1st stage

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
val owner : kotlin.String = owner_example // kotlin.String | owner
val name : kotlin.String = name_example // kotlin.String | name
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerFaceIDSigninBegin(owner, name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#iamApiControllerFaceIDSigninBegin")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#iamApiControllerFaceIDSigninBegin")
    e.printStackTrace()
}
```

### Parameters
| **owner** | **kotlin.String**| owner | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**| name | |

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

<a id="iamApiControllerGetApplicationLogin"></a>
# **iamApiControllerGetApplicationLogin**
> IamControllersResponse iamApiControllerGetApplicationLogin(clientId, responseType, redirectUri, scope, state)

Api Controller Get Application Login

get application login

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
val clientId : kotlin.String = clientId_example // kotlin.String | client id
val responseType : kotlin.String = responseType_example // kotlin.String | response type
val redirectUri : kotlin.String = redirectUri_example // kotlin.String | redirect uri
val scope : kotlin.String = scope_example // kotlin.String | scope
val state : kotlin.String = state_example // kotlin.String | state
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerGetApplicationLogin(clientId, responseType, redirectUri, scope, state)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#iamApiControllerGetApplicationLogin")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#iamApiControllerGetApplicationLogin")
    e.printStackTrace()
}
```

### Parameters
| **clientId** | **kotlin.String**| client id | |
| **responseType** | **kotlin.String**| response type | |
| **redirectUri** | **kotlin.String**| redirect uri | |
| **scope** | **kotlin.String**| scope | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **state** | **kotlin.String**| state | |

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

<a id="iamApiControllerGetCaptcha"></a>
# **iamApiControllerGetCaptcha**
> IamObjectUserinfo iamApiControllerGetCaptcha()

Api Controller Get Captcha

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
try {
    val result : IamObjectUserinfo = apiInstance.iamApiControllerGetCaptcha()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#iamApiControllerGetCaptcha")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#iamApiControllerGetCaptcha")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**IamObjectUserinfo**](IamObjectUserinfo.md)

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

<a id="iamApiControllerIntrospectToken"></a>
# **iamApiControllerIntrospectToken**
> IamObjectIntrospectionResponse iamApiControllerIntrospectToken(token, tokenTypeHint)

Api Controller Introspect Token

The introspection endpoint is an OAuth 2.0 endpoint that takes a

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
val token : kotlin.String = token_example // kotlin.String | access_token's value or refresh_token's value
val tokenTypeHint : kotlin.String = tokenTypeHint_example // kotlin.String | the token type access_token or refresh_token
try {
    val result : IamObjectIntrospectionResponse = apiInstance.iamApiControllerIntrospectToken(token, tokenTypeHint)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#iamApiControllerIntrospectToken")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#iamApiControllerIntrospectToken")
    e.printStackTrace()
}
```

### Parameters
| **token** | **kotlin.String**| access_token&#39;s value or refresh_token&#39;s value | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **tokenTypeHint** | **kotlin.String**| the token type access_token or refresh_token | |

### Return type

[**IamObjectIntrospectionResponse**](IamObjectIntrospectionResponse.md)

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

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json

<a id="iamApiControllerLogin"></a>
# **iamApiControllerLogin**
> IamControllersResponse iamApiControllerLogin(clientId, responseType, redirectUri, body, scope, state, nonce, codeChallengeMethod, codeChallenge)

Api Controller Login

login

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
val clientId : kotlin.String = clientId_example // kotlin.String | clientId
val responseType : kotlin.String = responseType_example // kotlin.String | responseType
val redirectUri : kotlin.String = redirectUri_example // kotlin.String | redirectUri
val body : kotlin.Any = Object // kotlin.Any | Login information
val scope : kotlin.String = scope_example // kotlin.String | scope
val state : kotlin.String = state_example // kotlin.String | state
val nonce : kotlin.String = nonce_example // kotlin.String | nonce
val codeChallengeMethod : kotlin.String = codeChallengeMethod_example // kotlin.String | code_challenge_method
val codeChallenge : kotlin.String = codeChallenge_example // kotlin.String | code_challenge
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerLogin(clientId, responseType, redirectUri, body, scope, state, nonce, codeChallengeMethod, codeChallenge)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#iamApiControllerLogin")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#iamApiControllerLogin")
    e.printStackTrace()
}
```

### Parameters
| **clientId** | **kotlin.String**| clientId | |
| **responseType** | **kotlin.String**| responseType | |
| **redirectUri** | **kotlin.String**| redirectUri | |
| **body** | **kotlin.Any**| Login information | |
| **scope** | **kotlin.String**| scope | [optional] |
| **state** | **kotlin.String**| state | [optional] |
| **nonce** | **kotlin.String**| nonce | [optional] |
| **codeChallengeMethod** | **kotlin.String**| code_challenge_method | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **codeChallenge** | **kotlin.String**| code_challenge | [optional] |

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

<a id="iamApiControllerLogout"></a>
# **iamApiControllerLogout**
> IamControllersResponse iamApiControllerLogout(idTokenHint, postLogoutRedirectUri, state)

Api Controller Logout

logout the current user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
val idTokenHint : kotlin.String = idTokenHint_example // kotlin.String | id_token_hint
val postLogoutRedirectUri : kotlin.String = postLogoutRedirectUri_example // kotlin.String | post_logout_redirect_uri
val state : kotlin.String = state_example // kotlin.String | state
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerLogout(idTokenHint, postLogoutRedirectUri, state)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#iamApiControllerLogout")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#iamApiControllerLogout")
    e.printStackTrace()
}
```

### Parameters
| **idTokenHint** | **kotlin.String**| id_token_hint | [optional] |
| **postLogoutRedirectUri** | **kotlin.String**| post_logout_redirect_uri | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **state** | **kotlin.String**| state | [optional] |

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

<a id="iamApiControllerSignup"></a>
# **iamApiControllerSignup**
> IamControllersResponse iamApiControllerSignup(username, password)

Api Controller Signup

sign up a new user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
val username : kotlin.String = username_example // kotlin.String | The username to sign up
val password : kotlin.String = password_example // kotlin.String | The password
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerSignup(username, password)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#iamApiControllerSignup")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#iamApiControllerSignup")
    e.printStackTrace()
}
```

### Parameters
| **username** | **kotlin.String**| The username to sign up | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **password** | **kotlin.String**| The password | |

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

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json

<a id="iamApiControllerSsoLogoutGet"></a>
# **iamApiControllerSsoLogoutGet**
> IamControllersResponse iamApiControllerSsoLogoutGet(logoutAll)

Api Controller Sso Logout

logout the current user from all applications or current session only

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
val logoutAll : kotlin.String = logoutAll_example // kotlin.String | Whether to logout from all sessions. Accepted values: 'true', '1', or empty (default: true). Any other value means false.
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerSsoLogoutGet(logoutAll)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#iamApiControllerSsoLogoutGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#iamApiControllerSsoLogoutGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **logoutAll** | **kotlin.String**| Whether to logout from all sessions. Accepted values: &#39;true&#39;, &#39;1&#39;, or empty (default: true). Any other value means false. | [optional] |

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

<a id="iamApiControllerSsoLogoutPost"></a>
# **iamApiControllerSsoLogoutPost**
> IamControllersResponse iamApiControllerSsoLogoutPost(logoutAll)

Api Controller Sso Logout

logout the current user from all applications or current session only

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
val logoutAll : kotlin.String = logoutAll_example // kotlin.String | Whether to logout from all sessions. Accepted values: 'true', '1', or empty (default: true). Any other value means false.
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerSsoLogoutPost(logoutAll)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#iamApiControllerSsoLogoutPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#iamApiControllerSsoLogoutPost")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **logoutAll** | **kotlin.String**| Whether to logout from all sessions. Accepted values: &#39;true&#39;, &#39;1&#39;, or empty (default: true). Any other value means false. | [optional] |

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

<a id="iamApiControllerUnlink"></a>
# **iamApiControllerUnlink**
> IamObjectUserinfo iamApiControllerUnlink()

Api Controller Unlink

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
try {
    val result : IamObjectUserinfo = apiInstance.iamApiControllerUnlink()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#iamApiControllerUnlink")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#iamApiControllerUnlink")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**IamObjectUserinfo**](IamObjectUserinfo.md)

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

<a id="iamApiControllerWebAuthnSigninBegin"></a>
# **iamApiControllerWebAuthnSigninBegin**
> kotlin.Any iamApiControllerWebAuthnSigninBegin(owner, name)

Api Controller Web Authn Signin Begin

WebAuthn Login Flow 1st stage

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
val owner : kotlin.String = owner_example // kotlin.String | owner
val name : kotlin.String = name_example // kotlin.String | name
try {
    val result : kotlin.Any = apiInstance.iamApiControllerWebAuthnSigninBegin(owner, name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#iamApiControllerWebAuthnSigninBegin")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#iamApiControllerWebAuthnSigninBegin")
    e.printStackTrace()
}
```

### Parameters
| **owner** | **kotlin.String**| owner | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**| name | |

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

<a id="iamApiControllerWebAuthnSigninFinish"></a>
# **iamApiControllerWebAuthnSigninFinish**
> IamControllersResponse iamApiControllerWebAuthnSigninFinish(body)

Api Controller Web Authn Signin Finish

WebAuthn Login Flow 2nd stage

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
val body : kotlin.Any = Object // kotlin.Any | authenticator assertion Response
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerWebAuthnSigninFinish(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#iamApiControllerWebAuthnSigninFinish")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#iamApiControllerWebAuthnSigninFinish")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**| authenticator assertion Response | |

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

<a id="iamRootControllerGetJwks"></a>
# **iamRootControllerGetJwks**
> kotlin.Any iamRootControllerGetJwks()

Root Controller Get Jwks

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
try {
    val result : kotlin.Any = apiInstance.iamRootControllerGetJwks()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#iamRootControllerGetJwks")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#iamRootControllerGetJwks")
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

<a id="iamRootControllerGetJwksByApplication"></a>
# **iamRootControllerGetJwksByApplication**
> kotlin.Any iamRootControllerGetJwksByApplication(application)

Root Controller Get Jwks By Application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
val application : kotlin.String = application_example // kotlin.String | application name
try {
    val result : kotlin.Any = apiInstance.iamRootControllerGetJwksByApplication(application)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#iamRootControllerGetJwksByApplication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#iamRootControllerGetJwksByApplication")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **application** | **kotlin.String**| application name | |

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

<a id="iamRootControllerGetOidcDiscovery"></a>
# **iamRootControllerGetOidcDiscovery**
> IamObjectOidcDiscovery iamRootControllerGetOidcDiscovery()

Root Controller Get Oidc Discovery

Get Oidc Discovery

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
try {
    val result : IamObjectOidcDiscovery = apiInstance.iamRootControllerGetOidcDiscovery()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#iamRootControllerGetOidcDiscovery")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#iamRootControllerGetOidcDiscovery")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**IamObjectOidcDiscovery**](IamObjectOidcDiscovery.md)

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

<a id="iamRootControllerGetOidcDiscoveryByApplication"></a>
# **iamRootControllerGetOidcDiscoveryByApplication**
> IamObjectOidcDiscovery iamRootControllerGetOidcDiscoveryByApplication(application)

Root Controller Get Oidc Discovery By Application

Get Oidc Discovery for specific application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
val application : kotlin.String = application_example // kotlin.String | application name
try {
    val result : IamObjectOidcDiscovery = apiInstance.iamRootControllerGetOidcDiscoveryByApplication(application)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#iamRootControllerGetOidcDiscoveryByApplication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#iamRootControllerGetOidcDiscoveryByApplication")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **application** | **kotlin.String**| application name | |

### Return type

[**IamObjectOidcDiscovery**](IamObjectOidcDiscovery.md)

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

<a id="iamRootControllerGetWebFinger"></a>
# **iamRootControllerGetWebFinger**
> IamObjectWebFinger iamRootControllerGetWebFinger(resource)

Root Controller Get Web Finger

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
val resource : kotlin.String = resource_example // kotlin.String | resource
try {
    val result : IamObjectWebFinger = apiInstance.iamRootControllerGetWebFinger(resource)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#iamRootControllerGetWebFinger")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#iamRootControllerGetWebFinger")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **resource** | **kotlin.String**| resource | |

### Return type

[**IamObjectWebFinger**](IamObjectWebFinger.md)

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

<a id="iamRootControllerGetWebFingerByApplication"></a>
# **iamRootControllerGetWebFingerByApplication**
> IamObjectWebFinger iamRootControllerGetWebFingerByApplication(application, resource)

Root Controller Get Web Finger By Application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthenticationApi()
val application : kotlin.String = application_example // kotlin.String | application name
val resource : kotlin.String = resource_example // kotlin.String | resource
try {
    val result : IamObjectWebFinger = apiInstance.iamRootControllerGetWebFingerByApplication(application, resource)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#iamRootControllerGetWebFingerByApplication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#iamRootControllerGetWebFingerByApplication")
    e.printStackTrace()
}
```

### Parameters
| **application** | **kotlin.String**| application name | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **resource** | **kotlin.String**| resource | |

### Return type

[**IamObjectWebFinger**](IamObjectWebFinger.md)

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

