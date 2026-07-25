# ApplicationApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformApplicationCancelDeployment**](ApplicationApi.md#platformApplicationCancelDeployment) | **POST** /v1/platform/application/cancelDeployment | Cancel an in-progress deployment |
| [**platformApplicationCleanQueues**](ApplicationApi.md#platformApplicationCleanQueues) | **POST** /v1/platform/application/cleanQueues | Clear pending deployment jobs |
| [**platformApplicationCreate**](ApplicationApi.md#platformApplicationCreate) | **POST** /v1/platform/application/create | Create a new application |
| [**platformApplicationDelete**](ApplicationApi.md#platformApplicationDelete) | **POST** /v1/platform/application/delete | Delete an application and all associated resources |
| [**platformApplicationDeploy**](ApplicationApi.md#platformApplicationDeploy) | **POST** /v1/platform/application/deploy | Trigger a new deployment |
| [**platformApplicationDisconnectGitProvider**](ApplicationApi.md#platformApplicationDisconnectGitProvider) | **POST** /v1/platform/application/disconnectGitProvider | Disconnect all git providers from application |
| [**platformApplicationMarkRunning**](ApplicationApi.md#platformApplicationMarkRunning) | **POST** /v1/platform/application/markRunning | Mark application status as running |
| [**platformApplicationMove**](ApplicationApi.md#platformApplicationMove) | **POST** /v1/platform/application/move | Move application to a different environment |
| [**platformApplicationOne**](ApplicationApi.md#platformApplicationOne) | **GET** /v1/platform/application/one | Get application details |
| [**platformApplicationReadAppMonitoring**](ApplicationApi.md#platformApplicationReadAppMonitoring) | **GET** /v1/platform/application/readAppMonitoring | Read container monitoring stats |
| [**platformApplicationReadTraefikConfig**](ApplicationApi.md#platformApplicationReadTraefikConfig) | **GET** /v1/platform/application/readTraefikConfig | Read Traefik routing config for an application |
| [**platformApplicationRedeploy**](ApplicationApi.md#platformApplicationRedeploy) | **POST** /v1/platform/application/redeploy | Redeploy (rebuild) an application |
| [**platformApplicationRefreshToken**](ApplicationApi.md#platformApplicationRefreshToken) | **POST** /v1/platform/application/refreshToken | Regenerate webhook refresh token |
| [**platformApplicationReload**](ApplicationApi.md#platformApplicationReload) | **POST** /v1/platform/application/reload | Reload application container (re-mechanize) |
| [**platformApplicationSaveBitbucketProvider**](ApplicationApi.md#platformApplicationSaveBitbucketProvider) | **POST** /v1/platform/application/saveBitbucketProvider | Configure Bitbucket as source provider |
| [**platformApplicationSaveBuildType**](ApplicationApi.md#platformApplicationSaveBuildType) | **POST** /v1/platform/application/saveBuildType | Configure the build type |
| [**platformApplicationSaveDockerProvider**](ApplicationApi.md#platformApplicationSaveDockerProvider) | **POST** /v1/platform/application/saveDockerProvider | Configure Docker image as source |
| [**platformApplicationSaveEnvironment**](ApplicationApi.md#platformApplicationSaveEnvironment) | **POST** /v1/platform/application/saveEnvironment | Save environment variables and build args |
| [**platformApplicationSaveGitProdiver**](ApplicationApi.md#platformApplicationSaveGitProdiver) | **POST** /v1/platform/application/saveGitProdiver | Configure custom Git URL as source |
| [**platformApplicationSaveGiteaProvider**](ApplicationApi.md#platformApplicationSaveGiteaProvider) | **POST** /v1/platform/application/saveGiteaProvider | Configure Gitea as source provider |
| [**platformApplicationSaveGithubProvider**](ApplicationApi.md#platformApplicationSaveGithubProvider) | **POST** /v1/platform/application/saveGithubProvider | Configure GitHub as source provider |
| [**platformApplicationSaveGitlabProvider**](ApplicationApi.md#platformApplicationSaveGitlabProvider) | **POST** /v1/platform/application/saveGitlabProvider | Configure GitLab as source provider |
| [**platformApplicationStart**](ApplicationApi.md#platformApplicationStart) | **POST** /v1/platform/application/start | Start a stopped application |
| [**platformApplicationStop**](ApplicationApi.md#platformApplicationStop) | **POST** /v1/platform/application/stop | Stop a running application |
| [**platformApplicationUpdate**](ApplicationApi.md#platformApplicationUpdate) | **POST** /v1/platform/application/update | Update application configuration |
| [**platformApplicationUpdateTraefikConfig**](ApplicationApi.md#platformApplicationUpdateTraefikConfig) | **POST** /v1/platform/application/updateTraefikConfig | Write Traefik routing config |


<a id="platformApplicationCancelDeployment"></a>
# **platformApplicationCancelDeployment**
> PlatformTRPCResult platformApplicationCancelDeployment(platformApplicationCancelDeploymentRequest)

Cancel an in-progress deployment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val platformApplicationCancelDeploymentRequest : PlatformApplicationCancelDeploymentRequest =  // PlatformApplicationCancelDeploymentRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationCancelDeployment(platformApplicationCancelDeploymentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationCancelDeployment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationCancelDeployment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformApplicationCancelDeploymentRequest** | [**PlatformApplicationCancelDeploymentRequest**](PlatformApplicationCancelDeploymentRequest.md)|  | |

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

<a id="platformApplicationCleanQueues"></a>
# **platformApplicationCleanQueues**
> PlatformTRPCResult platformApplicationCleanQueues(platformApplicationCancelDeploymentRequest)

Clear pending deployment jobs

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val platformApplicationCancelDeploymentRequest : PlatformApplicationCancelDeploymentRequest =  // PlatformApplicationCancelDeploymentRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationCleanQueues(platformApplicationCancelDeploymentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationCleanQueues")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationCleanQueues")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformApplicationCancelDeploymentRequest** | [**PlatformApplicationCancelDeploymentRequest**](PlatformApplicationCancelDeploymentRequest.md)|  | |

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

<a id="platformApplicationCreate"></a>
# **platformApplicationCreate**
> PlatformTRPCResult platformApplicationCreate(platformApplicationCreateRequest)

Create a new application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val platformApplicationCreateRequest : PlatformApplicationCreateRequest =  // PlatformApplicationCreateRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationCreate(platformApplicationCreateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationCreate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformApplicationCreateRequest** | [**PlatformApplicationCreateRequest**](PlatformApplicationCreateRequest.md)|  | |

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

<a id="platformApplicationDelete"></a>
# **platformApplicationDelete**
> PlatformTRPCResult platformApplicationDelete(platformApplicationCancelDeploymentRequest)

Delete an application and all associated resources

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val platformApplicationCancelDeploymentRequest : PlatformApplicationCancelDeploymentRequest =  // PlatformApplicationCancelDeploymentRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationDelete(platformApplicationCancelDeploymentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationDelete")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformApplicationCancelDeploymentRequest** | [**PlatformApplicationCancelDeploymentRequest**](PlatformApplicationCancelDeploymentRequest.md)|  | |

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

<a id="platformApplicationDeploy"></a>
# **platformApplicationDeploy**
> PlatformTRPCResult platformApplicationDeploy(platformApplicationDeployRequest)

Trigger a new deployment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val platformApplicationDeployRequest : PlatformApplicationDeployRequest =  // PlatformApplicationDeployRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationDeploy(platformApplicationDeployRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationDeploy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationDeploy")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformApplicationDeployRequest** | [**PlatformApplicationDeployRequest**](PlatformApplicationDeployRequest.md)|  | |

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

<a id="platformApplicationDisconnectGitProvider"></a>
# **platformApplicationDisconnectGitProvider**
> PlatformTRPCResult platformApplicationDisconnectGitProvider(platformApplicationCancelDeploymentRequest)

Disconnect all git providers from application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val platformApplicationCancelDeploymentRequest : PlatformApplicationCancelDeploymentRequest =  // PlatformApplicationCancelDeploymentRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationDisconnectGitProvider(platformApplicationCancelDeploymentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationDisconnectGitProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationDisconnectGitProvider")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformApplicationCancelDeploymentRequest** | [**PlatformApplicationCancelDeploymentRequest**](PlatformApplicationCancelDeploymentRequest.md)|  | |

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

<a id="platformApplicationMarkRunning"></a>
# **platformApplicationMarkRunning**
> PlatformTRPCResult platformApplicationMarkRunning(platformApplicationCancelDeploymentRequest)

Mark application status as running

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val platformApplicationCancelDeploymentRequest : PlatformApplicationCancelDeploymentRequest =  // PlatformApplicationCancelDeploymentRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationMarkRunning(platformApplicationCancelDeploymentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationMarkRunning")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationMarkRunning")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformApplicationCancelDeploymentRequest** | [**PlatformApplicationCancelDeploymentRequest**](PlatformApplicationCancelDeploymentRequest.md)|  | |

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

<a id="platformApplicationMove"></a>
# **platformApplicationMove**
> PlatformTRPCResult platformApplicationMove(platformApplicationMoveRequest)

Move application to a different environment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val platformApplicationMoveRequest : PlatformApplicationMoveRequest =  // PlatformApplicationMoveRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationMove(platformApplicationMoveRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationMove")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationMove")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformApplicationMoveRequest** | [**PlatformApplicationMoveRequest**](PlatformApplicationMoveRequest.md)|  | |

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

<a id="platformApplicationOne"></a>
# **platformApplicationOne**
> PlatformTRPCResult platformApplicationOne(input)

Get application details

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationOne(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationOne")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationOne")
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

<a id="platformApplicationReadAppMonitoring"></a>
# **platformApplicationReadAppMonitoring**
> PlatformTRPCResult platformApplicationReadAppMonitoring(input)

Read container monitoring stats

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationReadAppMonitoring(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationReadAppMonitoring")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationReadAppMonitoring")
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

<a id="platformApplicationReadTraefikConfig"></a>
# **platformApplicationReadTraefikConfig**
> PlatformTRPCResult platformApplicationReadTraefikConfig(input)

Read Traefik routing config for an application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationReadTraefikConfig(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationReadTraefikConfig")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationReadTraefikConfig")
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

<a id="platformApplicationRedeploy"></a>
# **platformApplicationRedeploy**
> PlatformTRPCResult platformApplicationRedeploy(platformApplicationDeployRequest)

Redeploy (rebuild) an application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val platformApplicationDeployRequest : PlatformApplicationDeployRequest =  // PlatformApplicationDeployRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationRedeploy(platformApplicationDeployRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationRedeploy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationRedeploy")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformApplicationDeployRequest** | [**PlatformApplicationDeployRequest**](PlatformApplicationDeployRequest.md)|  | |

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

<a id="platformApplicationRefreshToken"></a>
# **platformApplicationRefreshToken**
> PlatformTRPCResult platformApplicationRefreshToken(platformApplicationCancelDeploymentRequest)

Regenerate webhook refresh token

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val platformApplicationCancelDeploymentRequest : PlatformApplicationCancelDeploymentRequest =  // PlatformApplicationCancelDeploymentRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationRefreshToken(platformApplicationCancelDeploymentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationRefreshToken")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationRefreshToken")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformApplicationCancelDeploymentRequest** | [**PlatformApplicationCancelDeploymentRequest**](PlatformApplicationCancelDeploymentRequest.md)|  | |

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

<a id="platformApplicationReload"></a>
# **platformApplicationReload**
> PlatformTRPCResult platformApplicationReload(platformApplicationCancelDeploymentRequest)

Reload application container (re-mechanize)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val platformApplicationCancelDeploymentRequest : PlatformApplicationCancelDeploymentRequest =  // PlatformApplicationCancelDeploymentRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationReload(platformApplicationCancelDeploymentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationReload")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationReload")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformApplicationCancelDeploymentRequest** | [**PlatformApplicationCancelDeploymentRequest**](PlatformApplicationCancelDeploymentRequest.md)|  | |

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

<a id="platformApplicationSaveBitbucketProvider"></a>
# **platformApplicationSaveBitbucketProvider**
> PlatformTRPCResult platformApplicationSaveBitbucketProvider(platformApplicationSaveBitbucketProviderRequest)

Configure Bitbucket as source provider

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val platformApplicationSaveBitbucketProviderRequest : PlatformApplicationSaveBitbucketProviderRequest =  // PlatformApplicationSaveBitbucketProviderRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationSaveBitbucketProvider(platformApplicationSaveBitbucketProviderRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationSaveBitbucketProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationSaveBitbucketProvider")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformApplicationSaveBitbucketProviderRequest** | [**PlatformApplicationSaveBitbucketProviderRequest**](PlatformApplicationSaveBitbucketProviderRequest.md)|  | |

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

<a id="platformApplicationSaveBuildType"></a>
# **platformApplicationSaveBuildType**
> PlatformTRPCResult platformApplicationSaveBuildType(platformApplicationSaveBuildTypeRequest)

Configure the build type

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val platformApplicationSaveBuildTypeRequest : PlatformApplicationSaveBuildTypeRequest =  // PlatformApplicationSaveBuildTypeRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationSaveBuildType(platformApplicationSaveBuildTypeRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationSaveBuildType")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationSaveBuildType")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformApplicationSaveBuildTypeRequest** | [**PlatformApplicationSaveBuildTypeRequest**](PlatformApplicationSaveBuildTypeRequest.md)|  | |

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

<a id="platformApplicationSaveDockerProvider"></a>
# **platformApplicationSaveDockerProvider**
> PlatformTRPCResult platformApplicationSaveDockerProvider(platformApplicationSaveDockerProviderRequest)

Configure Docker image as source

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val platformApplicationSaveDockerProviderRequest : PlatformApplicationSaveDockerProviderRequest =  // PlatformApplicationSaveDockerProviderRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationSaveDockerProvider(platformApplicationSaveDockerProviderRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationSaveDockerProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationSaveDockerProvider")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformApplicationSaveDockerProviderRequest** | [**PlatformApplicationSaveDockerProviderRequest**](PlatformApplicationSaveDockerProviderRequest.md)|  | |

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

<a id="platformApplicationSaveEnvironment"></a>
# **platformApplicationSaveEnvironment**
> PlatformTRPCResult platformApplicationSaveEnvironment(platformApplicationSaveEnvironmentRequest)

Save environment variables and build args

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val platformApplicationSaveEnvironmentRequest : PlatformApplicationSaveEnvironmentRequest =  // PlatformApplicationSaveEnvironmentRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationSaveEnvironment(platformApplicationSaveEnvironmentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationSaveEnvironment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationSaveEnvironment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformApplicationSaveEnvironmentRequest** | [**PlatformApplicationSaveEnvironmentRequest**](PlatformApplicationSaveEnvironmentRequest.md)|  | |

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

<a id="platformApplicationSaveGitProdiver"></a>
# **platformApplicationSaveGitProdiver**
> PlatformTRPCResult platformApplicationSaveGitProdiver(platformApplicationSaveGitProdiverRequest)

Configure custom Git URL as source

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val platformApplicationSaveGitProdiverRequest : PlatformApplicationSaveGitProdiverRequest =  // PlatformApplicationSaveGitProdiverRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationSaveGitProdiver(platformApplicationSaveGitProdiverRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationSaveGitProdiver")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationSaveGitProdiver")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformApplicationSaveGitProdiverRequest** | [**PlatformApplicationSaveGitProdiverRequest**](PlatformApplicationSaveGitProdiverRequest.md)|  | |

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

<a id="platformApplicationSaveGiteaProvider"></a>
# **platformApplicationSaveGiteaProvider**
> PlatformTRPCResult platformApplicationSaveGiteaProvider(platformApplicationSaveGiteaProviderRequest)

Configure Gitea as source provider

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val platformApplicationSaveGiteaProviderRequest : PlatformApplicationSaveGiteaProviderRequest =  // PlatformApplicationSaveGiteaProviderRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationSaveGiteaProvider(platformApplicationSaveGiteaProviderRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationSaveGiteaProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationSaveGiteaProvider")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformApplicationSaveGiteaProviderRequest** | [**PlatformApplicationSaveGiteaProviderRequest**](PlatformApplicationSaveGiteaProviderRequest.md)|  | |

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

<a id="platformApplicationSaveGithubProvider"></a>
# **platformApplicationSaveGithubProvider**
> PlatformTRPCResult platformApplicationSaveGithubProvider(platformApplicationSaveGithubProviderRequest)

Configure GitHub as source provider

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val platformApplicationSaveGithubProviderRequest : PlatformApplicationSaveGithubProviderRequest =  // PlatformApplicationSaveGithubProviderRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationSaveGithubProvider(platformApplicationSaveGithubProviderRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationSaveGithubProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationSaveGithubProvider")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformApplicationSaveGithubProviderRequest** | [**PlatformApplicationSaveGithubProviderRequest**](PlatformApplicationSaveGithubProviderRequest.md)|  | |

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

<a id="platformApplicationSaveGitlabProvider"></a>
# **platformApplicationSaveGitlabProvider**
> PlatformTRPCResult platformApplicationSaveGitlabProvider(platformApplicationSaveGitlabProviderRequest)

Configure GitLab as source provider

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val platformApplicationSaveGitlabProviderRequest : PlatformApplicationSaveGitlabProviderRequest =  // PlatformApplicationSaveGitlabProviderRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationSaveGitlabProvider(platformApplicationSaveGitlabProviderRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationSaveGitlabProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationSaveGitlabProvider")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformApplicationSaveGitlabProviderRequest** | [**PlatformApplicationSaveGitlabProviderRequest**](PlatformApplicationSaveGitlabProviderRequest.md)|  | |

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

<a id="platformApplicationStart"></a>
# **platformApplicationStart**
> PlatformTRPCResult platformApplicationStart(platformApplicationCancelDeploymentRequest)

Start a stopped application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val platformApplicationCancelDeploymentRequest : PlatformApplicationCancelDeploymentRequest =  // PlatformApplicationCancelDeploymentRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationStart(platformApplicationCancelDeploymentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationStart")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationStart")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformApplicationCancelDeploymentRequest** | [**PlatformApplicationCancelDeploymentRequest**](PlatformApplicationCancelDeploymentRequest.md)|  | |

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

<a id="platformApplicationStop"></a>
# **platformApplicationStop**
> PlatformTRPCResult platformApplicationStop(platformApplicationCancelDeploymentRequest)

Stop a running application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val platformApplicationCancelDeploymentRequest : PlatformApplicationCancelDeploymentRequest =  // PlatformApplicationCancelDeploymentRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationStop(platformApplicationCancelDeploymentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationStop")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationStop")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformApplicationCancelDeploymentRequest** | [**PlatformApplicationCancelDeploymentRequest**](PlatformApplicationCancelDeploymentRequest.md)|  | |

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

<a id="platformApplicationUpdate"></a>
# **platformApplicationUpdate**
> PlatformTRPCResult platformApplicationUpdate(platformApplicationUpdateRequest)

Update application configuration

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val platformApplicationUpdateRequest : PlatformApplicationUpdateRequest =  // PlatformApplicationUpdateRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationUpdate(platformApplicationUpdateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationUpdate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformApplicationUpdateRequest** | [**PlatformApplicationUpdateRequest**](PlatformApplicationUpdateRequest.md)|  | |

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

<a id="platformApplicationUpdateTraefikConfig"></a>
# **platformApplicationUpdateTraefikConfig**
> PlatformTRPCResult platformApplicationUpdateTraefikConfig(platformApplicationUpdateTraefikConfigRequest)

Write Traefik routing config

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationApi()
val platformApplicationUpdateTraefikConfigRequest : PlatformApplicationUpdateTraefikConfigRequest =  // PlatformApplicationUpdateTraefikConfigRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformApplicationUpdateTraefikConfig(platformApplicationUpdateTraefikConfigRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationApi#platformApplicationUpdateTraefikConfig")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationApi#platformApplicationUpdateTraefikConfig")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformApplicationUpdateTraefikConfigRequest** | [**PlatformApplicationUpdateTraefikConfigRequest**](PlatformApplicationUpdateTraefikConfigRequest.md)|  | |

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

