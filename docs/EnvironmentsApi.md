# EnvironmentsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**kmsCreateEnvironment**](EnvironmentsApi.md#kmsCreateEnvironment) | **POST** /v1/kms/projects/{projectId}/environments | Create an environment |
| [**kmsDeleteEnvironment**](EnvironmentsApi.md#kmsDeleteEnvironment) | **DELETE** /v1/kms/projects/{projectId}/environments/{envId} | Delete an environment |
| [**kmsListEnvironments**](EnvironmentsApi.md#kmsListEnvironments) | **GET** /v1/kms/projects/{projectId}/environments | List project environments |
| [**kmsUpdateEnvironment**](EnvironmentsApi.md#kmsUpdateEnvironment) | **PATCH** /v1/kms/projects/{projectId}/environments/{envId} | Update an environment |
| [**paasCreateEnvironment**](EnvironmentsApi.md#paasCreateEnvironment) | **POST** /v1/paas/org/{orgId}/project/{projectId}/env | Create environment |
| [**paasDeleteEnvironment**](EnvironmentsApi.md#paasDeleteEnvironment) | **DELETE** /v1/paas/org/{orgId}/project/{projectId}/env/{envId} | Delete environment |
| [**paasGetEnvironment**](EnvironmentsApi.md#paasGetEnvironment) | **GET** /v1/paas/org/{orgId}/project/{projectId}/env/{envId} | Get environment |
| [**paasListEnvironments**](EnvironmentsApi.md#paasListEnvironments) | **GET** /v1/paas/org/{orgId}/project/{projectId}/env | List environments |


<a id="kmsCreateEnvironment"></a>
# **kmsCreateEnvironment**
> KmsCreateEnvironment200Response kmsCreateEnvironment(projectId, kmsCreateEnvironmentRequest)

Create an environment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EnvironmentsApi()
val projectId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val kmsCreateEnvironmentRequest : KmsCreateEnvironmentRequest =  // KmsCreateEnvironmentRequest | 
try {
    val result : KmsCreateEnvironment200Response = apiInstance.kmsCreateEnvironment(projectId, kmsCreateEnvironmentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EnvironmentsApi#kmsCreateEnvironment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EnvironmentsApi#kmsCreateEnvironment")
    e.printStackTrace()
}
```

### Parameters
| **projectId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsCreateEnvironmentRequest** | [**KmsCreateEnvironmentRequest**](KmsCreateEnvironmentRequest.md)|  | |

### Return type

[**KmsCreateEnvironment200Response**](KmsCreateEnvironment200Response.md)

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

<a id="kmsDeleteEnvironment"></a>
# **kmsDeleteEnvironment**
> kotlin.Any kmsDeleteEnvironment(projectId, envId)

Delete an environment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EnvironmentsApi()
val projectId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val envId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.kmsDeleteEnvironment(projectId, envId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EnvironmentsApi#kmsDeleteEnvironment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EnvironmentsApi#kmsDeleteEnvironment")
    e.printStackTrace()
}
```

### Parameters
| **projectId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **envId** | **java.util.UUID**|  | |

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

<a id="kmsListEnvironments"></a>
# **kmsListEnvironments**
> KmsListEnvironments200Response kmsListEnvironments(projectId)

List project environments

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EnvironmentsApi()
val projectId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : KmsListEnvironments200Response = apiInstance.kmsListEnvironments(projectId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EnvironmentsApi#kmsListEnvironments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EnvironmentsApi#kmsListEnvironments")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **projectId** | **java.util.UUID**|  | |

### Return type

[**KmsListEnvironments200Response**](KmsListEnvironments200Response.md)

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

<a id="kmsUpdateEnvironment"></a>
# **kmsUpdateEnvironment**
> KmsCreateEnvironment200Response kmsUpdateEnvironment(projectId, envId, kmsUpdateEnvironmentRequest)

Update an environment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EnvironmentsApi()
val projectId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val envId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val kmsUpdateEnvironmentRequest : KmsUpdateEnvironmentRequest =  // KmsUpdateEnvironmentRequest | 
try {
    val result : KmsCreateEnvironment200Response = apiInstance.kmsUpdateEnvironment(projectId, envId, kmsUpdateEnvironmentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EnvironmentsApi#kmsUpdateEnvironment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EnvironmentsApi#kmsUpdateEnvironment")
    e.printStackTrace()
}
```

### Parameters
| **projectId** | **java.util.UUID**|  | |
| **envId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsUpdateEnvironmentRequest** | [**KmsUpdateEnvironmentRequest**](KmsUpdateEnvironmentRequest.md)|  | |

### Return type

[**KmsCreateEnvironment200Response**](KmsCreateEnvironment200Response.md)

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

<a id="paasCreateEnvironment"></a>
# **paasCreateEnvironment**
> kotlin.Any paasCreateEnvironment(orgId, projectId, autoCreateTableRequest)

Create environment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EnvironmentsApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
val projectId : kotlin.String = projectId_example // kotlin.String | 
val autoCreateTableRequest : AutoCreateTableRequest =  // AutoCreateTableRequest | 
try {
    val result : kotlin.Any = apiInstance.paasCreateEnvironment(orgId, projectId, autoCreateTableRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EnvironmentsApi#paasCreateEnvironment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EnvironmentsApi#paasCreateEnvironment")
    e.printStackTrace()
}
```

### Parameters
| **orgId** | **kotlin.String**|  | |
| **projectId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoCreateTableRequest** | [**AutoCreateTableRequest**](AutoCreateTableRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="paasDeleteEnvironment"></a>
# **paasDeleteEnvironment**
> kotlin.Any paasDeleteEnvironment(orgId, projectId, envId)

Delete environment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EnvironmentsApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
val projectId : kotlin.String = projectId_example // kotlin.String | 
val envId : kotlin.String = envId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.paasDeleteEnvironment(orgId, projectId, envId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EnvironmentsApi#paasDeleteEnvironment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EnvironmentsApi#paasDeleteEnvironment")
    e.printStackTrace()
}
```

### Parameters
| **orgId** | **kotlin.String**|  | |
| **projectId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **envId** | **kotlin.String**|  | |

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

<a id="paasGetEnvironment"></a>
# **paasGetEnvironment**
> PaasEnvironment paasGetEnvironment(orgId, projectId, envId)

Get environment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EnvironmentsApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
val projectId : kotlin.String = projectId_example // kotlin.String | 
val envId : kotlin.String = envId_example // kotlin.String | 
try {
    val result : PaasEnvironment = apiInstance.paasGetEnvironment(orgId, projectId, envId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EnvironmentsApi#paasGetEnvironment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EnvironmentsApi#paasGetEnvironment")
    e.printStackTrace()
}
```

### Parameters
| **orgId** | **kotlin.String**|  | |
| **projectId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **envId** | **kotlin.String**|  | |

### Return type

[**PaasEnvironment**](PaasEnvironment.md)

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

<a id="paasListEnvironments"></a>
# **paasListEnvironments**
> kotlin.collections.List&lt;PaasEnvironment&gt; paasListEnvironments(orgId, projectId)

List environments

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EnvironmentsApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
val projectId : kotlin.String = projectId_example // kotlin.String | 
try {
    val result : kotlin.collections.List<PaasEnvironment> = apiInstance.paasListEnvironments(orgId, projectId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EnvironmentsApi#paasListEnvironments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EnvironmentsApi#paasListEnvironments")
    e.printStackTrace()
}
```

### Parameters
| **orgId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **projectId** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.List&lt;PaasEnvironment&gt;**](PaasEnvironment.md)

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

