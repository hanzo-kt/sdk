# UserInvitationsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoCreateUserInvitation**](UserInvitationsApi.md#autoCreateUserInvitation) | **POST** /v1/auto/user-invitations | Invite a user to a project |
| [**autoListUserInvitations**](UserInvitationsApi.md#autoListUserInvitations) | **GET** /v1/auto/user-invitations | List pending invitations |
| [**flowAcceptUserInvitation**](UserInvitationsApi.md#flowAcceptUserInvitation) | **POST** /v1/flow/user-invitations/{id}/accept | Accept an invitation |
| [**flowCreateUserInvitation**](UserInvitationsApi.md#flowCreateUserInvitation) | **POST** /v1/flow/user-invitations | Invite a user to a project |
| [**flowListUserInvitations**](UserInvitationsApi.md#flowListUserInvitations) | **GET** /v1/flow/user-invitations | List pending invitations |


<a id="autoCreateUserInvitation"></a>
# **autoCreateUserInvitation**
> kotlin.Any autoCreateUserInvitation(autoCreateUserInvitationRequest)

Invite a user to a project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UserInvitationsApi()
val autoCreateUserInvitationRequest : AutoCreateUserInvitationRequest =  // AutoCreateUserInvitationRequest | 
try {
    val result : kotlin.Any = apiInstance.autoCreateUserInvitation(autoCreateUserInvitationRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UserInvitationsApi#autoCreateUserInvitation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserInvitationsApi#autoCreateUserInvitation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoCreateUserInvitationRequest** | [**AutoCreateUserInvitationRequest**](AutoCreateUserInvitationRequest.md)|  | |

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

<a id="autoListUserInvitations"></a>
# **autoListUserInvitations**
> kotlin.Any autoListUserInvitations()

List pending invitations

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UserInvitationsApi()
try {
    val result : kotlin.Any = apiInstance.autoListUserInvitations()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UserInvitationsApi#autoListUserInvitations")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserInvitationsApi#autoListUserInvitations")
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

<a id="flowAcceptUserInvitation"></a>
# **flowAcceptUserInvitation**
> kotlin.Any flowAcceptUserInvitation(id)

Accept an invitation

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UserInvitationsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.flowAcceptUserInvitation(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UserInvitationsApi#flowAcceptUserInvitation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserInvitationsApi#flowAcceptUserInvitation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

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

<a id="flowCreateUserInvitation"></a>
# **flowCreateUserInvitation**
> kotlin.Any flowCreateUserInvitation(autoCreateUserInvitationRequest)

Invite a user to a project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UserInvitationsApi()
val autoCreateUserInvitationRequest : AutoCreateUserInvitationRequest =  // AutoCreateUserInvitationRequest | 
try {
    val result : kotlin.Any = apiInstance.flowCreateUserInvitation(autoCreateUserInvitationRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UserInvitationsApi#flowCreateUserInvitation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserInvitationsApi#flowCreateUserInvitation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoCreateUserInvitationRequest** | [**AutoCreateUserInvitationRequest**](AutoCreateUserInvitationRequest.md)|  | |

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

<a id="flowListUserInvitations"></a>
# **flowListUserInvitations**
> kotlin.Any flowListUserInvitations()

List pending invitations

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UserInvitationsApi()
try {
    val result : kotlin.Any = apiInstance.flowListUserInvitations()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UserInvitationsApi#flowListUserInvitations")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserInvitationsApi#flowListUserInvitations")
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

