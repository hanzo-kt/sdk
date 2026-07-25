# DeploymentAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerGetK8sStatus**](DeploymentAPIApi.md#cloudApiControllerGetK8sStatus) | **GET** /v1/cloud/get-k8s-status | Api Controller Get K8s Status |
| [**nexusGetK8sStatus**](DeploymentAPIApi.md#nexusGetK8sStatus) | **GET** /v1/nexus/get-k8s-status | get K8s Status |


<a id="cloudApiControllerGetK8sStatus"></a>
# **cloudApiControllerGetK8sStatus**
> kotlin.Any cloudApiControllerGetK8sStatus()

Api Controller Get K8s Status

get kubernetes cluster status

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DeploymentAPIApi()
try {
    val result : kotlin.Any = apiInstance.cloudApiControllerGetK8sStatus()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeploymentAPIApi#cloudApiControllerGetK8sStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeploymentAPIApi#cloudApiControllerGetK8sStatus")
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

<a id="nexusGetK8sStatus"></a>
# **nexusGetK8sStatus**
> kotlin.Any nexusGetK8sStatus()

get K8s Status

Get Kubernetes cluster status

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DeploymentAPIApi()
try {
    val result : kotlin.Any = apiInstance.nexusGetK8sStatus()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeploymentAPIApi#nexusGetK8sStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeploymentAPIApi#nexusGetK8sStatus")
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

