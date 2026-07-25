# ServerApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformServerAll**](ServerApi.md#platformServerAll) | **GET** /v1/platform/server/all | List all servers with service counts |
| [**platformServerCreate**](ServerApi.md#platformServerCreate) | **POST** /v1/platform/server/create | Register a new remote server |
| [**platformServerGetServerMetrics**](ServerApi.md#platformServerGetServerMetrics) | **GET** /v1/platform/server/getServerMetrics | Fetch server metrics (CPU, memory, disk, network) |
| [**platformServerOne**](ServerApi.md#platformServerOne) | **GET** /v1/platform/server/one | Get server details |
| [**platformServerPublicIp**](ServerApi.md#platformServerPublicIp) | **GET** /v1/platform/server/publicIp | Get platform host public IP |
| [**platformServerRemove**](ServerApi.md#platformServerRemove) | **POST** /v1/platform/server/remove | Remove a server (must have no active services) |
| [**platformServerSecurity**](ServerApi.md#platformServerSecurity) | **GET** /v1/platform/server/security | Run security audit (ufw, ssh, fail2ban) |
| [**platformServerSetup**](ServerApi.md#platformServerSetup) | **POST** /v1/platform/server/setup | Run initial setup (install Docker, Traefik, etc.) |
| [**platformServerSetupMonitoring**](ServerApi.md#platformServerSetupMonitoring) | **POST** /v1/platform/server/setupMonitoring | Configure and deploy monitoring agent |
| [**platformServerUpdate**](ServerApi.md#platformServerUpdate) | **POST** /v1/platform/server/update | Update server configuration |
| [**platformServerValidate**](ServerApi.md#platformServerValidate) | **GET** /v1/platform/server/validate | Validate server capabilities |


<a id="platformServerAll"></a>
# **platformServerAll**
> PlatformTRPCResult platformServerAll()

List all servers with service counts

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ServerApi()
try {
    val result : PlatformTRPCResult = apiInstance.platformServerAll()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServerApi#platformServerAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServerApi#platformServerAll")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

<a id="platformServerCreate"></a>
# **platformServerCreate**
> PlatformTRPCResult platformServerCreate(platformServerCreateRequest)

Register a new remote server

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ServerApi()
val platformServerCreateRequest : PlatformServerCreateRequest =  // PlatformServerCreateRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformServerCreate(platformServerCreateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServerApi#platformServerCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServerApi#platformServerCreate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformServerCreateRequest** | [**PlatformServerCreateRequest**](PlatformServerCreateRequest.md)|  | |

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

<a id="platformServerGetServerMetrics"></a>
# **platformServerGetServerMetrics**
> PlatformTRPCResult platformServerGetServerMetrics(input)

Fetch server metrics (CPU, memory, disk, network)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ServerApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformServerGetServerMetrics(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServerApi#platformServerGetServerMetrics")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServerApi#platformServerGetServerMetrics")
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

<a id="platformServerOne"></a>
# **platformServerOne**
> PlatformTRPCResult platformServerOne(input)

Get server details

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ServerApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformServerOne(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServerApi#platformServerOne")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServerApi#platformServerOne")
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

<a id="platformServerPublicIp"></a>
# **platformServerPublicIp**
> PlatformTRPCResult platformServerPublicIp()

Get platform host public IP

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ServerApi()
try {
    val result : PlatformTRPCResult = apiInstance.platformServerPublicIp()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServerApi#platformServerPublicIp")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServerApi#platformServerPublicIp")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

<a id="platformServerRemove"></a>
# **platformServerRemove**
> PlatformTRPCResult platformServerRemove(platformServerRemoveRequest)

Remove a server (must have no active services)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ServerApi()
val platformServerRemoveRequest : PlatformServerRemoveRequest =  // PlatformServerRemoveRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformServerRemove(platformServerRemoveRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServerApi#platformServerRemove")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServerApi#platformServerRemove")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformServerRemoveRequest** | [**PlatformServerRemoveRequest**](PlatformServerRemoveRequest.md)|  | |

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

<a id="platformServerSecurity"></a>
# **platformServerSecurity**
> PlatformTRPCResult platformServerSecurity(input)

Run security audit (ufw, ssh, fail2ban)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ServerApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformServerSecurity(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServerApi#platformServerSecurity")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServerApi#platformServerSecurity")
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

<a id="platformServerSetup"></a>
# **platformServerSetup**
> PlatformTRPCResult platformServerSetup(platformServerRemoveRequest)

Run initial setup (install Docker, Traefik, etc.)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ServerApi()
val platformServerRemoveRequest : PlatformServerRemoveRequest =  // PlatformServerRemoveRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformServerSetup(platformServerRemoveRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServerApi#platformServerSetup")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServerApi#platformServerSetup")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformServerRemoveRequest** | [**PlatformServerRemoveRequest**](PlatformServerRemoveRequest.md)|  | |

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

<a id="platformServerSetupMonitoring"></a>
# **platformServerSetupMonitoring**
> PlatformTRPCResult platformServerSetupMonitoring(platformServerSetupMonitoringRequest)

Configure and deploy monitoring agent

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ServerApi()
val platformServerSetupMonitoringRequest : PlatformServerSetupMonitoringRequest =  // PlatformServerSetupMonitoringRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformServerSetupMonitoring(platformServerSetupMonitoringRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServerApi#platformServerSetupMonitoring")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServerApi#platformServerSetupMonitoring")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformServerSetupMonitoringRequest** | [**PlatformServerSetupMonitoringRequest**](PlatformServerSetupMonitoringRequest.md)|  | |

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

<a id="platformServerUpdate"></a>
# **platformServerUpdate**
> PlatformTRPCResult platformServerUpdate(platformServerUpdateRequest)

Update server configuration

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ServerApi()
val platformServerUpdateRequest : PlatformServerUpdateRequest =  // PlatformServerUpdateRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformServerUpdate(platformServerUpdateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServerApi#platformServerUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServerApi#platformServerUpdate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformServerUpdateRequest** | [**PlatformServerUpdateRequest**](PlatformServerUpdateRequest.md)|  | |

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

<a id="platformServerValidate"></a>
# **platformServerValidate**
> PlatformTRPCResult platformServerValidate(input)

Validate server capabilities

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ServerApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformServerValidate(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServerApi#platformServerValidate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServerApi#platformServerValidate")
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

