# EnforcementApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**authzAuthzCheck**](EnforcementApi.md#authzAuthzCheck) | **POST** /v1/authz/check | Check a permission |


<a id="authzAuthzCheck"></a>
# **authzAuthzCheck**
> AuthzCheckResponse authzAuthzCheck(authzEnforceRequest)

Check a permission

Evaluates whether subject &#x60;sub&#x60; may perform action &#x60;act&#x60; on object &#x60;obj&#x60; under the calling org&#39;s policy set. The org is selected by the gateway-minted &#x60;X-Org-Id&#x60; header; an unauthenticated request (no org) is rejected. All three fields are required. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EnforcementApi()
val authzEnforceRequest : AuthzEnforceRequest =  // AuthzEnforceRequest | 
try {
    val result : AuthzCheckResponse = apiInstance.authzAuthzCheck(authzEnforceRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EnforcementApi#authzAuthzCheck")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EnforcementApi#authzAuthzCheck")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **authzEnforceRequest** | [**AuthzEnforceRequest**](AuthzEnforceRequest.md)|  | |

### Return type

[**AuthzCheckResponse**](AuthzCheckResponse.md)

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

