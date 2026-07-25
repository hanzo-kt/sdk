# UsageAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerGetRangeUsages**](UsageAPIApi.md#cloudApiControllerGetRangeUsages) | **GET** /v1/cloud/get-range-usages | Api Controller Get Range Usages |
| [**cloudApiControllerGetUserTableInfos**](UsageAPIApi.md#cloudApiControllerGetUserTableInfos) | **GET** /v1/cloud/get-usages | Api Controller Get User Table Infos |
| [**cloudApiControllerGetUsers**](UsageAPIApi.md#cloudApiControllerGetUsers) | **GET** /v1/cloud/get-users | Api Controller Get Users |
| [**nexusGetRangeUsages**](UsageAPIApi.md#nexusGetRangeUsages) | **GET** /v1/nexus/get-range-usages | get Range Usages |
| [**nexusGetUsages**](UsageAPIApi.md#nexusGetUsages) | **GET** /v1/nexus/get-usages | get Usages |
| [**nexusGetUsers**](UsageAPIApi.md#nexusGetUsers) | **GET** /v1/nexus/get-users | get Users |


<a id="cloudApiControllerGetRangeUsages"></a>
# **cloudApiControllerGetRangeUsages**
> kotlin.collections.List&lt;CloudObjectUsage&gt; cloudApiControllerGetRangeUsages(count)

Api Controller Get Range Usages

get range usages

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsageAPIApi()
val count : kotlin.String = count_example // kotlin.String | count of range usages
try {
    val result : kotlin.collections.List<CloudObjectUsage> = apiInstance.cloudApiControllerGetRangeUsages(count)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsageAPIApi#cloudApiControllerGetRangeUsages")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsageAPIApi#cloudApiControllerGetRangeUsages")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **count** | **kotlin.String**| count of range usages | |

### Return type

[**kotlin.collections.List&lt;CloudObjectUsage&gt;**](CloudObjectUsage.md)

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

<a id="cloudApiControllerGetUserTableInfos"></a>
# **cloudApiControllerGetUserTableInfos**
> kotlin.collections.List&lt;CloudObjectUsage&gt; cloudApiControllerGetUserTableInfos()

Api Controller Get User Table Infos

get userTableInfos

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsageAPIApi()
try {
    val result : kotlin.collections.List<CloudObjectUsage> = apiInstance.cloudApiControllerGetUserTableInfos()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsageAPIApi#cloudApiControllerGetUserTableInfos")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsageAPIApi#cloudApiControllerGetUserTableInfos")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;CloudObjectUsage&gt;**](CloudObjectUsage.md)

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

<a id="cloudApiControllerGetUsers"></a>
# **cloudApiControllerGetUsers**
> kotlin.collections.List&lt;kotlin.String&gt; cloudApiControllerGetUsers()

Api Controller Get Users

get users

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsageAPIApi()
try {
    val result : kotlin.collections.List<kotlin.String> = apiInstance.cloudApiControllerGetUsers()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsageAPIApi#cloudApiControllerGetUsers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsageAPIApi#cloudApiControllerGetUsers")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

**kotlin.collections.List&lt;kotlin.String&gt;**

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

<a id="nexusGetRangeUsages"></a>
# **nexusGetRangeUsages**
> kotlin.collections.List&lt;CloudObjectUsage&gt; nexusGetRangeUsages(count)

get Range Usages

Get range usages

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsageAPIApi()
val count : kotlin.String = count_example // kotlin.String | Count of range usages
try {
    val result : kotlin.collections.List<CloudObjectUsage> = apiInstance.nexusGetRangeUsages(count)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsageAPIApi#nexusGetRangeUsages")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsageAPIApi#nexusGetRangeUsages")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **count** | **kotlin.String**| Count of range usages | |

### Return type

[**kotlin.collections.List&lt;CloudObjectUsage&gt;**](CloudObjectUsage.md)

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

<a id="nexusGetUsages"></a>
# **nexusGetUsages**
> kotlin.collections.List&lt;CloudObjectUsage&gt; nexusGetUsages()

get Usages

Get usage information

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsageAPIApi()
try {
    val result : kotlin.collections.List<CloudObjectUsage> = apiInstance.nexusGetUsages()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsageAPIApi#nexusGetUsages")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsageAPIApi#nexusGetUsages")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;CloudObjectUsage&gt;**](CloudObjectUsage.md)

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

<a id="nexusGetUsers"></a>
# **nexusGetUsers**
> kotlin.collections.List&lt;kotlin.String&gt; nexusGetUsers()

get Users

Get users

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsageAPIApi()
try {
    val result : kotlin.collections.List<kotlin.String> = apiInstance.nexusGetUsers()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsageAPIApi#nexusGetUsers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsageAPIApi#nexusGetUsers")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

**kotlin.collections.List&lt;kotlin.String&gt;**

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

