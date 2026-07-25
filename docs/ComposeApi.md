# ComposeApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformComposeCancelDeployment**](ComposeApi.md#platformComposeCancelDeployment) | **POST** /v1/platform/compose/cancelDeployment | Cancel in-progress compose deployment |
| [**platformComposeCreate**](ComposeApi.md#platformComposeCreate) | **POST** /v1/platform/compose/create | Create a Docker Compose service |
| [**platformComposeDelete**](ComposeApi.md#platformComposeDelete) | **POST** /v1/platform/compose/delete | Delete a compose service |
| [**platformComposeDeploy**](ComposeApi.md#platformComposeDeploy) | **POST** /v1/platform/compose/deploy | Deploy a compose service |
| [**platformComposeDeployTemplate**](ComposeApi.md#platformComposeDeployTemplate) | **POST** /v1/platform/compose/deployTemplate | Deploy a one-click template |
| [**platformComposeDisconnectGitProvider**](ComposeApi.md#platformComposeDisconnectGitProvider) | **POST** /v1/platform/compose/disconnectGitProvider | Disconnect git providers from compose |
| [**platformComposeGetConvertedCompose**](ComposeApi.md#platformComposeGetConvertedCompose) | **GET** /v1/platform/compose/getConvertedCompose | Get final compose YAML with domains injected |
| [**platformComposeGetDefaultCommand**](ComposeApi.md#platformComposeGetDefaultCommand) | **GET** /v1/platform/compose/getDefaultCommand | Get the docker compose command |
| [**platformComposeGetTags**](ComposeApi.md#platformComposeGetTags) | **GET** /v1/platform/compose/getTags | Get unique tags from all templates |
| [**platformComposeLoadServices**](ComposeApi.md#platformComposeLoadServices) | **GET** /v1/platform/compose/loadServices | List running services within a compose stack |
| [**platformComposeMove**](ComposeApi.md#platformComposeMove) | **POST** /v1/platform/compose/move | Move compose to a different environment |
| [**platformComposeOne**](ComposeApi.md#platformComposeOne) | **GET** /v1/platform/compose/one | Get compose service details |
| [**platformComposeRedeploy**](ComposeApi.md#platformComposeRedeploy) | **POST** /v1/platform/compose/redeploy | Redeploy (rebuild) a compose service |
| [**platformComposeRefreshToken**](ComposeApi.md#platformComposeRefreshToken) | **POST** /v1/platform/compose/refreshToken | Regenerate webhook token |
| [**platformComposeStart**](ComposeApi.md#platformComposeStart) | **POST** /v1/platform/compose/start | Start a compose service |
| [**platformComposeStop**](ComposeApi.md#platformComposeStop) | **POST** /v1/platform/compose/stop | Stop a compose service |
| [**platformComposeTemplates**](ComposeApi.md#platformComposeTemplates) | **GET** /v1/platform/compose/templates | List available one-click templates |
| [**platformComposeUpdate**](ComposeApi.md#platformComposeUpdate) | **POST** /v1/platform/compose/update | Update compose configuration |


<a id="platformComposeCancelDeployment"></a>
# **platformComposeCancelDeployment**
> PlatformTRPCResult platformComposeCancelDeployment(platformComposeCancelDeploymentRequest)

Cancel in-progress compose deployment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ComposeApi()
val platformComposeCancelDeploymentRequest : PlatformComposeCancelDeploymentRequest =  // PlatformComposeCancelDeploymentRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformComposeCancelDeployment(platformComposeCancelDeploymentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ComposeApi#platformComposeCancelDeployment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComposeApi#platformComposeCancelDeployment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformComposeCancelDeploymentRequest** | [**PlatformComposeCancelDeploymentRequest**](PlatformComposeCancelDeploymentRequest.md)|  | |

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

<a id="platformComposeCreate"></a>
# **platformComposeCreate**
> PlatformTRPCResult platformComposeCreate(platformComposeCreateRequest)

Create a Docker Compose service

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ComposeApi()
val platformComposeCreateRequest : PlatformComposeCreateRequest =  // PlatformComposeCreateRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformComposeCreate(platformComposeCreateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ComposeApi#platformComposeCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComposeApi#platformComposeCreate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformComposeCreateRequest** | [**PlatformComposeCreateRequest**](PlatformComposeCreateRequest.md)|  | |

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

<a id="platformComposeDelete"></a>
# **platformComposeDelete**
> PlatformTRPCResult platformComposeDelete(platformComposeDeleteRequest)

Delete a compose service

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ComposeApi()
val platformComposeDeleteRequest : PlatformComposeDeleteRequest =  // PlatformComposeDeleteRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformComposeDelete(platformComposeDeleteRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ComposeApi#platformComposeDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComposeApi#platformComposeDelete")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformComposeDeleteRequest** | [**PlatformComposeDeleteRequest**](PlatformComposeDeleteRequest.md)|  | |

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

<a id="platformComposeDeploy"></a>
# **platformComposeDeploy**
> PlatformTRPCResult platformComposeDeploy(platformComposeDeployRequest)

Deploy a compose service

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ComposeApi()
val platformComposeDeployRequest : PlatformComposeDeployRequest =  // PlatformComposeDeployRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformComposeDeploy(platformComposeDeployRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ComposeApi#platformComposeDeploy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComposeApi#platformComposeDeploy")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformComposeDeployRequest** | [**PlatformComposeDeployRequest**](PlatformComposeDeployRequest.md)|  | |

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

<a id="platformComposeDeployTemplate"></a>
# **platformComposeDeployTemplate**
> PlatformTRPCResult platformComposeDeployTemplate(platformComposeDeployTemplateRequest)

Deploy a one-click template

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ComposeApi()
val platformComposeDeployTemplateRequest : PlatformComposeDeployTemplateRequest =  // PlatformComposeDeployTemplateRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformComposeDeployTemplate(platformComposeDeployTemplateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ComposeApi#platformComposeDeployTemplate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComposeApi#platformComposeDeployTemplate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformComposeDeployTemplateRequest** | [**PlatformComposeDeployTemplateRequest**](PlatformComposeDeployTemplateRequest.md)|  | |

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

<a id="platformComposeDisconnectGitProvider"></a>
# **platformComposeDisconnectGitProvider**
> PlatformTRPCResult platformComposeDisconnectGitProvider(platformComposeCancelDeploymentRequest)

Disconnect git providers from compose

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ComposeApi()
val platformComposeCancelDeploymentRequest : PlatformComposeCancelDeploymentRequest =  // PlatformComposeCancelDeploymentRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformComposeDisconnectGitProvider(platformComposeCancelDeploymentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ComposeApi#platformComposeDisconnectGitProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComposeApi#platformComposeDisconnectGitProvider")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformComposeCancelDeploymentRequest** | [**PlatformComposeCancelDeploymentRequest**](PlatformComposeCancelDeploymentRequest.md)|  | |

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

<a id="platformComposeGetConvertedCompose"></a>
# **platformComposeGetConvertedCompose**
> PlatformTRPCResult platformComposeGetConvertedCompose(input)

Get final compose YAML with domains injected

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ComposeApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformComposeGetConvertedCompose(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ComposeApi#platformComposeGetConvertedCompose")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComposeApi#platformComposeGetConvertedCompose")
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

<a id="platformComposeGetDefaultCommand"></a>
# **platformComposeGetDefaultCommand**
> PlatformTRPCResult platformComposeGetDefaultCommand(input)

Get the docker compose command

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ComposeApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformComposeGetDefaultCommand(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ComposeApi#platformComposeGetDefaultCommand")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComposeApi#platformComposeGetDefaultCommand")
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

<a id="platformComposeGetTags"></a>
# **platformComposeGetTags**
> PlatformTRPCResult platformComposeGetTags(input)

Get unique tags from all templates

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ComposeApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformComposeGetTags(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ComposeApi#platformComposeGetTags")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComposeApi#platformComposeGetTags")
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

<a id="platformComposeLoadServices"></a>
# **platformComposeLoadServices**
> PlatformTRPCResult platformComposeLoadServices(input)

List running services within a compose stack

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ComposeApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformComposeLoadServices(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ComposeApi#platformComposeLoadServices")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComposeApi#platformComposeLoadServices")
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

<a id="platformComposeMove"></a>
# **platformComposeMove**
> PlatformTRPCResult platformComposeMove(platformComposeMoveRequest)

Move compose to a different environment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ComposeApi()
val platformComposeMoveRequest : PlatformComposeMoveRequest =  // PlatformComposeMoveRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformComposeMove(platformComposeMoveRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ComposeApi#platformComposeMove")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComposeApi#platformComposeMove")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformComposeMoveRequest** | [**PlatformComposeMoveRequest**](PlatformComposeMoveRequest.md)|  | |

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

<a id="platformComposeOne"></a>
# **platformComposeOne**
> PlatformTRPCResult platformComposeOne(input)

Get compose service details

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ComposeApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformComposeOne(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ComposeApi#platformComposeOne")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComposeApi#platformComposeOne")
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

<a id="platformComposeRedeploy"></a>
# **platformComposeRedeploy**
> PlatformTRPCResult platformComposeRedeploy(platformComposeDeployRequest)

Redeploy (rebuild) a compose service

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ComposeApi()
val platformComposeDeployRequest : PlatformComposeDeployRequest =  // PlatformComposeDeployRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformComposeRedeploy(platformComposeDeployRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ComposeApi#platformComposeRedeploy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComposeApi#platformComposeRedeploy")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformComposeDeployRequest** | [**PlatformComposeDeployRequest**](PlatformComposeDeployRequest.md)|  | |

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

<a id="platformComposeRefreshToken"></a>
# **platformComposeRefreshToken**
> PlatformTRPCResult platformComposeRefreshToken(platformComposeCancelDeploymentRequest)

Regenerate webhook token

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ComposeApi()
val platformComposeCancelDeploymentRequest : PlatformComposeCancelDeploymentRequest =  // PlatformComposeCancelDeploymentRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformComposeRefreshToken(platformComposeCancelDeploymentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ComposeApi#platformComposeRefreshToken")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComposeApi#platformComposeRefreshToken")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformComposeCancelDeploymentRequest** | [**PlatformComposeCancelDeploymentRequest**](PlatformComposeCancelDeploymentRequest.md)|  | |

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

<a id="platformComposeStart"></a>
# **platformComposeStart**
> PlatformTRPCResult platformComposeStart(platformComposeCancelDeploymentRequest)

Start a compose service

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ComposeApi()
val platformComposeCancelDeploymentRequest : PlatformComposeCancelDeploymentRequest =  // PlatformComposeCancelDeploymentRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformComposeStart(platformComposeCancelDeploymentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ComposeApi#platformComposeStart")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComposeApi#platformComposeStart")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformComposeCancelDeploymentRequest** | [**PlatformComposeCancelDeploymentRequest**](PlatformComposeCancelDeploymentRequest.md)|  | |

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

<a id="platformComposeStop"></a>
# **platformComposeStop**
> PlatformTRPCResult platformComposeStop(platformComposeCancelDeploymentRequest)

Stop a compose service

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ComposeApi()
val platformComposeCancelDeploymentRequest : PlatformComposeCancelDeploymentRequest =  // PlatformComposeCancelDeploymentRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformComposeStop(platformComposeCancelDeploymentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ComposeApi#platformComposeStop")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComposeApi#platformComposeStop")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformComposeCancelDeploymentRequest** | [**PlatformComposeCancelDeploymentRequest**](PlatformComposeCancelDeploymentRequest.md)|  | |

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

<a id="platformComposeTemplates"></a>
# **platformComposeTemplates**
> PlatformTRPCResult platformComposeTemplates(input)

List available one-click templates

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ComposeApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformComposeTemplates(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ComposeApi#platformComposeTemplates")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComposeApi#platformComposeTemplates")
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

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="platformComposeUpdate"></a>
# **platformComposeUpdate**
> PlatformTRPCResult platformComposeUpdate(platformComposeUpdateRequest)

Update compose configuration

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ComposeApi()
val platformComposeUpdateRequest : PlatformComposeUpdateRequest =  // PlatformComposeUpdateRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformComposeUpdate(platformComposeUpdateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ComposeApi#platformComposeUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComposeApi#platformComposeUpdate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformComposeUpdateRequest** | [**PlatformComposeUpdateRequest**](PlatformComposeUpdateRequest.md)|  | |

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

