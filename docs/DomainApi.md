# DomainApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformDomainByApplicationId**](DomainApi.md#platformDomainByApplicationId) | **GET** /v1/platform/domain/byApplicationId | List domains for an application |
| [**platformDomainByComposeId**](DomainApi.md#platformDomainByComposeId) | **GET** /v1/platform/domain/byComposeId | List domains for a compose service |
| [**platformDomainCreate**](DomainApi.md#platformDomainCreate) | **POST** /v1/platform/domain/create | Create a domain mapping |
| [**platformDomainDelete**](DomainApi.md#platformDomainDelete) | **POST** /v1/platform/domain/delete | Delete a domain |
| [**platformDomainGenerateDomain**](DomainApi.md#platformDomainGenerateDomain) | **POST** /v1/platform/domain/generateDomain | Generate a traefik.me auto-domain |
| [**platformDomainOne**](DomainApi.md#platformDomainOne) | **GET** /v1/platform/domain/one | Get a domain by ID |
| [**platformDomainUpdate**](DomainApi.md#platformDomainUpdate) | **POST** /v1/platform/domain/update | Update a domain mapping |
| [**platformDomainValidateDomain**](DomainApi.md#platformDomainValidateDomain) | **POST** /v1/platform/domain/validateDomain | Validate DNS for a domain |


<a id="platformDomainByApplicationId"></a>
# **platformDomainByApplicationId**
> PlatformTRPCResult platformDomainByApplicationId(input)

List domains for an application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DomainApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformDomainByApplicationId(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DomainApi#platformDomainByApplicationId")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DomainApi#platformDomainByApplicationId")
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

<a id="platformDomainByComposeId"></a>
# **platformDomainByComposeId**
> PlatformTRPCResult platformDomainByComposeId(input)

List domains for a compose service

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DomainApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformDomainByComposeId(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DomainApi#platformDomainByComposeId")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DomainApi#platformDomainByComposeId")
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

<a id="platformDomainCreate"></a>
# **platformDomainCreate**
> PlatformTRPCResult platformDomainCreate(platformDomainCreateRequest)

Create a domain mapping

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DomainApi()
val platformDomainCreateRequest : PlatformDomainCreateRequest =  // PlatformDomainCreateRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformDomainCreate(platformDomainCreateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DomainApi#platformDomainCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DomainApi#platformDomainCreate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformDomainCreateRequest** | [**PlatformDomainCreateRequest**](PlatformDomainCreateRequest.md)|  | |

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

<a id="platformDomainDelete"></a>
# **platformDomainDelete**
> PlatformTRPCResult platformDomainDelete(platformDomainDeleteRequest)

Delete a domain

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DomainApi()
val platformDomainDeleteRequest : PlatformDomainDeleteRequest =  // PlatformDomainDeleteRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformDomainDelete(platformDomainDeleteRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DomainApi#platformDomainDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DomainApi#platformDomainDelete")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformDomainDeleteRequest** | [**PlatformDomainDeleteRequest**](PlatformDomainDeleteRequest.md)|  | |

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

<a id="platformDomainGenerateDomain"></a>
# **platformDomainGenerateDomain**
> PlatformTRPCResult platformDomainGenerateDomain(platformDomainGenerateDomainRequest)

Generate a traefik.me auto-domain

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DomainApi()
val platformDomainGenerateDomainRequest : PlatformDomainGenerateDomainRequest =  // PlatformDomainGenerateDomainRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformDomainGenerateDomain(platformDomainGenerateDomainRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DomainApi#platformDomainGenerateDomain")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DomainApi#platformDomainGenerateDomain")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformDomainGenerateDomainRequest** | [**PlatformDomainGenerateDomainRequest**](PlatformDomainGenerateDomainRequest.md)|  | |

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

<a id="platformDomainOne"></a>
# **platformDomainOne**
> PlatformTRPCResult platformDomainOne(input)

Get a domain by ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DomainApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformDomainOne(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DomainApi#platformDomainOne")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DomainApi#platformDomainOne")
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

<a id="platformDomainUpdate"></a>
# **platformDomainUpdate**
> PlatformTRPCResult platformDomainUpdate(platformDomainUpdateRequest)

Update a domain mapping

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DomainApi()
val platformDomainUpdateRequest : PlatformDomainUpdateRequest =  // PlatformDomainUpdateRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformDomainUpdate(platformDomainUpdateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DomainApi#platformDomainUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DomainApi#platformDomainUpdate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformDomainUpdateRequest** | [**PlatformDomainUpdateRequest**](PlatformDomainUpdateRequest.md)|  | |

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

<a id="platformDomainValidateDomain"></a>
# **platformDomainValidateDomain**
> PlatformTRPCResult platformDomainValidateDomain(platformDomainValidateDomainRequest)

Validate DNS for a domain

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DomainApi()
val platformDomainValidateDomainRequest : PlatformDomainValidateDomainRequest =  // PlatformDomainValidateDomainRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformDomainValidateDomain(platformDomainValidateDomainRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DomainApi#platformDomainValidateDomain")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DomainApi#platformDomainValidateDomain")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformDomainValidateDomainRequest** | [**PlatformDomainValidateDomainRequest**](PlatformDomainValidateDomainRequest.md)|  | |

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

