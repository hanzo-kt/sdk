# FlagsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoGetFlags**](FlagsApi.md#autoGetFlags) | **GET** /v1/auto/flags | Get feature flags and configuration |
| [**flowGetFlags**](FlagsApi.md#flowGetFlags) | **GET** /v1/flow/flags | Get feature flags and configuration |


<a id="autoGetFlags"></a>
# **autoGetFlags**
> kotlin.Any autoGetFlags()

Get feature flags and configuration

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlagsApi()
try {
    val result : kotlin.Any = apiInstance.autoGetFlags()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlagsApi#autoGetFlags")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlagsApi#autoGetFlags")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="flowGetFlags"></a>
# **flowGetFlags**
> kotlin.Any flowGetFlags()

Get feature flags and configuration

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlagsApi()
try {
    val result : kotlin.Any = apiInstance.flowGetFlags()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlagsApi#flowGetFlags")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlagsApi#flowGetFlags")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

