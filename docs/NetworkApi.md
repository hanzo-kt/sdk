# NetworkApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**searchGetNetwork**](NetworkApi.md#searchGetNetwork) | **GET** /v1/search/network | Get network/federation configuration |
| [**searchUpdateNetwork**](NetworkApi.md#searchUpdateNetwork) | **PATCH** /v1/search/network | Update network configuration |


<a id="searchGetNetwork"></a>
# **searchGetNetwork**
> SearchNetwork searchGetNetwork()

Get network/federation configuration

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NetworkApi()
try {
    val result : SearchNetwork = apiInstance.searchGetNetwork()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NetworkApi#searchGetNetwork")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NetworkApi#searchGetNetwork")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**SearchNetwork**](SearchNetwork.md)

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

<a id="searchUpdateNetwork"></a>
# **searchUpdateNetwork**
> SearchNetwork searchUpdateNetwork(searchNetwork)

Update network configuration

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NetworkApi()
val searchNetwork : SearchNetwork =  // SearchNetwork | 
try {
    val result : SearchNetwork = apiInstance.searchUpdateNetwork(searchNetwork)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NetworkApi#searchUpdateNetwork")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NetworkApi#searchUpdateNetwork")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **searchNetwork** | [**SearchNetwork**](SearchNetwork.md)|  | |

### Return type

[**SearchNetwork**](SearchNetwork.md)

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

