# ApplicationAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerAddApplication**](ApplicationAPIApi.md#cloudApiControllerAddApplication) | **POST** /v1/cloud/add-application | Api Controller Add Application |
| [**cloudApiControllerDeleteApplication**](ApplicationAPIApi.md#cloudApiControllerDeleteApplication) | **POST** /v1/cloud/delete-application | Api Controller Delete Application |
| [**cloudApiControllerDeployApplication**](ApplicationAPIApi.md#cloudApiControllerDeployApplication) | **POST** /v1/cloud/deploy-application | Api Controller Deploy Application |
| [**cloudApiControllerGetApplication**](ApplicationAPIApi.md#cloudApiControllerGetApplication) | **GET** /v1/cloud/get-application | Api Controller Get Application |
| [**cloudApiControllerGetApplicationStatus**](ApplicationAPIApi.md#cloudApiControllerGetApplicationStatus) | **GET** /v1/cloud/get-application-status | Api Controller Get Application Status |
| [**cloudApiControllerGetApplications**](ApplicationAPIApi.md#cloudApiControllerGetApplications) | **GET** /v1/cloud/get-applications | Api Controller Get Applications |
| [**cloudApiControllerUndeployApplication**](ApplicationAPIApi.md#cloudApiControllerUndeployApplication) | **POST** /v1/cloud/undeploy-application | Api Controller Undeploy Application |
| [**cloudApiControllerUpdateApplication**](ApplicationAPIApi.md#cloudApiControllerUpdateApplication) | **POST** /v1/cloud/update-application | Api Controller Update Application |
| [**nexusAddApplication**](ApplicationAPIApi.md#nexusAddApplication) | **POST** /v1/nexus/add-application | add Application |
| [**nexusDeleteApplication**](ApplicationAPIApi.md#nexusDeleteApplication) | **POST** /v1/nexus/delete-application | delete Application |
| [**nexusDeployApplication**](ApplicationAPIApi.md#nexusDeployApplication) | **POST** /v1/nexus/deploy-application | deploy Application |
| [**nexusGetApplication**](ApplicationAPIApi.md#nexusGetApplication) | **GET** /v1/nexus/get-application | get Application |
| [**nexusGetApplicationStatus**](ApplicationAPIApi.md#nexusGetApplicationStatus) | **GET** /v1/nexus/get-application-status | get Application Status |
| [**nexusGetApplications**](ApplicationAPIApi.md#nexusGetApplications) | **GET** /v1/nexus/get-applications | get Applications |
| [**nexusUndeployApplication**](ApplicationAPIApi.md#nexusUndeployApplication) | **POST** /v1/nexus/undeploy-application | undeploy Application |
| [**nexusUpdateApplication**](ApplicationAPIApi.md#nexusUpdateApplication) | **POST** /v1/nexus/update-application | update Application |


<a id="cloudApiControllerAddApplication"></a>
# **cloudApiControllerAddApplication**
> CloudControllersResponse cloudApiControllerAddApplication(cloudObjectApplication)

Api Controller Add Application

add application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationAPIApi()
val cloudObjectApplication : CloudObjectApplication =  // CloudObjectApplication | The details of the application
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerAddApplication(cloudObjectApplication)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationAPIApi#cloudApiControllerAddApplication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationAPIApi#cloudApiControllerAddApplication")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectApplication** | [**CloudObjectApplication**](CloudObjectApplication.md)| The details of the application | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="cloudApiControllerDeleteApplication"></a>
# **cloudApiControllerDeleteApplication**
> CloudControllersResponse cloudApiControllerDeleteApplication(cloudObjectApplication)

Api Controller Delete Application

delete application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationAPIApi()
val cloudObjectApplication : CloudObjectApplication =  // CloudObjectApplication | The details of the application
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerDeleteApplication(cloudObjectApplication)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationAPIApi#cloudApiControllerDeleteApplication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationAPIApi#cloudApiControllerDeleteApplication")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectApplication** | [**CloudObjectApplication**](CloudObjectApplication.md)| The details of the application | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="cloudApiControllerDeployApplication"></a>
# **cloudApiControllerDeployApplication**
> CloudControllersResponse cloudApiControllerDeployApplication(body)

Api Controller Deploy Application

deploy application synchronously

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationAPIApi()
val body : kotlin.Any = Object // kotlin.Any | The deployment request details
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerDeployApplication(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationAPIApi#cloudApiControllerDeployApplication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationAPIApi#cloudApiControllerDeployApplication")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**| The deployment request details | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="cloudApiControllerGetApplication"></a>
# **cloudApiControllerGetApplication**
> CloudObjectApplication cloudApiControllerGetApplication(id)

Api Controller Get Application

get application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id of application
try {
    val result : CloudObjectApplication = apiInstance.cloudApiControllerGetApplication(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationAPIApi#cloudApiControllerGetApplication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationAPIApi#cloudApiControllerGetApplication")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id of application | |

### Return type

[**CloudObjectApplication**](CloudObjectApplication.md)

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

<a id="cloudApiControllerGetApplicationStatus"></a>
# **cloudApiControllerGetApplicationStatus**
> kotlin.Any cloudApiControllerGetApplicationStatus(id)

Api Controller Get Application Status

get application deployment status

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the application
try {
    val result : kotlin.Any = apiInstance.cloudApiControllerGetApplicationStatus(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationAPIApi#cloudApiControllerGetApplicationStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationAPIApi#cloudApiControllerGetApplicationStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id (owner/name) of the application | |

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

<a id="cloudApiControllerGetApplications"></a>
# **cloudApiControllerGetApplications**
> kotlin.collections.List&lt;CloudObjectApplication&gt; cloudApiControllerGetApplications(owner)

Api Controller Get Applications

get applications

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationAPIApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of applications
try {
    val result : kotlin.collections.List<CloudObjectApplication> = apiInstance.cloudApiControllerGetApplications(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationAPIApi#cloudApiControllerGetApplications")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationAPIApi#cloudApiControllerGetApplications")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of applications | |

### Return type

[**kotlin.collections.List&lt;CloudObjectApplication&gt;**](CloudObjectApplication.md)

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

<a id="cloudApiControllerUndeployApplication"></a>
# **cloudApiControllerUndeployApplication**
> CloudControllersResponse cloudApiControllerUndeployApplication(body)

Api Controller Undeploy Application

undeploy application synchronously

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationAPIApi()
val body : kotlin.Any = Object // kotlin.Any | The deployment request details
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerUndeployApplication(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationAPIApi#cloudApiControllerUndeployApplication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationAPIApi#cloudApiControllerUndeployApplication")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**| The deployment request details | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="cloudApiControllerUpdateApplication"></a>
# **cloudApiControllerUpdateApplication**
> CloudControllersResponse cloudApiControllerUpdateApplication(id, cloudObjectApplication)

Api Controller Update Application

update application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the application
val cloudObjectApplication : CloudObjectApplication =  // CloudObjectApplication | The details of the application
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerUpdateApplication(id, cloudObjectApplication)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationAPIApi#cloudApiControllerUpdateApplication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationAPIApi#cloudApiControllerUpdateApplication")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the application | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectApplication** | [**CloudObjectApplication**](CloudObjectApplication.md)| The details of the application | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="nexusAddApplication"></a>
# **nexusAddApplication**
> NexusResponse nexusAddApplication(cloudObjectApplication)

add Application

Add an application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationAPIApi()
val cloudObjectApplication : CloudObjectApplication =  // CloudObjectApplication | The details of the application
try {
    val result : NexusResponse = apiInstance.nexusAddApplication(cloudObjectApplication)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationAPIApi#nexusAddApplication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationAPIApi#nexusAddApplication")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectApplication** | [**CloudObjectApplication**](CloudObjectApplication.md)| The details of the application | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

<a id="nexusDeleteApplication"></a>
# **nexusDeleteApplication**
> NexusResponse nexusDeleteApplication(cloudObjectApplication)

delete Application

Delete an application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationAPIApi()
val cloudObjectApplication : CloudObjectApplication =  // CloudObjectApplication | The details of the application
try {
    val result : NexusResponse = apiInstance.nexusDeleteApplication(cloudObjectApplication)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationAPIApi#nexusDeleteApplication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationAPIApi#nexusDeleteApplication")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectApplication** | [**CloudObjectApplication**](CloudObjectApplication.md)| The details of the application | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

<a id="nexusDeployApplication"></a>
# **nexusDeployApplication**
> NexusResponse nexusDeployApplication(body)

deploy Application

Deploy an application synchronously

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationAPIApi()
val body : kotlin.Any = Object // kotlin.Any | The deployment request details
try {
    val result : NexusResponse = apiInstance.nexusDeployApplication(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationAPIApi#nexusDeployApplication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationAPIApi#nexusDeployApplication")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**| The deployment request details | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

<a id="nexusGetApplication"></a>
# **nexusGetApplication**
> CloudObjectApplication nexusGetApplication(id)

get Application

Get an application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id of the application
try {
    val result : CloudObjectApplication = apiInstance.nexusGetApplication(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationAPIApi#nexusGetApplication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationAPIApi#nexusGetApplication")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id of the application | |

### Return type

[**CloudObjectApplication**](CloudObjectApplication.md)

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

<a id="nexusGetApplicationStatus"></a>
# **nexusGetApplicationStatus**
> kotlin.Any nexusGetApplicationStatus(id)

get Application Status

Get application deployment status

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the application
try {
    val result : kotlin.Any = apiInstance.nexusGetApplicationStatus(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationAPIApi#nexusGetApplicationStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationAPIApi#nexusGetApplicationStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id (owner/name) of the application | |

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

<a id="nexusGetApplications"></a>
# **nexusGetApplications**
> kotlin.collections.List&lt;CloudObjectApplication&gt; nexusGetApplications(owner)

get Applications

Get applications

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationAPIApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of the applications
try {
    val result : kotlin.collections.List<CloudObjectApplication> = apiInstance.nexusGetApplications(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationAPIApi#nexusGetApplications")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationAPIApi#nexusGetApplications")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of the applications | |

### Return type

[**kotlin.collections.List&lt;CloudObjectApplication&gt;**](CloudObjectApplication.md)

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

<a id="nexusUndeployApplication"></a>
# **nexusUndeployApplication**
> NexusResponse nexusUndeployApplication(body)

undeploy Application

Undeploy an application synchronously

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationAPIApi()
val body : kotlin.Any = Object // kotlin.Any | The deployment request details
try {
    val result : NexusResponse = apiInstance.nexusUndeployApplication(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationAPIApi#nexusUndeployApplication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationAPIApi#nexusUndeployApplication")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**| The deployment request details | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

<a id="nexusUpdateApplication"></a>
# **nexusUpdateApplication**
> NexusResponse nexusUpdateApplication(id, cloudObjectApplication)

update Application

Update an application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the application
val cloudObjectApplication : CloudObjectApplication =  // CloudObjectApplication | The details of the application
try {
    val result : NexusResponse = apiInstance.nexusUpdateApplication(id, cloudObjectApplication)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationAPIApi#nexusUpdateApplication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationAPIApi#nexusUpdateApplication")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the application | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectApplication** | [**CloudObjectApplication**](CloudObjectApplication.md)| The details of the application | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

