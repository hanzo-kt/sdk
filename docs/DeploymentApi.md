# DeploymentApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformDeploymentAll**](DeploymentApi.md#platformDeploymentAll) | **GET** /v1/platform/deployment/all | List deployments for an application |
| [**platformDeploymentAllByCompose**](DeploymentApi.md#platformDeploymentAllByCompose) | **GET** /v1/platform/deployment/allByCompose | List deployments for a compose service |
| [**platformDeploymentAllByServer**](DeploymentApi.md#platformDeploymentAllByServer) | **GET** /v1/platform/deployment/allByServer | List deployments on a server |
| [**platformDeploymentAllByType**](DeploymentApi.md#platformDeploymentAllByType) | **GET** /v1/platform/deployment/allByType | List deployments by resource type and ID |
| [**platformDeploymentKillProcess**](DeploymentApi.md#platformDeploymentKillProcess) | **POST** /v1/platform/deployment/killProcess | Kill a running deployment process |
| [**platformWebhookDeployApplication**](DeploymentApi.md#platformWebhookDeployApplication) | **POST** /v1/platform/deploy/{refreshToken} | Webhook to trigger application deployment |
| [**platformWebhookDeployCompose**](DeploymentApi.md#platformWebhookDeployCompose) | **POST** /v1/platform/deploy/compose/{refreshToken} | Webhook to trigger compose deployment |
| [**platformWebhookGithub**](DeploymentApi.md#platformWebhookGithub) | **POST** /v1/platform/deploy/github | GitHub webhook receiver for auto-deploy |


<a id="platformDeploymentAll"></a>
# **platformDeploymentAll**
> PlatformTRPCResult platformDeploymentAll(input)

List deployments for an application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DeploymentApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformDeploymentAll(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeploymentApi#platformDeploymentAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeploymentApi#platformDeploymentAll")
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

<a id="platformDeploymentAllByCompose"></a>
# **platformDeploymentAllByCompose**
> PlatformTRPCResult platformDeploymentAllByCompose(input)

List deployments for a compose service

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DeploymentApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformDeploymentAllByCompose(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeploymentApi#platformDeploymentAllByCompose")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeploymentApi#platformDeploymentAllByCompose")
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

<a id="platformDeploymentAllByServer"></a>
# **platformDeploymentAllByServer**
> PlatformTRPCResult platformDeploymentAllByServer(input)

List deployments on a server

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DeploymentApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformDeploymentAllByServer(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeploymentApi#platformDeploymentAllByServer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeploymentApi#platformDeploymentAllByServer")
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

<a id="platformDeploymentAllByType"></a>
# **platformDeploymentAllByType**
> PlatformTRPCResult platformDeploymentAllByType(input)

List deployments by resource type and ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DeploymentApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformDeploymentAllByType(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeploymentApi#platformDeploymentAllByType")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeploymentApi#platformDeploymentAllByType")
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

<a id="platformDeploymentKillProcess"></a>
# **platformDeploymentKillProcess**
> PlatformTRPCResult platformDeploymentKillProcess(platformDeploymentKillProcessRequest)

Kill a running deployment process

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DeploymentApi()
val platformDeploymentKillProcessRequest : PlatformDeploymentKillProcessRequest =  // PlatformDeploymentKillProcessRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformDeploymentKillProcess(platformDeploymentKillProcessRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeploymentApi#platformDeploymentKillProcess")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeploymentApi#platformDeploymentKillProcess")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformDeploymentKillProcessRequest** | [**PlatformDeploymentKillProcessRequest**](PlatformDeploymentKillProcessRequest.md)|  | |

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

<a id="platformWebhookDeployApplication"></a>
# **platformWebhookDeployApplication**
> platformWebhookDeployApplication(refreshToken)

Webhook to trigger application deployment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DeploymentApi()
val refreshToken : kotlin.String = refreshToken_example // kotlin.String | 
try {
    apiInstance.platformWebhookDeployApplication(refreshToken)
} catch (e: ClientException) {
    println("4xx response calling DeploymentApi#platformWebhookDeployApplication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeploymentApi#platformWebhookDeployApplication")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **refreshToken** | **kotlin.String**|  | |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="platformWebhookDeployCompose"></a>
# **platformWebhookDeployCompose**
> platformWebhookDeployCompose(refreshToken)

Webhook to trigger compose deployment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DeploymentApi()
val refreshToken : kotlin.String = refreshToken_example // kotlin.String | 
try {
    apiInstance.platformWebhookDeployCompose(refreshToken)
} catch (e: ClientException) {
    println("4xx response calling DeploymentApi#platformWebhookDeployCompose")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeploymentApi#platformWebhookDeployCompose")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **refreshToken** | **kotlin.String**|  | |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="platformWebhookGithub"></a>
# **platformWebhookGithub**
> platformWebhookGithub(body)

GitHub webhook receiver for auto-deploy

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DeploymentApi()
val body : kotlin.Any = Object // kotlin.Any | 
try {
    apiInstance.platformWebhookGithub(body)
} catch (e: ClientException) {
    println("4xx response calling DeploymentApi#platformWebhookGithub")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeploymentApi#platformWebhookGithub")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | [optional] |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

