# SCIMApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**didScimCreateUser**](SCIMApi.md#didScimCreateUser) | **POST** /v1/did/scim/v2/Users | SCIM create user |
| [**didScimListUsers**](SCIMApi.md#didScimListUsers) | **GET** /v1/did/scim/v2/Users | SCIM list users |


<a id="didScimCreateUser"></a>
# **didScimCreateUser**
> didScimCreateUser(body)

SCIM create user

Provision a user via SCIM 2.0.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SCIMApi()
val body : kotlin.Any = Object // kotlin.Any | 
try {
    apiInstance.didScimCreateUser(body)
} catch (e: ClientException) {
    println("4xx response calling SCIMApi#didScimCreateUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SCIMApi#didScimCreateUser")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

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

 - **Content-Type**: application/scim+json
 - **Accept**: Not defined

<a id="didScimListUsers"></a>
# **didScimListUsers**
> kotlin.Any didScimListUsers(filter, count, startIndex)

SCIM list users

SCIM 2.0 compliant user listing for external IdP provisioning.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SCIMApi()
val filter : kotlin.String = filter_example // kotlin.String | SCIM filter expression
val count : kotlin.Int = 56 // kotlin.Int | 
val startIndex : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : kotlin.Any = apiInstance.didScimListUsers(filter, count, startIndex)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SCIMApi#didScimListUsers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SCIMApi#didScimListUsers")
    e.printStackTrace()
}
```

### Parameters
| **filter** | **kotlin.String**| SCIM filter expression | [optional] |
| **count** | **kotlin.Int**|  | [optional] [default to 100] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **startIndex** | **kotlin.Int**|  | [optional] [default to 1] |

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
 - **Accept**: application/scim+json

