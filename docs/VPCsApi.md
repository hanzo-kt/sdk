# VPCsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**doCreateVpc**](VPCsApi.md#doCreateVpc) | **POST** /v1/vpcs | Create a VPC |
| [**doDeleteVpc**](VPCsApi.md#doDeleteVpc) | **DELETE** /v1/vpcs/{id} | Delete one VPC (owned) |
| [**doGetVpc**](VPCsApi.md#doGetVpc) | **GET** /v1/vpcs/{id} | Get one VPC (owned) |
| [**doListVpcs**](VPCsApi.md#doListVpcs) | **GET** /v1/vpcs | List the caller&#39;s VPCs |


<a id="doCreateVpc"></a>
# **doCreateVpc**
> DoVpc doCreateVpc(doVpcCreate)

Create a VPC

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VPCsApi()
val doVpcCreate : DoVpcCreate =  // DoVpcCreate | 
try {
    val result : DoVpc = apiInstance.doCreateVpc(doVpcCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VPCsApi#doCreateVpc")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VPCsApi#doCreateVpc")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **doVpcCreate** | [**DoVpcCreate**](DoVpcCreate.md)|  | |

### Return type

[**DoVpc**](DoVpc.md)

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

<a id="doDeleteVpc"></a>
# **doDeleteVpc**
> doDeleteVpc(id)

Delete one VPC (owned)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VPCsApi()
val id : kotlin.String = id_example // kotlin.String | DO VPC id
try {
    apiInstance.doDeleteVpc(id)
} catch (e: ClientException) {
    println("4xx response calling VPCsApi#doDeleteVpc")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VPCsApi#doDeleteVpc")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| DO VPC id | |

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

<a id="doGetVpc"></a>
# **doGetVpc**
> DoVpc doGetVpc(id)

Get one VPC (owned)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VPCsApi()
val id : kotlin.String = id_example // kotlin.String | DO VPC id
try {
    val result : DoVpc = apiInstance.doGetVpc(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VPCsApi#doGetVpc")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VPCsApi#doGetVpc")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| DO VPC id | |

### Return type

[**DoVpc**](DoVpc.md)

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

<a id="doListVpcs"></a>
# **doListVpcs**
> DoListVpcs200Response doListVpcs()

List the caller&#39;s VPCs

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VPCsApi()
try {
    val result : DoListVpcs200Response = apiInstance.doListVpcs()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VPCsApi#doListVpcs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VPCsApi#doListVpcs")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**DoListVpcs200Response**](DoListVpcs200Response.md)

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

