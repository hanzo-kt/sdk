# RulesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**securitySecurityHealth**](RulesApi.md#securitySecurityHealth) | **GET** /v1/security/health | Health check |
| [**securitySecurityListRules**](RulesApi.md#securitySecurityListRules) | **GET** /v1/security/rules | List the detection ruleset |


<a id="securitySecurityHealth"></a>
# **securitySecurityHealth**
> SecuritySecurityHealth200Response securitySecurityHealth()

Health check

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RulesApi()
try {
    val result : SecuritySecurityHealth200Response = apiInstance.securitySecurityHealth()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RulesApi#securitySecurityHealth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RulesApi#securitySecurityHealth")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**SecuritySecurityHealth200Response**](SecuritySecurityHealth200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="securitySecurityListRules"></a>
# **securitySecurityListRules**
> SecuritySecurityListRules200Response securitySecurityListRules()

List the detection ruleset

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RulesApi()
try {
    val result : SecuritySecurityListRules200Response = apiInstance.securitySecurityListRules()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RulesApi#securitySecurityListRules")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RulesApi#securitySecurityListRules")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**SecuritySecurityListRules200Response**](SecuritySecurityListRules200Response.md)

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

