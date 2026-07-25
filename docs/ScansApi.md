# ScansApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**registryGetScanReport**](ScansApi.md#registryGetScanReport) | **GET** /v1/registry/projects/{name}/repositories/{repo}/artifacts/{digest}/scan/report | Get scan report |
| [**registryTriggerScan**](ScansApi.md#registryTriggerScan) | **POST** /v1/registry/projects/{name}/repositories/{repo}/artifacts/{digest}/scan | Trigger vulnerability scan |
| [**securitySecurityGetScan**](ScansApi.md#securitySecurityGetScan) | **GET** /v1/security/scans/{id} | Get a scan with its findings |
| [**securitySecurityListScans**](ScansApi.md#securitySecurityListScans) | **GET** /v1/security/scans | List scans |
| [**securitySecuritySubmitScan**](ScansApi.md#securitySecuritySubmitScan) | **POST** /v1/security/scans | Submit a scan |


<a id="registryGetScanReport"></a>
# **registryGetScanReport**
> RegistryScanReport registryGetScanReport(name, repo, digest)

Get scan report

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ScansApi()
val name : kotlin.String = name_example // kotlin.String | 
val repo : kotlin.String = repo_example // kotlin.String | 
val digest : kotlin.String = digest_example // kotlin.String | 
try {
    val result : RegistryScanReport = apiInstance.registryGetScanReport(name, repo, digest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ScansApi#registryGetScanReport")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScansApi#registryGetScanReport")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**|  | |
| **repo** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **digest** | **kotlin.String**|  | |

### Return type

[**RegistryScanReport**](RegistryScanReport.md)

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

<a id="registryTriggerScan"></a>
# **registryTriggerScan**
> registryTriggerScan(name, repo, digest)

Trigger vulnerability scan

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ScansApi()
val name : kotlin.String = name_example // kotlin.String | 
val repo : kotlin.String = repo_example // kotlin.String | 
val digest : kotlin.String = digest_example // kotlin.String | 
try {
    apiInstance.registryTriggerScan(name, repo, digest)
} catch (e: ClientException) {
    println("4xx response calling ScansApi#registryTriggerScan")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScansApi#registryTriggerScan")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**|  | |
| **repo** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **digest** | **kotlin.String**|  | |

### Return type

null (empty response body)

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

<a id="securitySecurityGetScan"></a>
# **securitySecurityGetScan**
> SecuritySecurityGetScan200Response securitySecurityGetScan(id)

Get a scan with its findings

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ScansApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : SecuritySecurityGetScan200Response = apiInstance.securitySecurityGetScan(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ScansApi#securitySecurityGetScan")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScansApi#securitySecurityGetScan")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**SecuritySecurityGetScan200Response**](SecuritySecurityGetScan200Response.md)

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

<a id="securitySecurityListScans"></a>
# **securitySecurityListScans**
> SecuritySecurityListScans200Response securitySecurityListScans(limit)

List scans

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ScansApi()
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : SecuritySecurityListScans200Response = apiInstance.securitySecurityListScans(limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ScansApi#securitySecurityListScans")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScansApi#securitySecurityListScans")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] |

### Return type

[**SecuritySecurityListScans200Response**](SecuritySecurityListScans200Response.md)

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

<a id="securitySecuritySubmitScan"></a>
# **securitySecuritySubmitScan**
> SecurityScan securitySecuritySubmitScan(securityScanRequest)

Submit a scan

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ScansApi()
val securityScanRequest : SecurityScanRequest =  // SecurityScanRequest | 
try {
    val result : SecurityScan = apiInstance.securitySecuritySubmitScan(securityScanRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ScansApi#securitySecuritySubmitScan")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScansApi#securitySecuritySubmitScan")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **securityScanRequest** | [**SecurityScanRequest**](SecurityScanRequest.md)|  | |

### Return type

[**SecurityScan**](SecurityScan.md)

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

