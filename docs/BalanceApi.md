# BalanceApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatGetBalance**](BalanceApi.md#chatGetBalance) | **GET** /v1/chat/balance | Get user token balance |


<a id="chatGetBalance"></a>
# **chatGetBalance**
> kotlin.Any chatGetBalance()

Get user token balance

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BalanceApi()
try {
    val result : kotlin.Any = apiInstance.chatGetBalance()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BalanceApi#chatGetBalance")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BalanceApi#chatGetBalance")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

