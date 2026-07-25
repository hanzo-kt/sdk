# ProfilesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**didGetProfile**](ProfilesApi.md#didGetProfile) | **GET** /v1/did/profiles/{profile_id} | Get a profile |
| [**didGetProfileHistory**](ProfilesApi.md#didGetProfileHistory) | **GET** /v1/did/profiles/{profile_id}/history | Get profile change history |
| [**didListProfiles**](ProfilesApi.md#didListProfiles) | **GET** /v1/did/profiles | List profiles |
| [**didUpdateProfile**](ProfilesApi.md#didUpdateProfile) | **PUT** /v1/did/profiles/{profile_id} | Update a profile |


<a id="didGetProfile"></a>
# **didGetProfile**
> DidProfile didGetProfile(profileId)

Get a profile

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProfilesApi()
val profileId : kotlin.String = profileId_example // kotlin.String | 
try {
    val result : DidProfile = apiInstance.didGetProfile(profileId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProfilesApi#didGetProfile")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProfilesApi#didGetProfile")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **profileId** | **kotlin.String**|  | |

### Return type

[**DidProfile**](DidProfile.md)

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

<a id="didGetProfileHistory"></a>
# **didGetProfileHistory**
> DidGetProfileHistory200Response didGetProfileHistory(profileId, limit)

Get profile change history

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProfilesApi()
val profileId : kotlin.String = profileId_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : DidGetProfileHistory200Response = apiInstance.didGetProfileHistory(profileId, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProfilesApi#didGetProfileHistory")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProfilesApi#didGetProfileHistory")
    e.printStackTrace()
}
```

### Parameters
| **profileId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] [default to 50] |

### Return type

[**DidGetProfileHistory200Response**](DidGetProfileHistory200Response.md)

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

<a id="didListProfiles"></a>
# **didListProfiles**
> DidListProfiles200Response didListProfiles(organization, type, team, status, search, limit, cursor)

List profiles

List all profiles in an organization, with optional filtering.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProfilesApi()
val organization : kotlin.String = organization_example // kotlin.String | Organization to list profiles for
val type : kotlin.String = type_example // kotlin.String | Filter by profile type
val team : kotlin.String = team_example // kotlin.String | Filter by team membership
val status : kotlin.String = status_example // kotlin.String | Filter by status
val search : kotlin.String = search_example // kotlin.String | Search by name or email
val limit : kotlin.Int = 56 // kotlin.Int | 
val cursor : kotlin.String = cursor_example // kotlin.String | 
try {
    val result : DidListProfiles200Response = apiInstance.didListProfiles(organization, type, team, status, search, limit, cursor)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProfilesApi#didListProfiles")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProfilesApi#didListProfiles")
    e.printStackTrace()
}
```

### Parameters
| **organization** | **kotlin.String**| Organization to list profiles for | |
| **type** | **kotlin.String**| Filter by profile type | [optional] [enum: user, service_account, bot] |
| **team** | **kotlin.String**| Filter by team membership | [optional] |
| **status** | **kotlin.String**| Filter by status | [optional] [enum: active, suspended, deactivated] |
| **search** | **kotlin.String**| Search by name or email | [optional] |
| **limit** | **kotlin.Int**|  | [optional] [default to 50] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cursor** | **kotlin.String**|  | [optional] |

### Return type

[**DidListProfiles200Response**](DidListProfiles200Response.md)

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

<a id="didUpdateProfile"></a>
# **didUpdateProfile**
> DidProfile didUpdateProfile(profileId, didUpdateProfileRequest)

Update a profile

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProfilesApi()
val profileId : kotlin.String = profileId_example // kotlin.String | 
val didUpdateProfileRequest : DidUpdateProfileRequest =  // DidUpdateProfileRequest | 
try {
    val result : DidProfile = apiInstance.didUpdateProfile(profileId, didUpdateProfileRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProfilesApi#didUpdateProfile")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProfilesApi#didUpdateProfile")
    e.printStackTrace()
}
```

### Parameters
| **profileId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **didUpdateProfileRequest** | [**DidUpdateProfileRequest**](DidUpdateProfileRequest.md)|  | |

### Return type

[**DidProfile**](DidProfile.md)

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

