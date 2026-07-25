# UsersApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**analyticsCreateUser**](UsersApi.md#analyticsCreateUser) | **POST** /v1/analytics/users | Create a new user (admin only) |
| [**analyticsDeleteUser**](UsersApi.md#analyticsDeleteUser) | **DELETE** /v1/analytics/users/{userId} | Delete user (admin only) |
| [**analyticsGetUser**](UsersApi.md#analyticsGetUser) | **GET** /v1/analytics/users/{userId} | Get user by ID |
| [**analyticsGetUserTeams**](UsersApi.md#analyticsGetUserTeams) | **GET** /v1/analytics/users/{userId}/teams | List teams a user belongs to |
| [**analyticsGetUserUsage**](UsersApi.md#analyticsGetUserUsage) | **GET** /v1/analytics/users/{userId}/usage | Get event usage breakdown for a user (admin only) |
| [**analyticsGetUserWebsites**](UsersApi.md#analyticsGetUserWebsites) | **GET** /v1/analytics/users/{userId}/websites | List websites owned by a user |
| [**analyticsUpdateUser**](UsersApi.md#analyticsUpdateUser) | **POST** /v1/analytics/users/{userId} | Update user |
| [**autoListUsers**](UsersApi.md#autoListUsers) | **GET** /v1/auto/users | List platform users |
| [**botGetUser**](UsersApi.md#botGetUser) | **GET** /v1/bot/users/{handle} | Get user profile by handle |
| [**botListUserSkills**](UsersApi.md#botListUserSkills) | **GET** /v1/bot/users/{handle}/skills | List skills published by a user |
| [**botListUserStars**](UsersApi.md#botListUserStars) | **GET** /v1/bot/users/{handle}/stars | List skills starred by a user |
| [**botUpdateProfile**](UsersApi.md#botUpdateProfile) | **PATCH** /v1/bot/users/me | Update current user&#39;s profile |
| [**commerceCreateUser**](UsersApi.md#commerceCreateUser) | **POST** /v1/commerce/user | Create user |
| [**commerceCreateWalletAccount**](UsersApi.md#commerceCreateWalletAccount) | **POST** /v1/commerce/user/{userid}/wallet/account | Create wallet account |
| [**commerceDeleteUser**](UsersApi.md#commerceDeleteUser) | **DELETE** /v1/commerce/user/{userid} | Delete user |
| [**commerceGetUser**](UsersApi.md#commerceGetUser) | **GET** /v1/commerce/user/{userid} | Get user |
| [**commerceGetUserOrders**](UsersApi.md#commerceGetUserOrders) | **GET** /v1/commerce/user/{userid}/orders | Get user orders |
| [**commerceGetUserPaymentMethods**](UsersApi.md#commerceGetUserPaymentMethods) | **GET** /v1/commerce/user/{userid}/paymentmethods | Get user payment methods |
| [**commerceGetUserReferrals**](UsersApi.md#commerceGetUserReferrals) | **GET** /v1/commerce/user/{userid}/referrals | Get user referrals |
| [**commerceGetUserReferrers**](UsersApi.md#commerceGetUserReferrers) | **GET** /v1/commerce/user/{userid}/referrers | Get user referrers |
| [**commerceGetUserTransactions**](UsersApi.md#commerceGetUserTransactions) | **GET** /v1/commerce/user/{userid}/transactions | Get user transactions |
| [**commerceGetUserWallet**](UsersApi.md#commerceGetUserWallet) | **GET** /v1/commerce/user/{userid}/wallet | Get user wallet |
| [**commerceGetWalletAccount**](UsersApi.md#commerceGetWalletAccount) | **GET** /v1/commerce/user/{userid}/wallet/account/{name} | Get wallet account |
| [**commerceListUsers**](UsersApi.md#commerceListUsers) | **GET** /v1/commerce/user | List users |
| [**commercePatchUser**](UsersApi.md#commercePatchUser) | **PATCH** /v1/commerce/user/{userid} | Partially update user |
| [**commerceResetUserPassword**](UsersApi.md#commerceResetUserPassword) | **GET** /v1/commerce/user/{userid}/password/reset | Reset user password (admin) |
| [**commerceUpdateUser**](UsersApi.md#commerceUpdateUser) | **PUT** /v1/commerce/user/{userid} | Update user |
| [**commerceWalletPay**](UsersApi.md#commerceWalletPay) | **POST** /v1/commerce/user/{userid}/wallet/pay | Send payment from wallet |
| [**flowGetUser**](UsersApi.md#flowGetUser) | **GET** /v1/flow/users/{id} | Get user by id |
| [**flowListUsers**](UsersApi.md#flowListUsers) | **GET** /v1/flow/users | List platform users |
| [**iamApiControllerAddLdap**](UsersApi.md#iamApiControllerAddLdap) | **POST** /v1/iam/ldaps | Api Controller Add Ldap |
| [**iamApiControllerAddUser**](UsersApi.md#iamApiControllerAddUser) | **POST** /v1/iam/users | Api Controller Add User |
| [**iamApiControllerAddUserKeys**](UsersApi.md#iamApiControllerAddUserKeys) | **POST** /v1/iam/user-keys | Api Controller Add User Keys |
| [**iamApiControllerCheckUserPassword**](UsersApi.md#iamApiControllerCheckUserPassword) | **POST** /v1/iam/auth/check-password | Api Controller Check User Password |
| [**iamApiControllerDeleteLdap**](UsersApi.md#iamApiControllerDeleteLdap) | **DELETE** /v1/iam/ldaps/{id} | Api Controller Delete Ldap |
| [**iamApiControllerDeleteUser**](UsersApi.md#iamApiControllerDeleteUser) | **DELETE** /v1/iam/users/{id} | Api Controller Delete User |
| [**iamApiControllerExitImpersonateUser**](UsersApi.md#iamApiControllerExitImpersonateUser) | **POST** /v1/iam/impersonation/exit | Api Controller Exit Impersonate User |
| [**iamApiControllerGetAccount**](UsersApi.md#iamApiControllerGetAccount) | **GET** /v1/iam/accounts/{id} | Api Controller Get Account |
| [**iamApiControllerGetEmailAndPhone**](UsersApi.md#iamApiControllerGetEmailAndPhone) | **GET** /v1/iam/auth/contact | Api Controller Get Email And Phone |
| [**iamApiControllerGetGlobalUsers**](UsersApi.md#iamApiControllerGetGlobalUsers) | **GET** /v1/iam/global-users | Api Controller Get Global Users |
| [**iamApiControllerGetLdap**](UsersApi.md#iamApiControllerGetLdap) | **GET** /v1/iam/ldaps/{id} | Api Controller Get Ldap |
| [**iamApiControllerGetLdaps**](UsersApi.md#iamApiControllerGetLdaps) | **GET** /v1/iam/ldaps | Api Controller Get Ldaps |
| [**iamApiControllerGetLdapser**](UsersApi.md#iamApiControllerGetLdapser) | **GET** /v1/iam/ldap-users | Api Controller Get Ldapser |
| [**iamApiControllerGetSortedUsers**](UsersApi.md#iamApiControllerGetSortedUsers) | **GET** /v1/iam/sorted-users | Api Controller Get Sorted Users |
| [**iamApiControllerGetUser**](UsersApi.md#iamApiControllerGetUser) | **GET** /v1/iam/users/{id} | Api Controller Get User |
| [**iamApiControllerGetUserCount**](UsersApi.md#iamApiControllerGetUserCount) | **GET** /v1/iam/user-counts/{id} | Api Controller Get User Count |
| [**iamApiControllerGetUsers**](UsersApi.md#iamApiControllerGetUsers) | **GET** /v1/iam/users | Api Controller Get Users |
| [**iamApiControllerImpersonateUser**](UsersApi.md#iamApiControllerImpersonateUser) | **POST** /v1/iam/impersonation-user | Api Controller Impersonate User |
| [**iamApiControllerResetEmailOrPhone**](UsersApi.md#iamApiControllerResetEmailOrPhone) | **POST** /v1/iam/auth/reset-contact | Api Controller Reset Email Or Phone |
| [**iamApiControllerSetPassword**](UsersApi.md#iamApiControllerSetPassword) | **POST** /v1/iam/auth/set-password | Api Controller Set Password |
| [**iamApiControllerSyncLdapUsers**](UsersApi.md#iamApiControllerSyncLdapUsers) | **POST** /v1/iam/ldap/sync | Api Controller Sync Ldap Users |
| [**iamApiControllerUpdateLdap**](UsersApi.md#iamApiControllerUpdateLdap) | **PUT** /v1/iam/ldaps/{id} | Api Controller Update Ldap |
| [**iamApiControllerUpdateUser**](UsersApi.md#iamApiControllerUpdateUser) | **PUT** /v1/iam/users/{id} | Api Controller Update User |
| [**iamApiControllerUserInfo**](UsersApi.md#iamApiControllerUserInfo) | **GET** /oauth/userinfo | Api Controller User Info |
| [**iamApiControllerUserInfo2**](UsersApi.md#iamApiControllerUserInfo2) | **GET** /v1/iam/user | Api Controller User Info2 |
| [**iamApiControllerVerifyIdentification**](UsersApi.md#iamApiControllerVerifyIdentification) | **POST** /v1/iam/auth/identification/verify | Api Controller Verify Identification |
| [**iamApiControllerWebAuthnSignupBegin**](UsersApi.md#iamApiControllerWebAuthnSignupBegin) | **GET** /v1/iam/auth/webauthn/signup/begin | Api Controller Web Authn Signup Begin |
| [**iamApiControllerWebAuthnSignupFinish**](UsersApi.md#iamApiControllerWebAuthnSignupFinish) | **POST** /v1/iam/auth/webauthn/signup/finish | Api Controller Web Authn Signup Finish |
| [**kmsGetCurrentUser**](UsersApi.md#kmsGetCurrentUser) | **GET** /v1/kms/user | Get the current authenticated user |


<a id="analyticsCreateUser"></a>
# **analyticsCreateUser**
> AnalyticsUser analyticsCreateUser(analyticsCreateUserRequest)

Create a new user (admin only)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val analyticsCreateUserRequest : AnalyticsCreateUserRequest =  // AnalyticsCreateUserRequest | 
try {
    val result : AnalyticsUser = apiInstance.analyticsCreateUser(analyticsCreateUserRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#analyticsCreateUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#analyticsCreateUser")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **analyticsCreateUserRequest** | [**AnalyticsCreateUserRequest**](AnalyticsCreateUserRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="analyticsDeleteUser"></a>
# **analyticsDeleteUser**
> kotlin.Any analyticsDeleteUser(userId)

Delete user (admin only)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val userId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.analyticsDeleteUser(userId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#analyticsDeleteUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#analyticsDeleteUser")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **userId** | **java.util.UUID**|  | |

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

<a id="analyticsGetUser"></a>
# **analyticsGetUser**
> AnalyticsUser analyticsGetUser(userId)

Get user by ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val userId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : AnalyticsUser = apiInstance.analyticsGetUser(userId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#analyticsGetUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#analyticsGetUser")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **userId** | **java.util.UUID**|  | |

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

<a id="analyticsGetUserTeams"></a>
# **analyticsGetUserTeams**
> kotlin.collections.List&lt;AnalyticsTeam&gt; analyticsGetUserTeams(userId, page, pageSize, orderBy, search)

List teams a user belongs to

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val userId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val orderBy : kotlin.String = orderBy_example // kotlin.String | 
val search : kotlin.String = search_example // kotlin.String | 
try {
    val result : kotlin.collections.List<AnalyticsTeam> = apiInstance.analyticsGetUserTeams(userId, page, pageSize, orderBy, search)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#analyticsGetUserTeams")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#analyticsGetUserTeams")
    e.printStackTrace()
}
```

### Parameters
| **userId** | **java.util.UUID**|  | |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **orderBy** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **search** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;AnalyticsTeam&gt;**](AnalyticsTeam.md)

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

<a id="analyticsGetUserUsage"></a>
# **analyticsGetUserUsage**
> AnalyticsGetUserUsage200Response analyticsGetUserUsage(userId, startAt, endAt)

Get event usage breakdown for a user (admin only)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val userId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val startAt : kotlin.Long = 789 // kotlin.Long | Start timestamp in milliseconds
val endAt : kotlin.Long = 789 // kotlin.Long | End timestamp in milliseconds
try {
    val result : AnalyticsGetUserUsage200Response = apiInstance.analyticsGetUserUsage(userId, startAt, endAt)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#analyticsGetUserUsage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#analyticsGetUserUsage")
    e.printStackTrace()
}
```

### Parameters
| **userId** | **java.util.UUID**|  | |
| **startAt** | **kotlin.Long**| Start timestamp in milliseconds | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **endAt** | **kotlin.Long**| End timestamp in milliseconds | |

### Return type

[**AnalyticsGetUserUsage200Response**](AnalyticsGetUserUsage200Response.md)

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

<a id="analyticsGetUserWebsites"></a>
# **analyticsGetUserWebsites**
> kotlin.collections.List&lt;AnalyticsWebsite&gt; analyticsGetUserWebsites(userId, page, pageSize, orderBy, search)

List websites owned by a user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val userId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val orderBy : kotlin.String = orderBy_example // kotlin.String | 
val search : kotlin.String = search_example // kotlin.String | 
try {
    val result : kotlin.collections.List<AnalyticsWebsite> = apiInstance.analyticsGetUserWebsites(userId, page, pageSize, orderBy, search)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#analyticsGetUserWebsites")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#analyticsGetUserWebsites")
    e.printStackTrace()
}
```

### Parameters
| **userId** | **java.util.UUID**|  | |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **orderBy** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **search** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;AnalyticsWebsite&gt;**](AnalyticsWebsite.md)

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

<a id="analyticsUpdateUser"></a>
# **analyticsUpdateUser**
> AnalyticsUser analyticsUpdateUser(userId, analyticsUpdateUserRequest)

Update user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val userId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val analyticsUpdateUserRequest : AnalyticsUpdateUserRequest =  // AnalyticsUpdateUserRequest | 
try {
    val result : AnalyticsUser = apiInstance.analyticsUpdateUser(userId, analyticsUpdateUserRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#analyticsUpdateUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#analyticsUpdateUser")
    e.printStackTrace()
}
```

### Parameters
| **userId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **analyticsUpdateUserRequest** | [**AnalyticsUpdateUserRequest**](AnalyticsUpdateUserRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="autoListUsers"></a>
# **autoListUsers**
> kotlin.Any autoListUsers()

List platform users

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
try {
    val result : kotlin.Any = apiInstance.autoListUsers()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#autoListUsers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#autoListUsers")
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

<a id="botGetUser"></a>
# **botGetUser**
> BotUser botGetUser(handle)

Get user profile by handle

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val handle : kotlin.String = handle_example // kotlin.String | 
try {
    val result : BotUser = apiInstance.botGetUser(handle)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#botGetUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#botGetUser")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **handle** | **kotlin.String**|  | |

### Return type

[**BotUser**](BotUser.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="botListUserSkills"></a>
# **botListUserSkills**
> BotListUserSkills200Response botListUserSkills(handle)

List skills published by a user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val handle : kotlin.String = handle_example // kotlin.String | 
try {
    val result : BotListUserSkills200Response = apiInstance.botListUserSkills(handle)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#botListUserSkills")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#botListUserSkills")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **handle** | **kotlin.String**|  | |

### Return type

[**BotListUserSkills200Response**](BotListUserSkills200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="botListUserStars"></a>
# **botListUserStars**
> BotListUserStars200Response botListUserStars(handle)

List skills starred by a user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val handle : kotlin.String = handle_example // kotlin.String | 
try {
    val result : BotListUserStars200Response = apiInstance.botListUserStars(handle)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#botListUserStars")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#botListUserStars")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **handle** | **kotlin.String**|  | |

### Return type

[**BotListUserStars200Response**](BotListUserStars200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="botUpdateProfile"></a>
# **botUpdateProfile**
> AnalyticsHeartbeat200Response botUpdateProfile(botUpdateProfileRequest)

Update current user&#39;s profile

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val botUpdateProfileRequest : BotUpdateProfileRequest =  // BotUpdateProfileRequest | 
try {
    val result : AnalyticsHeartbeat200Response = apiInstance.botUpdateProfile(botUpdateProfileRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#botUpdateProfile")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#botUpdateProfile")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **botUpdateProfileRequest** | [**BotUpdateProfileRequest**](BotUpdateProfileRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="commerceCreateUser"></a>
# **commerceCreateUser**
> CommerceUser commerceCreateUser(commerceUser)

Create user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val commerceUser : CommerceUser =  // CommerceUser | 
try {
    val result : CommerceUser = apiInstance.commerceCreateUser(commerceUser)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#commerceCreateUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#commerceCreateUser")
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

<a id="commerceCreateWalletAccount"></a>
# **commerceCreateWalletAccount**
> kotlin.Any commerceCreateWalletAccount(userid, commerceCreateWalletAccountRequest)

Create wallet account

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val userid : kotlin.String = userid_example // kotlin.String | 
val commerceCreateWalletAccountRequest : CommerceCreateWalletAccountRequest =  // CommerceCreateWalletAccountRequest | 
try {
    val result : kotlin.Any = apiInstance.commerceCreateWalletAccount(userid, commerceCreateWalletAccountRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#commerceCreateWalletAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#commerceCreateWalletAccount")
    e.printStackTrace()
}
```

### Parameters
| **userid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceCreateWalletAccountRequest** | [**CommerceCreateWalletAccountRequest**](CommerceCreateWalletAccountRequest.md)|  | |

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

<a id="commerceDeleteUser"></a>
# **commerceDeleteUser**
> commerceDeleteUser(userid)

Delete user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val userid : kotlin.String = userid_example // kotlin.String | 
try {
    apiInstance.commerceDeleteUser(userid)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#commerceDeleteUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#commerceDeleteUser")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **userid** | **kotlin.String**|  | |

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

<a id="commerceGetUser"></a>
# **commerceGetUser**
> CommerceUser commerceGetUser(userid)

Get user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val userid : kotlin.String = userid_example // kotlin.String | 
try {
    val result : CommerceUser = apiInstance.commerceGetUser(userid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#commerceGetUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#commerceGetUser")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **userid** | **kotlin.String**|  | |

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

<a id="commerceGetUserOrders"></a>
# **commerceGetUserOrders**
> kotlin.collections.List&lt;CommerceOrder&gt; commerceGetUserOrders(userid)

Get user orders

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val userid : kotlin.String = userid_example // kotlin.String | 
try {
    val result : kotlin.collections.List<CommerceOrder> = apiInstance.commerceGetUserOrders(userid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#commerceGetUserOrders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#commerceGetUserOrders")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **userid** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.List&lt;CommerceOrder&gt;**](CommerceOrder.md)

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

<a id="commerceGetUserPaymentMethods"></a>
# **commerceGetUserPaymentMethods**
> kotlin.collections.List&lt;CommercePaymentMethod&gt; commerceGetUserPaymentMethods(userid)

Get user payment methods

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val userid : kotlin.String = userid_example // kotlin.String | 
try {
    val result : kotlin.collections.List<CommercePaymentMethod> = apiInstance.commerceGetUserPaymentMethods(userid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#commerceGetUserPaymentMethods")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#commerceGetUserPaymentMethods")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **userid** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.List&lt;CommercePaymentMethod&gt;**](CommercePaymentMethod.md)

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

<a id="commerceGetUserReferrals"></a>
# **commerceGetUserReferrals**
> kotlin.collections.List&lt;CommerceReferral&gt; commerceGetUserReferrals(userid)

Get user referrals

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val userid : kotlin.String = userid_example // kotlin.String | 
try {
    val result : kotlin.collections.List<CommerceReferral> = apiInstance.commerceGetUserReferrals(userid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#commerceGetUserReferrals")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#commerceGetUserReferrals")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **userid** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.List&lt;CommerceReferral&gt;**](CommerceReferral.md)

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

<a id="commerceGetUserReferrers"></a>
# **commerceGetUserReferrers**
> kotlin.collections.List&lt;CommerceReferrer&gt; commerceGetUserReferrers(userid)

Get user referrers

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val userid : kotlin.String = userid_example // kotlin.String | 
try {
    val result : kotlin.collections.List<CommerceReferrer> = apiInstance.commerceGetUserReferrers(userid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#commerceGetUserReferrers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#commerceGetUserReferrers")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **userid** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.List&lt;CommerceReferrer&gt;**](CommerceReferrer.md)

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

<a id="commerceGetUserTransactions"></a>
# **commerceGetUserTransactions**
> kotlin.collections.Map&lt;kotlin.String, CommerceTransactionData&gt; commerceGetUserTransactions(userid)

Get user transactions

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val userid : kotlin.String = userid_example // kotlin.String | 
try {
    val result : kotlin.collections.Map<kotlin.String, CommerceTransactionData> = apiInstance.commerceGetUserTransactions(userid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#commerceGetUserTransactions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#commerceGetUserTransactions")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **userid** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.Map&lt;kotlin.String, CommerceTransactionData&gt;**](CommerceTransactionData.md)

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

<a id="commerceGetUserWallet"></a>
# **commerceGetUserWallet**
> CommerceWallet commerceGetUserWallet(userid)

Get user wallet

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val userid : kotlin.String = userid_example // kotlin.String | 
try {
    val result : CommerceWallet = apiInstance.commerceGetUserWallet(userid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#commerceGetUserWallet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#commerceGetUserWallet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **userid** | **kotlin.String**|  | |

### Return type

[**CommerceWallet**](CommerceWallet.md)

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

<a id="commerceGetWalletAccount"></a>
# **commerceGetWalletAccount**
> CommerceWalletAccount commerceGetWalletAccount(userid, name)

Get wallet account

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val userid : kotlin.String = userid_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
try {
    val result : CommerceWalletAccount = apiInstance.commerceGetWalletAccount(userid, name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#commerceGetWalletAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#commerceGetWalletAccount")
    e.printStackTrace()
}
```

### Parameters
| **userid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | |

### Return type

[**CommerceWalletAccount**](CommerceWalletAccount.md)

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

<a id="commerceListUsers"></a>
# **commerceListUsers**
> CommercePaginatedUsers commerceListUsers(page, display, sort, q)

List users

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val page : kotlin.Int = 56 // kotlin.Int | Page number (1-indexed)
val display : kotlin.Int = 56 // kotlin.Int | Number of items per page
val sort : kotlin.String = sort_example // kotlin.String | Sort field (prefix with - for descending)
val q : kotlin.String = q_example // kotlin.String | Search query
try {
    val result : CommercePaginatedUsers = apiInstance.commerceListUsers(page, display, sort, q)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#commerceListUsers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#commerceListUsers")
    e.printStackTrace()
}
```

### Parameters
| **page** | **kotlin.Int**| Page number (1-indexed) | [optional] [default to 1] |
| **display** | **kotlin.Int**| Number of items per page | [optional] [default to 20] |
| **sort** | **kotlin.String**| Sort field (prefix with - for descending) | [optional] [default to &quot;-UpdatedAt&quot;] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **q** | **kotlin.String**| Search query | [optional] |

### Return type

[**CommercePaginatedUsers**](CommercePaginatedUsers.md)

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

<a id="commercePatchUser"></a>
# **commercePatchUser**
> CommerceUser commercePatchUser(userid, commerceUser)

Partially update user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val userid : kotlin.String = userid_example // kotlin.String | 
val commerceUser : CommerceUser =  // CommerceUser | 
try {
    val result : CommerceUser = apiInstance.commercePatchUser(userid, commerceUser)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#commercePatchUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#commercePatchUser")
    e.printStackTrace()
}
```

### Parameters
| **userid** | **kotlin.String**|  | |
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

<a id="commerceResetUserPassword"></a>
# **commerceResetUserPassword**
> kotlin.Any commerceResetUserPassword(userid)

Reset user password (admin)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val userid : kotlin.String = userid_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.commerceResetUserPassword(userid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#commerceResetUserPassword")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#commerceResetUserPassword")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **userid** | **kotlin.String**|  | |

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

<a id="commerceUpdateUser"></a>
# **commerceUpdateUser**
> CommerceUser commerceUpdateUser(userid, commerceUser)

Update user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val userid : kotlin.String = userid_example // kotlin.String | 
val commerceUser : CommerceUser =  // CommerceUser | 
try {
    val result : CommerceUser = apiInstance.commerceUpdateUser(userid, commerceUser)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#commerceUpdateUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#commerceUpdateUser")
    e.printStackTrace()
}
```

### Parameters
| **userid** | **kotlin.String**|  | |
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

<a id="commerceWalletPay"></a>
# **commerceWalletPay**
> kotlin.Any commerceWalletPay(userid, commerceWalletPayRequest)

Send payment from wallet

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val userid : kotlin.String = userid_example // kotlin.String | 
val commerceWalletPayRequest : CommerceWalletPayRequest =  // CommerceWalletPayRequest | 
try {
    val result : kotlin.Any = apiInstance.commerceWalletPay(userid, commerceWalletPayRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#commerceWalletPay")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#commerceWalletPay")
    e.printStackTrace()
}
```

### Parameters
| **userid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceWalletPayRequest** | [**CommerceWalletPayRequest**](CommerceWalletPayRequest.md)|  | |

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

<a id="flowGetUser"></a>
# **flowGetUser**
> FlowUser flowGetUser(id)

Get user by id

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : FlowUser = apiInstance.flowGetUser(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#flowGetUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#flowGetUser")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**FlowUser**](FlowUser.md)

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

<a id="flowListUsers"></a>
# **flowListUsers**
> FlowListUsers200Response flowListUsers(cursor, limit)

List platform users

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val cursor : kotlin.String = cursor_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : FlowListUsers200Response = apiInstance.flowListUsers(cursor, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#flowListUsers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#flowListUsers")
    e.printStackTrace()
}
```

### Parameters
| **cursor** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] |

### Return type

[**FlowListUsers200Response**](FlowListUsers200Response.md)

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

<a id="iamApiControllerAddLdap"></a>
# **iamApiControllerAddLdap**
> IamControllersResponse iamApiControllerAddLdap(iamObjectLdap)

Api Controller Add Ldap

add ldap

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val iamObjectLdap : IamObjectLdap =  // IamObjectLdap | The details of the ldap
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddLdap(iamObjectLdap)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerAddLdap")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerAddLdap")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectLdap** | [**IamObjectLdap**](IamObjectLdap.md)| The details of the ldap | |

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

<a id="iamApiControllerAddUser"></a>
# **iamApiControllerAddUser**
> IamControllersResponse iamApiControllerAddUser(iamObjectUser)

Api Controller Add User

add user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val iamObjectUser : IamObjectUser =  // IamObjectUser | The details of the user
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddUser(iamObjectUser)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerAddUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerAddUser")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectUser** | [**IamObjectUser**](IamObjectUser.md)| The details of the user | |

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

<a id="iamApiControllerAddUserKeys"></a>
# **iamApiControllerAddUserKeys**
> IamObjectUserinfo iamApiControllerAddUserKeys()

Api Controller Add User Keys

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
try {
    val result : IamObjectUserinfo = apiInstance.iamApiControllerAddUserKeys()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerAddUserKeys")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerAddUserKeys")
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

<a id="iamApiControllerCheckUserPassword"></a>
# **iamApiControllerCheckUserPassword**
> IamObjectUserinfo iamApiControllerCheckUserPassword()

Api Controller Check User Password

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
try {
    val result : IamObjectUserinfo = apiInstance.iamApiControllerCheckUserPassword()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerCheckUserPassword")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerCheckUserPassword")
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

<a id="iamApiControllerDeleteLdap"></a>
# **iamApiControllerDeleteLdap**
> IamControllersResponse iamApiControllerDeleteLdap(id, iamObjectLdap)

Api Controller Delete Ldap

delete ldap

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectLdap : IamObjectLdap =  // IamObjectLdap | The details of the ldap
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeleteLdap(id, iamObjectLdap)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerDeleteLdap")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerDeleteLdap")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectLdap** | [**IamObjectLdap**](IamObjectLdap.md)| The details of the ldap | |

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

<a id="iamApiControllerDeleteUser"></a>
# **iamApiControllerDeleteUser**
> IamControllersResponse iamApiControllerDeleteUser(id, iamObjectUser)

Api Controller Delete User

delete user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectUser : IamObjectUser =  // IamObjectUser | The details of the user
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeleteUser(id, iamObjectUser)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerDeleteUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerDeleteUser")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectUser** | [**IamObjectUser**](IamObjectUser.md)| The details of the user | |

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

<a id="iamApiControllerExitImpersonateUser"></a>
# **iamApiControllerExitImpersonateUser**
> IamControllersResponse iamApiControllerExitImpersonateUser()

Api Controller Exit Impersonate User

clear impersonation info for current session

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerExitImpersonateUser()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerExitImpersonateUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerExitImpersonateUser")
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

<a id="iamApiControllerGetAccount"></a>
# **iamApiControllerGetAccount**
> IamControllersResponse iamApiControllerGetAccount(id)

Api Controller Get Account

get the details of the current account

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerGetAccount(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerGetAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerGetAccount")
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

<a id="iamApiControllerGetEmailAndPhone"></a>
# **iamApiControllerGetEmailAndPhone**
> IamControllersResponse iamApiControllerGetEmailAndPhone(username, organization)

Api Controller Get Email And Phone

get email and phone by username

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val username : kotlin.String = username_example // kotlin.String | The username of the user
val organization : kotlin.String = organization_example // kotlin.String | The organization of the user
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerGetEmailAndPhone(username, organization)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerGetEmailAndPhone")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerGetEmailAndPhone")
    e.printStackTrace()
}
```

### Parameters
| **username** | **kotlin.String**| The username of the user | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **organization** | **kotlin.String**| The organization of the user | |

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

<a id="iamApiControllerGetGlobalUsers"></a>
# **iamApiControllerGetGlobalUsers**
> kotlin.collections.List&lt;IamObjectUser&gt; iamApiControllerGetGlobalUsers()

Api Controller Get Global Users

get global users

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
try {
    val result : kotlin.collections.List<IamObjectUser> = apiInstance.iamApiControllerGetGlobalUsers()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerGetGlobalUsers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerGetGlobalUsers")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;IamObjectUser&gt;**](IamObjectUser.md)

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

<a id="iamApiControllerGetLdap"></a>
# **iamApiControllerGetLdap**
> IamObjectLdap iamApiControllerGetLdap(id)

Api Controller Get Ldap

get ldap

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val id : kotlin.String = id_example // kotlin.String | id
try {
    val result : IamObjectLdap = apiInstance.iamApiControllerGetLdap(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerGetLdap")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerGetLdap")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| id | |

### Return type

[**IamObjectLdap**](IamObjectLdap.md)

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

<a id="iamApiControllerGetLdaps"></a>
# **iamApiControllerGetLdaps**
> kotlin.collections.List&lt;IamObjectLdap&gt; iamApiControllerGetLdaps(owner)

Api Controller Get Ldaps

get ldaps

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val owner : kotlin.String = owner_example // kotlin.String | owner
try {
    val result : kotlin.collections.List<IamObjectLdap> = apiInstance.iamApiControllerGetLdaps(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerGetLdaps")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerGetLdaps")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| owner | [optional] |

### Return type

[**kotlin.collections.List&lt;IamObjectLdap&gt;**](IamObjectLdap.md)

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

<a id="iamApiControllerGetLdapser"></a>
# **iamApiControllerGetLdapser**
> IamControllersLdapResp iamApiControllerGetLdapser()

Api Controller Get Ldapser

get ldap users

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
try {
    val result : IamControllersLdapResp = apiInstance.iamApiControllerGetLdapser()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerGetLdapser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerGetLdapser")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**IamControllersLdapResp**](IamControllersLdapResp.md)

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

<a id="iamApiControllerGetSortedUsers"></a>
# **iamApiControllerGetSortedUsers**
> kotlin.collections.List&lt;IamObjectUser&gt; iamApiControllerGetSortedUsers(owner, sorter, limit)

Api Controller Get Sorted Users

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of users
val sorter : kotlin.String = sorter_example // kotlin.String | The DB column name to sort by, e.g., created_time
val limit : kotlin.String = limit_example // kotlin.String | The count of users to return, e.g., 25
try {
    val result : kotlin.collections.List<IamObjectUser> = apiInstance.iamApiControllerGetSortedUsers(owner, sorter, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerGetSortedUsers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerGetSortedUsers")
    e.printStackTrace()
}
```

### Parameters
| **owner** | **kotlin.String**| The owner of users | |
| **sorter** | **kotlin.String**| The DB column name to sort by, e.g., created_time | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.String**| The count of users to return, e.g., 25 | |

### Return type

[**kotlin.collections.List&lt;IamObjectUser&gt;**](IamObjectUser.md)

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

<a id="iamApiControllerGetUser"></a>
# **iamApiControllerGetUser**
> IamObjectUser iamApiControllerGetUser(id, owner, email, phone, userId)

Api Controller Get User

get user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the user
val owner : kotlin.String = owner_example // kotlin.String | The owner of the user
val email : kotlin.String = email_example // kotlin.String | The email of the user
val phone : kotlin.String = phone_example // kotlin.String | The phone of the user
val userId : kotlin.String = userId_example // kotlin.String | The userId of the user
try {
    val result : IamObjectUser = apiInstance.iamApiControllerGetUser(id, owner, email, phone, userId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerGetUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerGetUser")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the user | |
| **owner** | **kotlin.String**| The owner of the user | [optional] |
| **email** | **kotlin.String**| The email of the user | [optional] |
| **phone** | **kotlin.String**| The phone of the user | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **userId** | **kotlin.String**| The userId of the user | [optional] |

### Return type

[**IamObjectUser**](IamObjectUser.md)

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

<a id="iamApiControllerGetUserCount"></a>
# **iamApiControllerGetUserCount**
> kotlin.Any iamApiControllerGetUserCount(id, owner, isOnline)

Api Controller Get User Count

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val owner : kotlin.String = owner_example // kotlin.String | The owner of users
val isOnline : kotlin.String = isOnline_example // kotlin.String | The filter for query, 1 for online, 0 for offline, empty string for all users
try {
    val result : kotlin.Any = apiInstance.iamApiControllerGetUserCount(id, owner, isOnline)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerGetUserCount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerGetUserCount")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| **owner** | **kotlin.String**| The owner of users | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **isOnline** | **kotlin.String**| The filter for query, 1 for online, 0 for offline, empty string for all users | |

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

<a id="iamApiControllerGetUsers"></a>
# **iamApiControllerGetUsers**
> kotlin.collections.List&lt;IamObjectUser&gt; iamApiControllerGetUsers(owner)

Api Controller Get Users

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of users
try {
    val result : kotlin.collections.List<IamObjectUser> = apiInstance.iamApiControllerGetUsers(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerGetUsers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerGetUsers")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of users | |

### Return type

[**kotlin.collections.List&lt;IamObjectUser&gt;**](IamObjectUser.md)

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

<a id="iamApiControllerImpersonateUser"></a>
# **iamApiControllerImpersonateUser**
> IamControllersResponse iamApiControllerImpersonateUser(username)

Api Controller Impersonate User

set impersonation user for current admin session

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val username : kotlin.String = username_example // kotlin.String | The username to impersonate (owner/name)
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerImpersonateUser(username)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerImpersonateUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerImpersonateUser")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **username** | **kotlin.String**| The username to impersonate (owner/name) | |

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

<a id="iamApiControllerResetEmailOrPhone"></a>
# **iamApiControllerResetEmailOrPhone**
> IamObjectUserinfo iamApiControllerResetEmailOrPhone()

Api Controller Reset Email Or Phone

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
try {
    val result : IamObjectUserinfo = apiInstance.iamApiControllerResetEmailOrPhone()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerResetEmailOrPhone")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerResetEmailOrPhone")
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

<a id="iamApiControllerSetPassword"></a>
# **iamApiControllerSetPassword**
> IamControllersResponse iamApiControllerSetPassword(userOwner, userName, oldPassword, newPassword)

Api Controller Set Password

set password

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val userOwner : kotlin.String = userOwner_example // kotlin.String | The owner of the user
val userName : kotlin.String = userName_example // kotlin.String | The name of the user
val oldPassword : kotlin.String = oldPassword_example // kotlin.String | The old password of the user
val newPassword : kotlin.String = newPassword_example // kotlin.String | The new password of the user
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerSetPassword(userOwner, userName, oldPassword, newPassword)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerSetPassword")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerSetPassword")
    e.printStackTrace()
}
```

### Parameters
| **userOwner** | **kotlin.String**| The owner of the user | |
| **userName** | **kotlin.String**| The name of the user | |
| **oldPassword** | **kotlin.String**| The old password of the user | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **newPassword** | **kotlin.String**| The new password of the user | |

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

<a id="iamApiControllerSyncLdapUsers"></a>
# **iamApiControllerSyncLdapUsers**
> IamControllersLdapSyncResp iamApiControllerSyncLdapUsers(id)

Api Controller Sync Ldap Users

sync ldap users

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val id : kotlin.String = id_example // kotlin.String | id
try {
    val result : IamControllersLdapSyncResp = apiInstance.iamApiControllerSyncLdapUsers(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerSyncLdapUsers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerSyncLdapUsers")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| id | |

### Return type

[**IamControllersLdapSyncResp**](IamControllersLdapSyncResp.md)

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

<a id="iamApiControllerUpdateLdap"></a>
# **iamApiControllerUpdateLdap**
> IamControllersResponse iamApiControllerUpdateLdap(id, iamObjectLdap)

Api Controller Update Ldap

update ldap

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectLdap : IamObjectLdap =  // IamObjectLdap | The details of the ldap
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdateLdap(id, iamObjectLdap)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerUpdateLdap")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerUpdateLdap")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectLdap** | [**IamObjectLdap**](IamObjectLdap.md)| The details of the ldap | |

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

<a id="iamApiControllerUpdateUser"></a>
# **iamApiControllerUpdateUser**
> IamControllersResponse iamApiControllerUpdateUser(id, iamObjectUser, userId, owner)

Api Controller Update User

update user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the user
val iamObjectUser : IamObjectUser =  // IamObjectUser | The details of the user
val userId : kotlin.String = userId_example // kotlin.String | The userId (UUID) of the user
val owner : kotlin.String = owner_example // kotlin.String | The owner of the user (required when using userId)
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdateUser(id, iamObjectUser, userId, owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerUpdateUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerUpdateUser")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the user | |
| **iamObjectUser** | [**IamObjectUser**](IamObjectUser.md)| The details of the user | |
| **userId** | **kotlin.String**| The userId (UUID) of the user | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of the user (required when using userId) | [optional] |

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

<a id="iamApiControllerUserInfo"></a>
# **iamApiControllerUserInfo**
> IamObjectUserinfo iamApiControllerUserInfo()

Api Controller User Info

return user information according to OIDC standards

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
try {
    val result : IamObjectUserinfo = apiInstance.iamApiControllerUserInfo()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerUserInfo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerUserInfo")
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

<a id="iamApiControllerUserInfo2"></a>
# **iamApiControllerUserInfo2**
> IamControllersLaravelResponse iamApiControllerUserInfo2()

Api Controller User Info2

return Laravel compatible user information according to OAuth 2.0

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
try {
    val result : IamControllersLaravelResponse = apiInstance.iamApiControllerUserInfo2()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerUserInfo2")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerUserInfo2")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**IamControllersLaravelResponse**](IamControllersLaravelResponse.md)

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

<a id="iamApiControllerVerifyIdentification"></a>
# **iamApiControllerVerifyIdentification**
> IamControllersResponse iamApiControllerVerifyIdentification(owner, name, provider)

Api Controller Verify Identification

verify user&#39;s real identity using ID Verification provider

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of the user (optional, defaults to logged-in user)
val name : kotlin.String = name_example // kotlin.String | The name of the user (optional, defaults to logged-in user)
val provider : kotlin.String = provider_example // kotlin.String | The name of the ID Verification provider (optional, auto-selected if not provided)
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerVerifyIdentification(owner, name, provider)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerVerifyIdentification")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerVerifyIdentification")
    e.printStackTrace()
}
```

### Parameters
| **owner** | **kotlin.String**| The owner of the user (optional, defaults to logged-in user) | [optional] |
| **name** | **kotlin.String**| The name of the user (optional, defaults to logged-in user) | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **provider** | **kotlin.String**| The name of the ID Verification provider (optional, auto-selected if not provided) | [optional] |

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

<a id="iamApiControllerWebAuthnSignupBegin"></a>
# **iamApiControllerWebAuthnSignupBegin**
> kotlin.Any iamApiControllerWebAuthnSignupBegin()

Api Controller Web Authn Signup Begin

WebAuthn Registration Flow 1st stage

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
try {
    val result : kotlin.Any = apiInstance.iamApiControllerWebAuthnSignupBegin()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerWebAuthnSignupBegin")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerWebAuthnSignupBegin")
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

<a id="iamApiControllerWebAuthnSignupFinish"></a>
# **iamApiControllerWebAuthnSignupFinish**
> IamControllersResponse iamApiControllerWebAuthnSignupFinish(body)

Api Controller Web Authn Signup Finish

WebAuthn Registration Flow 2nd stage

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
val body : kotlin.Any = Object // kotlin.Any | authenticator attestation Response
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerWebAuthnSignupFinish(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#iamApiControllerWebAuthnSignupFinish")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#iamApiControllerWebAuthnSignupFinish")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**| authenticator attestation Response | |

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

<a id="kmsGetCurrentUser"></a>
# **kmsGetCurrentUser**
> KmsGetCurrentUser200Response kmsGetCurrentUser()

Get the current authenticated user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsersApi()
try {
    val result : KmsGetCurrentUser200Response = apiInstance.kmsGetCurrentUser()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsersApi#kmsGetCurrentUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsersApi#kmsGetCurrentUser")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**KmsGetCurrentUser200Response**](KmsGetCurrentUser200Response.md)

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

