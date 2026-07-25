# IdentityResolutionApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**didLinkIdentity**](IdentityResolutionApi.md#didLinkIdentity) | **POST** /v1/did/profiles/{profile_id}/identities | Link an external identity |
| [**didListLinkedIdentities**](IdentityResolutionApi.md#didListLinkedIdentities) | **GET** /v1/did/profiles/{profile_id}/identities | List linked identities |
| [**didResolveIdentity**](IdentityResolutionApi.md#didResolveIdentity) | **GET** /v1/did/resolve | Resolve identity across providers |
| [**didUnlinkIdentity**](IdentityResolutionApi.md#didUnlinkIdentity) | **DELETE** /v1/did/profiles/{profile_id}/identities/{provider} | Unlink an external identity |


<a id="didLinkIdentity"></a>
# **didLinkIdentity**
> DidLinkedIdentity didLinkIdentity(profileId, didLinkIdentityRequest)

Link an external identity

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IdentityResolutionApi()
val profileId : kotlin.String = profileId_example // kotlin.String | 
val didLinkIdentityRequest : DidLinkIdentityRequest =  // DidLinkIdentityRequest | 
try {
    val result : DidLinkedIdentity = apiInstance.didLinkIdentity(profileId, didLinkIdentityRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IdentityResolutionApi#didLinkIdentity")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IdentityResolutionApi#didLinkIdentity")
    e.printStackTrace()
}
```

### Parameters
| **profileId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **didLinkIdentityRequest** | [**DidLinkIdentityRequest**](DidLinkIdentityRequest.md)|  | |

### Return type

[**DidLinkedIdentity**](DidLinkedIdentity.md)

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

<a id="didListLinkedIdentities"></a>
# **didListLinkedIdentities**
> DidListLinkedIdentities200Response didListLinkedIdentities(profileId)

List linked identities

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IdentityResolutionApi()
val profileId : kotlin.String = profileId_example // kotlin.String | 
try {
    val result : DidListLinkedIdentities200Response = apiInstance.didListLinkedIdentities(profileId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IdentityResolutionApi#didListLinkedIdentities")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IdentityResolutionApi#didListLinkedIdentities")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **profileId** | **kotlin.String**|  | |

### Return type

[**DidListLinkedIdentities200Response**](DidListLinkedIdentities200Response.md)

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

<a id="didResolveIdentity"></a>
# **didResolveIdentity**
> DidProfile didResolveIdentity(provider, externalId)

Resolve identity across providers

Find a Hanzo profile by external provider identity.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IdentityResolutionApi()
val provider : kotlin.String = provider_example // kotlin.String | 
val externalId : kotlin.String = externalId_example // kotlin.String | 
try {
    val result : DidProfile = apiInstance.didResolveIdentity(provider, externalId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IdentityResolutionApi#didResolveIdentity")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IdentityResolutionApi#didResolveIdentity")
    e.printStackTrace()
}
```

### Parameters
| **provider** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **externalId** | **kotlin.String**|  | |

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

<a id="didUnlinkIdentity"></a>
# **didUnlinkIdentity**
> didUnlinkIdentity(profileId, provider)

Unlink an external identity

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IdentityResolutionApi()
val profileId : kotlin.String = profileId_example // kotlin.String | 
val provider : kotlin.String = provider_example // kotlin.String | 
try {
    apiInstance.didUnlinkIdentity(profileId, provider)
} catch (e: ClientException) {
    println("4xx response calling IdentityResolutionApi#didUnlinkIdentity")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IdentityResolutionApi#didUnlinkIdentity")
    e.printStackTrace()
}
```

### Parameters
| **profileId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **provider** | **kotlin.String**|  | |

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
 - **Accept**: Not defined

