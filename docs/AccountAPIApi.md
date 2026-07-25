# AccountAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerGetAccount**](AccountAPIApi.md#cloudApiControllerGetAccount) | **GET** /v1/cloud/get-account | Api Controller Get Account |
| [**cloudApiControllerSignin**](AccountAPIApi.md#cloudApiControllerSignin) | **POST** /v1/cloud/signin | Api Controller Signin |
| [**cloudApiControllerSignout**](AccountAPIApi.md#cloudApiControllerSignout) | **POST** /v1/cloud/signout | Api Controller Signout |
| [**nexusGetAccount**](AccountAPIApi.md#nexusGetAccount) | **GET** /v1/nexus/get-account | get Account |
| [**nexusSignin**](AccountAPIApi.md#nexusSignin) | **POST** /v1/nexus/signin | signin |
| [**nexusSignout**](AccountAPIApi.md#nexusSignout) | **POST** /v1/nexus/signout | signout |


<a id="cloudApiControllerGetAccount"></a>
# **cloudApiControllerGetAccount**
> kotlin.Any cloudApiControllerGetAccount()

Api Controller Get Account

get account

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AccountAPIApi()
try {
    val result : kotlin.Any = apiInstance.cloudApiControllerGetAccount()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountAPIApi#cloudApiControllerGetAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountAPIApi#cloudApiControllerGetAccount")
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

<a id="cloudApiControllerSignin"></a>
# **cloudApiControllerSignin**
> kotlin.Any cloudApiControllerSignin(code, state)

Api Controller Signin

sign in

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AccountAPIApi()
val code : kotlin.String = code_example // kotlin.String | code of account
val state : kotlin.String = state_example // kotlin.String | state of account
try {
    val result : kotlin.Any = apiInstance.cloudApiControllerSignin(code, state)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountAPIApi#cloudApiControllerSignin")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountAPIApi#cloudApiControllerSignin")
    e.printStackTrace()
}
```

### Parameters
| **code** | **kotlin.String**| code of account | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **state** | **kotlin.String**| state of account | |

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

<a id="cloudApiControllerSignout"></a>
# **cloudApiControllerSignout**
> CloudControllersResponse cloudApiControllerSignout()

Api Controller Signout

sign out

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AccountAPIApi()
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerSignout()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountAPIApi#cloudApiControllerSignout")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountAPIApi#cloudApiControllerSignout")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="nexusGetAccount"></a>
# **nexusGetAccount**
> kotlin.Any nexusGetAccount()

get Account

Get the current account

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AccountAPIApi()
try {
    val result : kotlin.Any = apiInstance.nexusGetAccount()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountAPIApi#nexusGetAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountAPIApi#nexusGetAccount")
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

<a id="nexusSignin"></a>
# **nexusSignin**
> kotlin.Any nexusSignin(code, state)

signin

Sign in

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AccountAPIApi()
val code : kotlin.String = code_example // kotlin.String | Authorization code
val state : kotlin.String = state_example // kotlin.String | OAuth state
try {
    val result : kotlin.Any = apiInstance.nexusSignin(code, state)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountAPIApi#nexusSignin")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountAPIApi#nexusSignin")
    e.printStackTrace()
}
```

### Parameters
| **code** | **kotlin.String**| Authorization code | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **state** | **kotlin.String**| OAuth state | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="nexusSignout"></a>
# **nexusSignout**
> NexusResponse nexusSignout()

signout

Sign out

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AccountAPIApi()
try {
    val result : NexusResponse = apiInstance.nexusSignout()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountAPIApi#nexusSignout")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountAPIApi#nexusSignout")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**NexusResponse**](NexusResponse.md)

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

