# ScoreConfigsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**consoleCreateScoreConfig**](ScoreConfigsApi.md#consoleCreateScoreConfig) | **POST** /v1/console/score-configs | Create a score config |
| [**consoleGetScoreConfig**](ScoreConfigsApi.md#consoleGetScoreConfig) | **GET** /v1/console/score-configs/{configId} | Get a score config |
| [**consoleListScoreConfigs**](ScoreConfigsApi.md#consoleListScoreConfigs) | **GET** /v1/console/score-configs | Get all score configs |
| [**consoleUpdateScoreConfig**](ScoreConfigsApi.md#consoleUpdateScoreConfig) | **PATCH** /v1/console/score-configs/{configId} | Update a score config |


<a id="consoleCreateScoreConfig"></a>
# **consoleCreateScoreConfig**
> ConsoleScoreConfig consoleCreateScoreConfig(consoleCreateScoreConfigRequest)

Create a score config

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ScoreConfigsApi()
val consoleCreateScoreConfigRequest : ConsoleCreateScoreConfigRequest =  // ConsoleCreateScoreConfigRequest | 
try {
    val result : ConsoleScoreConfig = apiInstance.consoleCreateScoreConfig(consoleCreateScoreConfigRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ScoreConfigsApi#consoleCreateScoreConfig")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScoreConfigsApi#consoleCreateScoreConfig")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **consoleCreateScoreConfigRequest** | [**ConsoleCreateScoreConfigRequest**](ConsoleCreateScoreConfigRequest.md)|  | |

### Return type

[**ConsoleScoreConfig**](ConsoleScoreConfig.md)

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

<a id="consoleGetScoreConfig"></a>
# **consoleGetScoreConfig**
> ConsoleScoreConfig consoleGetScoreConfig(configId)

Get a score config

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ScoreConfigsApi()
val configId : kotlin.String = configId_example // kotlin.String | 
try {
    val result : ConsoleScoreConfig = apiInstance.consoleGetScoreConfig(configId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ScoreConfigsApi#consoleGetScoreConfig")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScoreConfigsApi#consoleGetScoreConfig")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **configId** | **kotlin.String**|  | |

### Return type

[**ConsoleScoreConfig**](ConsoleScoreConfig.md)

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

<a id="consoleListScoreConfigs"></a>
# **consoleListScoreConfigs**
> ConsoleListScoreConfigs200Response consoleListScoreConfigs(page, limit)

Get all score configs

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ScoreConfigsApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : ConsoleListScoreConfigs200Response = apiInstance.consoleListScoreConfigs(page, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ScoreConfigsApi#consoleListScoreConfigs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScoreConfigsApi#consoleListScoreConfigs")
    e.printStackTrace()
}
```

### Parameters
| **page** | **kotlin.Int**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] |

### Return type

[**ConsoleListScoreConfigs200Response**](ConsoleListScoreConfigs200Response.md)

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

<a id="consoleUpdateScoreConfig"></a>
# **consoleUpdateScoreConfig**
> ConsoleScoreConfig consoleUpdateScoreConfig(configId, consoleUpdateScoreConfigRequest)

Update a score config

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ScoreConfigsApi()
val configId : kotlin.String = configId_example // kotlin.String | 
val consoleUpdateScoreConfigRequest : ConsoleUpdateScoreConfigRequest =  // ConsoleUpdateScoreConfigRequest | 
try {
    val result : ConsoleScoreConfig = apiInstance.consoleUpdateScoreConfig(configId, consoleUpdateScoreConfigRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ScoreConfigsApi#consoleUpdateScoreConfig")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScoreConfigsApi#consoleUpdateScoreConfig")
    e.printStackTrace()
}
```

### Parameters
| **configId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **consoleUpdateScoreConfigRequest** | [**ConsoleUpdateScoreConfigRequest**](ConsoleUpdateScoreConfigRequest.md)|  | |

### Return type

[**ConsoleScoreConfig**](ConsoleScoreConfig.md)

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

