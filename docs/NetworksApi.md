# NetworksApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**ztGetNetwork**](NetworksApi.md#ztGetNetwork) | **GET** /v1/networks/{id} | Get one overlay network by id |
| [**ztListNetworks**](NetworksApi.md#ztListNetworks) | **GET** /v1/networks | List the org&#39;s ZT overlay network(s) |


<a id="ztGetNetwork"></a>
# **ztGetNetwork**
> ZtNetworkView ztGetNetwork(id)

Get one overlay network by id

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NetworksApi()
val id : kotlin.String = id_example // kotlin.String | The org-derived network id (org-<org>)
try {
    val result : ZtNetworkView = apiInstance.ztGetNetwork(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NetworksApi#ztGetNetwork")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NetworksApi#ztGetNetwork")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The org-derived network id (org-&lt;org&gt;) | |

### Return type

[**ZtNetworkView**](ZtNetworkView.md)

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

<a id="ztListNetworks"></a>
# **ztListNetworks**
> ZtListNetworks200Response ztListNetworks()

List the org&#39;s ZT overlay network(s)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NetworksApi()
try {
    val result : ZtListNetworks200Response = apiInstance.ztListNetworks()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NetworksApi#ztListNetworks")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NetworksApi#ztListNetworks")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ZtListNetworks200Response**](ZtListNetworks200Response.md)

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

