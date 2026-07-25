# ApplicationsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**iamApiControllerAddApplication**](ApplicationsApi.md#iamApiControllerAddApplication) | **POST** /v1/iam/applications | Api Controller Add Application |
| [**iamApiControllerDeleteApplication**](ApplicationsApi.md#iamApiControllerDeleteApplication) | **DELETE** /v1/iam/applications/{id} | Api Controller Delete Application |
| [**iamApiControllerGetApplication**](ApplicationsApi.md#iamApiControllerGetApplication) | **GET** /v1/iam/applications/{id} | Api Controller Get Application |
| [**iamApiControllerGetApplications**](ApplicationsApi.md#iamApiControllerGetApplications) | **GET** /v1/iam/applications | Api Controller Get Applications |
| [**iamApiControllerGetOrganizationApplications**](ApplicationsApi.md#iamApiControllerGetOrganizationApplications) | **GET** /v1/iam/organizations/applications | Api Controller Get Organization Applications |
| [**iamApiControllerGetUserApplication**](ApplicationsApi.md#iamApiControllerGetUserApplication) | **GET** /v1/iam/users/application | Api Controller Get User Application |
| [**iamApiControllerUpdateApplication**](ApplicationsApi.md#iamApiControllerUpdateApplication) | **PUT** /v1/iam/applications/{id} | Api Controller Update Application |


<a id="iamApiControllerAddApplication"></a>
# **iamApiControllerAddApplication**
> IamControllersResponse iamApiControllerAddApplication(iamObjectApplication)

Api Controller Add Application

add an application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationsApi()
val iamObjectApplication : IamObjectApplication =  // IamObjectApplication | The details of the application
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddApplication(iamObjectApplication)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationsApi#iamApiControllerAddApplication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationsApi#iamApiControllerAddApplication")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectApplication** | [**IamObjectApplication**](IamObjectApplication.md)| The details of the application | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerDeleteApplication"></a>
# **iamApiControllerDeleteApplication**
> IamControllersResponse iamApiControllerDeleteApplication(id, iamObjectApplication)

Api Controller Delete Application

delete an application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationsApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectApplication : IamObjectApplication =  // IamObjectApplication | The details of the application
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeleteApplication(id, iamObjectApplication)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationsApi#iamApiControllerDeleteApplication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationsApi#iamApiControllerDeleteApplication")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectApplication** | [**IamObjectApplication**](IamObjectApplication.md)| The details of the application | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerGetApplication"></a>
# **iamApiControllerGetApplication**
> IamObjectApplication iamApiControllerGetApplication(id)

Api Controller Get Application

get the detail of an application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the application.
try {
    val result : IamObjectApplication = apiInstance.iamApiControllerGetApplication(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationsApi#iamApiControllerGetApplication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationsApi#iamApiControllerGetApplication")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the application. | |

### Return type

[**IamObjectApplication**](IamObjectApplication.md)

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

<a id="iamApiControllerGetApplications"></a>
# **iamApiControllerGetApplications**
> kotlin.collections.List&lt;IamObjectApplication&gt; iamApiControllerGetApplications(owner)

Api Controller Get Applications

get all applications

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationsApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of applications.
try {
    val result : kotlin.collections.List<IamObjectApplication> = apiInstance.iamApiControllerGetApplications(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationsApi#iamApiControllerGetApplications")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationsApi#iamApiControllerGetApplications")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of applications. | |

### Return type

[**kotlin.collections.List&lt;IamObjectApplication&gt;**](IamObjectApplication.md)

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

<a id="iamApiControllerGetOrganizationApplications"></a>
# **iamApiControllerGetOrganizationApplications**
> kotlin.collections.List&lt;IamObjectApplication&gt; iamApiControllerGetOrganizationApplications(organization)

Api Controller Get Organization Applications

get the detail of the organization&#39;s application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationsApi()
val organization : kotlin.String = organization_example // kotlin.String | The organization name
try {
    val result : kotlin.collections.List<IamObjectApplication> = apiInstance.iamApiControllerGetOrganizationApplications(organization)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationsApi#iamApiControllerGetOrganizationApplications")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationsApi#iamApiControllerGetOrganizationApplications")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **organization** | **kotlin.String**| The organization name | |

### Return type

[**kotlin.collections.List&lt;IamObjectApplication&gt;**](IamObjectApplication.md)

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

<a id="iamApiControllerGetUserApplication"></a>
# **iamApiControllerGetUserApplication**
> IamObjectApplication iamApiControllerGetUserApplication(id)

Api Controller Get User Application

get the detail of the user&#39;s application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the user
try {
    val result : IamObjectApplication = apiInstance.iamApiControllerGetUserApplication(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationsApi#iamApiControllerGetUserApplication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationsApi#iamApiControllerGetUserApplication")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the user | |

### Return type

[**IamObjectApplication**](IamObjectApplication.md)

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

<a id="iamApiControllerUpdateApplication"></a>
# **iamApiControllerUpdateApplication**
> IamControllersResponse iamApiControllerUpdateApplication(id, iamObjectApplication)

Api Controller Update Application

update an application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApplicationsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the application
val iamObjectApplication : IamObjectApplication =  // IamObjectApplication | The details of the application
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdateApplication(id, iamObjectApplication)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApplicationsApi#iamApiControllerUpdateApplication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApplicationsApi#iamApiControllerUpdateApplication")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the application | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectApplication** | [**IamObjectApplication**](IamObjectApplication.md)| The details of the application | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

