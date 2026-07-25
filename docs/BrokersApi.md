# BrokersApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**streamGetBrokerConfig**](BrokersApi.md#streamGetBrokerConfig) | **GET** /v1/stream/brokers/config | Get broker configuration |
| [**streamListBrokers**](BrokersApi.md#streamListBrokers) | **GET** /v1/stream/brokers | List broker instances |


<a id="streamGetBrokerConfig"></a>
# **streamGetBrokerConfig**
> StreamGetBrokerConfig200Response streamGetBrokerConfig()

Get broker configuration

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BrokersApi()
try {
    val result : StreamGetBrokerConfig200Response = apiInstance.streamGetBrokerConfig()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BrokersApi#streamGetBrokerConfig")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BrokersApi#streamGetBrokerConfig")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**StreamGetBrokerConfig200Response**](StreamGetBrokerConfig200Response.md)

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

<a id="streamListBrokers"></a>
# **streamListBrokers**
> StreamListBrokers200Response streamListBrokers()

List broker instances

Returns metadata for all Hanzo Stream broker instances.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BrokersApi()
try {
    val result : StreamListBrokers200Response = apiInstance.streamListBrokers()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BrokersApi#streamListBrokers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BrokersApi#streamListBrokers")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**StreamListBrokers200Response**](StreamListBrokers200Response.md)

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

