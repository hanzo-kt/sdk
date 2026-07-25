# MFAApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**iamApiControllerDeleteMfa**](MFAApi.md#iamApiControllerDeleteMfa) | **DELETE** /v1/iam/mfa/s/{id} | Api Controller Delete Mfa |
| [**iamApiControllerGetUserVerifications**](MFAApi.md#iamApiControllerGetUserVerifications) | **GET** /v1/iam/user-payments | Api Controller Get User Verifications |
| [**iamApiControllerGetVerification**](MFAApi.md#iamApiControllerGetVerification) | **GET** /v1/iam/payments/{id} | Api Controller Get Verification |
| [**iamApiControllerGetVerifications**](MFAApi.md#iamApiControllerGetVerifications) | **GET** /v1/iam/payments | Api Controller Get Verifications |
| [**iamApiControllerMfaSetupEnable**](MFAApi.md#iamApiControllerMfaSetupEnable) | **POST** /v1/iam/mfa/setup/enable | Api Controller Mfa Setup Enable |
| [**iamApiControllerMfaSetupInitiate**](MFAApi.md#iamApiControllerMfaSetupInitiate) | **POST** /v1/iam/mfa/setup/initiate | Api Controller Mfa Setup Initiate |
| [**iamApiControllerMfaSetupVerify**](MFAApi.md#iamApiControllerMfaSetupVerify) | **POST** /v1/iam/mfa/setup/verify | Api Controller Mfa Setup Verify |
| [**iamApiControllerSendVerificationCode**](MFAApi.md#iamApiControllerSendVerificationCode) | **POST** /v1/iam/auth/verification-code/send | Api Controller Send Verification Code |
| [**iamApiControllerSetPreferredMfa**](MFAApi.md#iamApiControllerSetPreferredMfa) | **POST** /v1/iam/mfa/preferred | Api Controller Set Preferred Mfa |
| [**iamApiControllerVerifyCaptcha**](MFAApi.md#iamApiControllerVerifyCaptcha) | **POST** /v1/iam/captcha/verify | Api Controller Verify Captcha |
| [**iamApiControllerVerifyCode**](MFAApi.md#iamApiControllerVerifyCode) | **POST** /v1/iam/auth/verification-code/verify | Api Controller Verify Code |


<a id="iamApiControllerDeleteMfa"></a>
# **iamApiControllerDeleteMfa**
> IamControllersResponse iamApiControllerDeleteMfa(id)

Api Controller Delete Mfa

: Delete MFA

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MFAApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeleteMfa(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MFAApi#iamApiControllerDeleteMfa")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MFAApi#iamApiControllerDeleteMfa")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| Resource identifier (owner/name) | |

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

<a id="iamApiControllerGetUserVerifications"></a>
# **iamApiControllerGetUserVerifications**
> kotlin.collections.List&lt;kotlin.Any&gt; iamApiControllerGetUserVerifications(owner, organization, user)

Api Controller Get User Verifications

get payments for a user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MFAApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of payments
val organization : kotlin.String = organization_example // kotlin.String | The organization of the user
val user : kotlin.String = user_example // kotlin.String | The username of the user
try {
    val result : kotlin.collections.List<kotlin.Any> = apiInstance.iamApiControllerGetUserVerifications(owner, organization, user)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MFAApi#iamApiControllerGetUserVerifications")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MFAApi#iamApiControllerGetUserVerifications")
    e.printStackTrace()
}
```

### Parameters
| **owner** | **kotlin.String**| The owner of payments | |
| **organization** | **kotlin.String**| The organization of the user | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **user** | **kotlin.String**| The username of the user | |

### Return type

[**kotlin.collections.List&lt;kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="iamApiControllerGetVerification"></a>
# **iamApiControllerGetVerification**
> kotlin.Any iamApiControllerGetVerification(id)

Api Controller Get Verification

get payment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MFAApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the payment
try {
    val result : kotlin.Any = apiInstance.iamApiControllerGetVerification(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MFAApi#iamApiControllerGetVerification")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MFAApi#iamApiControllerGetVerification")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the payment | |

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

<a id="iamApiControllerGetVerifications"></a>
# **iamApiControllerGetVerifications**
> kotlin.collections.List&lt;kotlin.Any&gt; iamApiControllerGetVerifications(owner)

Api Controller Get Verifications

get payments

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MFAApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of payments
try {
    val result : kotlin.collections.List<kotlin.Any> = apiInstance.iamApiControllerGetVerifications(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MFAApi#iamApiControllerGetVerifications")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MFAApi#iamApiControllerGetVerifications")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of payments | |

### Return type

[**kotlin.collections.List&lt;kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="iamApiControllerMfaSetupEnable"></a>
# **iamApiControllerMfaSetupEnable**
> IamControllersResponse iamApiControllerMfaSetupEnable()

Api Controller Mfa Setup Enable

enable totp

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MFAApi()
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerMfaSetupEnable()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MFAApi#iamApiControllerMfaSetupEnable")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MFAApi#iamApiControllerMfaSetupEnable")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

<a id="iamApiControllerMfaSetupInitiate"></a>
# **iamApiControllerMfaSetupInitiate**
> IamControllersResponse iamApiControllerMfaSetupInitiate()

Api Controller Mfa Setup Initiate

setup MFA

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MFAApi()
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerMfaSetupInitiate()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MFAApi#iamApiControllerMfaSetupInitiate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MFAApi#iamApiControllerMfaSetupInitiate")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

<a id="iamApiControllerMfaSetupVerify"></a>
# **iamApiControllerMfaSetupVerify**
> IamControllersResponse iamApiControllerMfaSetupVerify()

Api Controller Mfa Setup Verify

setup verify totp

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MFAApi()
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerMfaSetupVerify()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MFAApi#iamApiControllerMfaSetupVerify")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MFAApi#iamApiControllerMfaSetupVerify")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

<a id="iamApiControllerSendVerificationCode"></a>
# **iamApiControllerSendVerificationCode**
> IamObjectUserinfo iamApiControllerSendVerificationCode()

Api Controller Send Verification Code

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MFAApi()
try {
    val result : IamObjectUserinfo = apiInstance.iamApiControllerSendVerificationCode()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MFAApi#iamApiControllerSendVerificationCode")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MFAApi#iamApiControllerSendVerificationCode")
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

<a id="iamApiControllerSetPreferredMfa"></a>
# **iamApiControllerSetPreferredMfa**
> IamControllersResponse iamApiControllerSetPreferredMfa()

Api Controller Set Preferred Mfa

: Set specific Mfa Preferred

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MFAApi()
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerSetPreferredMfa()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MFAApi#iamApiControllerSetPreferredMfa")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MFAApi#iamApiControllerSetPreferredMfa")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

<a id="iamApiControllerVerifyCaptcha"></a>
# **iamApiControllerVerifyCaptcha**
> IamObjectUserinfo iamApiControllerVerifyCaptcha()

Api Controller Verify Captcha

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MFAApi()
try {
    val result : IamObjectUserinfo = apiInstance.iamApiControllerVerifyCaptcha()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MFAApi#iamApiControllerVerifyCaptcha")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MFAApi#iamApiControllerVerifyCaptcha")
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

<a id="iamApiControllerVerifyCode"></a>
# **iamApiControllerVerifyCode**
> IamObjectUserinfo iamApiControllerVerifyCode()

Api Controller Verify Code

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MFAApi()
try {
    val result : IamObjectUserinfo = apiInstance.iamApiControllerVerifyCode()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MFAApi#iamApiControllerVerifyCode")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MFAApi#iamApiControllerVerifyCode")
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

