# DeploysApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**authorsRecordDeploy**](DeploysApi.md#authorsRecordDeploy) | **POST** /v1/authors/deploys/record | Record a deploy |


<a id="authorsRecordDeploy"></a>
# **authorsRecordDeploy**
> AuthorsRecordDeploy200Response authorsRecordDeploy(authorsRecordDeployRequest)

Record a deploy

Records a deploy-attribution edge for the caller (the DEPLOYING org). When &#x60;repoUrl&#x60; matches a verified author repo, the edge is recorded (idempotent per repo+project+org) and becomes eligible for royalty. A deploy of a repo that is not a verified author repo is NOT an error — it returns &#x60;recorded: false&#x60; so the deploy path can fire this unconditionally. A self-deploy is recorded (provenance) but excluded from accrual. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DeploysApi()
val authorsRecordDeployRequest : AuthorsRecordDeployRequest =  // AuthorsRecordDeployRequest | 
try {
    val result : AuthorsRecordDeploy200Response = apiInstance.authorsRecordDeploy(authorsRecordDeployRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeploysApi#authorsRecordDeploy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeploysApi#authorsRecordDeploy")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **authorsRecordDeployRequest** | [**AuthorsRecordDeployRequest**](AuthorsRecordDeployRequest.md)|  | |

### Return type

[**AuthorsRecordDeploy200Response**](AuthorsRecordDeploy200Response.md)

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

