# SystemAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerGetPrometheusInfo**](SystemAPIApi.md#cloudApiControllerGetPrometheusInfo) | **GET** /v1/cloud/get-prometheus-info | Api Controller Get Prometheus Info |
| [**cloudApiControllerGetSystemInfo**](SystemAPIApi.md#cloudApiControllerGetSystemInfo) | **GET** /v1/cloud/get-system-info | Api Controller Get System Info |
| [**cloudApiControllerGetVersionInfo**](SystemAPIApi.md#cloudApiControllerGetVersionInfo) | **GET** /v1/cloud/get-version-info | Api Controller Get Version Info |
| [**nexusGetPrometheusInfo**](SystemAPIApi.md#nexusGetPrometheusInfo) | **GET** /v1/nexus/get-prometheus-info | get Prometheus Info |
| [**nexusGetSystemInfo**](SystemAPIApi.md#nexusGetSystemInfo) | **GET** /v1/nexus/get-system-info | get System Info |
| [**nexusGetVersionInfo**](SystemAPIApi.md#nexusGetVersionInfo) | **GET** /v1/nexus/get-version-info | get Version Info |


<a id="cloudApiControllerGetPrometheusInfo"></a>
# **cloudApiControllerGetPrometheusInfo**
> CloudObjectPrometheusInfo cloudApiControllerGetPrometheusInfo()

Api Controller Get Prometheus Info

get Prometheus Info

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemAPIApi()
try {
    val result : CloudObjectPrometheusInfo = apiInstance.cloudApiControllerGetPrometheusInfo()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemAPIApi#cloudApiControllerGetPrometheusInfo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemAPIApi#cloudApiControllerGetPrometheusInfo")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**CloudObjectPrometheusInfo**](CloudObjectPrometheusInfo.md)

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

<a id="cloudApiControllerGetSystemInfo"></a>
# **cloudApiControllerGetSystemInfo**
> CloudUtilSystemInfo cloudApiControllerGetSystemInfo()

Api Controller Get System Info

get system info like CPU and memory usage

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemAPIApi()
try {
    val result : CloudUtilSystemInfo = apiInstance.cloudApiControllerGetSystemInfo()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemAPIApi#cloudApiControllerGetSystemInfo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemAPIApi#cloudApiControllerGetSystemInfo")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**CloudUtilSystemInfo**](CloudUtilSystemInfo.md)

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

<a id="cloudApiControllerGetVersionInfo"></a>
# **cloudApiControllerGetVersionInfo**
> CloudUtilVersionInfo cloudApiControllerGetVersionInfo()

Api Controller Get Version Info

get version info like IAM release version and commit ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemAPIApi()
try {
    val result : CloudUtilVersionInfo = apiInstance.cloudApiControllerGetVersionInfo()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemAPIApi#cloudApiControllerGetVersionInfo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemAPIApi#cloudApiControllerGetVersionInfo")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**CloudUtilVersionInfo**](CloudUtilVersionInfo.md)

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

<a id="nexusGetPrometheusInfo"></a>
# **nexusGetPrometheusInfo**
> NexusPrometheusInfo nexusGetPrometheusInfo()

get Prometheus Info

Get Prometheus metrics info

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemAPIApi()
try {
    val result : NexusPrometheusInfo = apiInstance.nexusGetPrometheusInfo()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemAPIApi#nexusGetPrometheusInfo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemAPIApi#nexusGetPrometheusInfo")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**NexusPrometheusInfo**](NexusPrometheusInfo.md)

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

<a id="nexusGetSystemInfo"></a>
# **nexusGetSystemInfo**
> CloudUtilSystemInfo nexusGetSystemInfo()

get System Info

Get system info (CPU, memory usage)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemAPIApi()
try {
    val result : CloudUtilSystemInfo = apiInstance.nexusGetSystemInfo()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemAPIApi#nexusGetSystemInfo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemAPIApi#nexusGetSystemInfo")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**CloudUtilSystemInfo**](CloudUtilSystemInfo.md)

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

<a id="nexusGetVersionInfo"></a>
# **nexusGetVersionInfo**
> CloudUtilVersionInfo nexusGetVersionInfo()

get Version Info

Get version info (release version, commit ID)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemAPIApi()
try {
    val result : CloudUtilVersionInfo = apiInstance.nexusGetVersionInfo()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemAPIApi#nexusGetVersionInfo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemAPIApi#nexusGetVersionInfo")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**CloudUtilVersionInfo**](CloudUtilVersionInfo.md)

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

