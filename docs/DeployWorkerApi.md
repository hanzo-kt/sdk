# DeployWorkerApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformDeployWorkerCancelDeployment**](DeployWorkerApi.md#platformDeployWorkerCancelDeployment) | **POST** /v1/platform/cancel-deployment | Cancel an in-progress worker deployment |
| [**platformDeployWorkerDeploy**](DeployWorkerApi.md#platformDeployWorkerDeploy) | **POST** /v1/platform/deploy | Submit deployment job to worker queue |


<a id="platformDeployWorkerCancelDeployment"></a>
# **platformDeployWorkerCancelDeployment**
> PlatformDeployWorkerCancelDeployment200Response platformDeployWorkerCancelDeployment(platformCancelDeploymentJob)

Cancel an in-progress worker deployment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DeployWorkerApi()
val platformCancelDeploymentJob : PlatformCancelDeploymentJob =  // PlatformCancelDeploymentJob | 
try {
    val result : PlatformDeployWorkerCancelDeployment200Response = apiInstance.platformDeployWorkerCancelDeployment(platformCancelDeploymentJob)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeployWorkerApi#platformDeployWorkerCancelDeployment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeployWorkerApi#platformDeployWorkerCancelDeployment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformCancelDeploymentJob** | [**PlatformCancelDeploymentJob**](PlatformCancelDeploymentJob.md)|  | |

### Return type

[**PlatformDeployWorkerCancelDeployment200Response**](PlatformDeployWorkerCancelDeployment200Response.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.apiKey["X-API-Key"] = ""
    ApiClient.apiKeyPrefix["X-API-Key"] = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="platformDeployWorkerDeploy"></a>
# **platformDeployWorkerDeploy**
> PlatformDeployWorkerDeploy200Response platformDeployWorkerDeploy(platformDeployJob)

Submit deployment job to worker queue

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DeployWorkerApi()
val platformDeployJob : PlatformDeployJob =  // PlatformDeployJob | 
try {
    val result : PlatformDeployWorkerDeploy200Response = apiInstance.platformDeployWorkerDeploy(platformDeployJob)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeployWorkerApi#platformDeployWorkerDeploy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeployWorkerApi#platformDeployWorkerDeploy")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformDeployJob** | [**PlatformDeployJob**](PlatformDeployJob.md)|  | |

### Return type

[**PlatformDeployWorkerDeploy200Response**](PlatformDeployWorkerDeploy200Response.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.apiKey["X-API-Key"] = ""
    ApiClient.apiKeyPrefix["X-API-Key"] = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

