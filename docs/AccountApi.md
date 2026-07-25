# AccountApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**commerceAccountExists**](AccountApi.md#commerceAccountExists) | **GET** /v1/commerce/account/exists/{emailorusername} | Check if account exists |
| [**commerceAccountLogin**](AccountApi.md#commerceAccountLogin) | **POST** /v1/commerce/account/login | Login to account |
| [**commerceAccountWithdraw**](AccountApi.md#commerceAccountWithdraw) | **POST** /v1/commerce/account/withdraw | Withdraw funds |
| [**commerceConfirmPasswordReset**](AccountApi.md#commerceConfirmPasswordReset) | **POST** /v1/commerce/account/confirm/{tokenid} | Confirm password reset |
| [**commerceCreateAccount**](AccountApi.md#commerceCreateAccount) | **POST** /v1/commerce/account/create | Create new account |
| [**commerceCreatePaymentMethod**](AccountApi.md#commerceCreatePaymentMethod) | **POST** /v1/commerce/account/paymentmethod/{paymentmethodtype} | Create payment method |
| [**commerceEnableAccount**](AccountApi.md#commerceEnableAccount) | **POST** /v1/commerce/account/enable/{tokenid} | Enable account with token |
| [**commerceGetAccount**](AccountApi.md#commerceGetAccount) | **GET** /v1/commerce/account | Get current account |
| [**commerceGetAccountOrder**](AccountApi.md#commerceGetAccountOrder) | **GET** /v1/commerce/account/order/{orderid} | Get account order |
| [**commercePatchAccount**](AccountApi.md#commercePatchAccount) | **PATCH** /v1/commerce/account | Partially update account |
| [**commercePatchAccountOrder**](AccountApi.md#commercePatchAccountOrder) | **PATCH** /v1/commerce/account/order/{orderid} | Update account order |
| [**commerceRequestPasswordReset**](AccountApi.md#commerceRequestPasswordReset) | **POST** /v1/commerce/account/reset | Request password reset |
| [**commerceUpdateAccount**](AccountApi.md#commerceUpdateAccount) | **PUT** /v1/commerce/account | Update account |


<a id="commerceAccountExists"></a>
# **commerceAccountExists**
> CommerceAccountExists200Response commerceAccountExists(emailorusername)

Check if account exists

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AccountApi()
val emailorusername : kotlin.String = emailorusername_example // kotlin.String | 
try {
    val result : CommerceAccountExists200Response = apiInstance.commerceAccountExists(emailorusername)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountApi#commerceAccountExists")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountApi#commerceAccountExists")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **emailorusername** | **kotlin.String**|  | |

### Return type

[**CommerceAccountExists200Response**](CommerceAccountExists200Response.md)

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

<a id="commerceAccountLogin"></a>
# **commerceAccountLogin**
> CommerceUser commerceAccountLogin(chatPostAuthLoginRequest)

Login to account

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AccountApi()
val chatPostAuthLoginRequest : ChatPostAuthLoginRequest =  // ChatPostAuthLoginRequest | 
try {
    val result : CommerceUser = apiInstance.commerceAccountLogin(chatPostAuthLoginRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountApi#commerceAccountLogin")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountApi#commerceAccountLogin")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostAuthLoginRequest** | [**ChatPostAuthLoginRequest**](ChatPostAuthLoginRequest.md)|  | |

### Return type

[**CommerceUser**](CommerceUser.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="commerceAccountWithdraw"></a>
# **commerceAccountWithdraw**
> kotlin.Any commerceAccountWithdraw(commerceAccountWithdrawRequest)

Withdraw funds

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AccountApi()
val commerceAccountWithdrawRequest : CommerceAccountWithdrawRequest =  // CommerceAccountWithdrawRequest | 
try {
    val result : kotlin.Any = apiInstance.commerceAccountWithdraw(commerceAccountWithdrawRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountApi#commerceAccountWithdraw")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountApi#commerceAccountWithdraw")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceAccountWithdrawRequest** | [**CommerceAccountWithdrawRequest**](CommerceAccountWithdrawRequest.md)|  | |

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

<a id="commerceConfirmPasswordReset"></a>
# **commerceConfirmPasswordReset**
> kotlin.Any commerceConfirmPasswordReset(tokenid, commerceConfirmPasswordResetRequest)

Confirm password reset

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AccountApi()
val tokenid : kotlin.String = tokenid_example // kotlin.String | 
val commerceConfirmPasswordResetRequest : CommerceConfirmPasswordResetRequest =  // CommerceConfirmPasswordResetRequest | 
try {
    val result : kotlin.Any = apiInstance.commerceConfirmPasswordReset(tokenid, commerceConfirmPasswordResetRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountApi#commerceConfirmPasswordReset")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountApi#commerceConfirmPasswordReset")
    e.printStackTrace()
}
```

### Parameters
| **tokenid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceConfirmPasswordResetRequest** | [**CommerceConfirmPasswordResetRequest**](CommerceConfirmPasswordResetRequest.md)|  | |

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

<a id="commerceCreateAccount"></a>
# **commerceCreateAccount**
> CommerceUser commerceCreateAccount(commerceCreateAccountRequest)

Create new account

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AccountApi()
val commerceCreateAccountRequest : CommerceCreateAccountRequest =  // CommerceCreateAccountRequest | 
try {
    val result : CommerceUser = apiInstance.commerceCreateAccount(commerceCreateAccountRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountApi#commerceCreateAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountApi#commerceCreateAccount")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceCreateAccountRequest** | [**CommerceCreateAccountRequest**](CommerceCreateAccountRequest.md)|  | |

### Return type

[**CommerceUser**](CommerceUser.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="commerceCreatePaymentMethod"></a>
# **commerceCreatePaymentMethod**
> CommercePaymentMethod commerceCreatePaymentMethod(paymentmethodtype, commercePaymentMethod)

Create payment method

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AccountApi()
val paymentmethodtype : kotlin.String = paymentmethodtype_example // kotlin.String | 
val commercePaymentMethod : CommercePaymentMethod =  // CommercePaymentMethod | 
try {
    val result : CommercePaymentMethod = apiInstance.commerceCreatePaymentMethod(paymentmethodtype, commercePaymentMethod)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountApi#commerceCreatePaymentMethod")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountApi#commerceCreatePaymentMethod")
    e.printStackTrace()
}
```

### Parameters
| **paymentmethodtype** | **kotlin.String**|  | [enum: card, paypal, bank] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commercePaymentMethod** | [**CommercePaymentMethod**](CommercePaymentMethod.md)|  | |

### Return type

[**CommercePaymentMethod**](CommercePaymentMethod.md)

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

<a id="commerceEnableAccount"></a>
# **commerceEnableAccount**
> kotlin.Any commerceEnableAccount(tokenid)

Enable account with token

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AccountApi()
val tokenid : kotlin.String = tokenid_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.commerceEnableAccount(tokenid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountApi#commerceEnableAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountApi#commerceEnableAccount")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **tokenid** | **kotlin.String**|  | |

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

<a id="commerceGetAccount"></a>
# **commerceGetAccount**
> CommerceUser commerceGetAccount()

Get current account

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AccountApi()
try {
    val result : CommerceUser = apiInstance.commerceGetAccount()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountApi#commerceGetAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountApi#commerceGetAccount")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**CommerceUser**](CommerceUser.md)

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

<a id="commerceGetAccountOrder"></a>
# **commerceGetAccountOrder**
> CommerceOrder commerceGetAccountOrder(orderid)

Get account order

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AccountApi()
val orderid : kotlin.String = orderid_example // kotlin.String | 
try {
    val result : CommerceOrder = apiInstance.commerceGetAccountOrder(orderid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountApi#commerceGetAccountOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountApi#commerceGetAccountOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderid** | **kotlin.String**|  | |

### Return type

[**CommerceOrder**](CommerceOrder.md)

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

<a id="commercePatchAccount"></a>
# **commercePatchAccount**
> CommerceUser commercePatchAccount(commerceUser)

Partially update account

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AccountApi()
val commerceUser : CommerceUser =  // CommerceUser | 
try {
    val result : CommerceUser = apiInstance.commercePatchAccount(commerceUser)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountApi#commercePatchAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountApi#commercePatchAccount")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceUser** | [**CommerceUser**](CommerceUser.md)|  | |

### Return type

[**CommerceUser**](CommerceUser.md)

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

<a id="commercePatchAccountOrder"></a>
# **commercePatchAccountOrder**
> CommerceOrder commercePatchAccountOrder(orderid, commerceOrder)

Update account order

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AccountApi()
val orderid : kotlin.String = orderid_example // kotlin.String | 
val commerceOrder : CommerceOrder =  // CommerceOrder | 
try {
    val result : CommerceOrder = apiInstance.commercePatchAccountOrder(orderid, commerceOrder)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountApi#commercePatchAccountOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountApi#commercePatchAccountOrder")
    e.printStackTrace()
}
```

### Parameters
| **orderid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceOrder** | [**CommerceOrder**](CommerceOrder.md)|  | |

### Return type

[**CommerceOrder**](CommerceOrder.md)

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

<a id="commerceRequestPasswordReset"></a>
# **commerceRequestPasswordReset**
> kotlin.Any commerceRequestPasswordReset(chatPostAuthRequestpasswordresetRequest)

Request password reset

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AccountApi()
val chatPostAuthRequestpasswordresetRequest : ChatPostAuthRequestpasswordresetRequest =  // ChatPostAuthRequestpasswordresetRequest | 
try {
    val result : kotlin.Any = apiInstance.commerceRequestPasswordReset(chatPostAuthRequestpasswordresetRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountApi#commerceRequestPasswordReset")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountApi#commerceRequestPasswordReset")
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

<a id="commerceUpdateAccount"></a>
# **commerceUpdateAccount**
> CommerceUser commerceUpdateAccount(commerceUser)

Update account

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AccountApi()
val commerceUser : CommerceUser =  // CommerceUser | 
try {
    val result : CommerceUser = apiInstance.commerceUpdateAccount(commerceUser)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountApi#commerceUpdateAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountApi#commerceUpdateAccount")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceUser** | [**CommerceUser**](CommerceUser.md)|  | |

### Return type

[**CommerceUser**](CommerceUser.md)

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

