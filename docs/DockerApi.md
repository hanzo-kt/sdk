# DockerApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformDockerGetConfig**](DockerApi.md#platformDockerGetConfig) | **GET** /v1/platform/docker/getConfig | Get Docker inspect for a container |
| [**platformDockerGetContainers**](DockerApi.md#platformDockerGetContainers) | **GET** /v1/platform/docker/getContainers | List all Docker containers |
| [**platformDockerRestartContainer**](DockerApi.md#platformDockerRestartContainer) | **POST** /v1/platform/docker/restartContainer | Restart a container by ID |


<a id="platformDockerGetConfig"></a>
# **platformDockerGetConfig**
> PlatformTRPCResult platformDockerGetConfig(input)

Get Docker inspect for a container

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DockerApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformDockerGetConfig(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DockerApi#platformDockerGetConfig")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DockerApi#platformDockerGetConfig")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **input** | **kotlin.String**| URL-encoded JSON input for tRPC queries | [optional] |

### Return type

[**PlatformTRPCResult**](PlatformTRPCResult.md)

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

<a id="platformDockerGetContainers"></a>
# **platformDockerGetContainers**
> PlatformTRPCResult platformDockerGetContainers(input)

List all Docker containers

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DockerApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformDockerGetContainers(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DockerApi#platformDockerGetContainers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DockerApi#platformDockerGetContainers")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **input** | **kotlin.String**| URL-encoded JSON input for tRPC queries | [optional] |

### Return type

[**PlatformTRPCResult**](PlatformTRPCResult.md)

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

<a id="platformDockerRestartContainer"></a>
# **platformDockerRestartContainer**
> PlatformTRPCResult platformDockerRestartContainer(platformDockerRestartContainerRequest)

Restart a container by ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DockerApi()
val platformDockerRestartContainerRequest : PlatformDockerRestartContainerRequest =  // PlatformDockerRestartContainerRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformDockerRestartContainer(platformDockerRestartContainerRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DockerApi#platformDockerRestartContainer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DockerApi#platformDockerRestartContainer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformDockerRestartContainerRequest** | [**PlatformDockerRestartContainerRequest**](PlatformDockerRestartContainerRequest.md)|  | |

### Return type

[**PlatformTRPCResult**](PlatformTRPCResult.md)

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

