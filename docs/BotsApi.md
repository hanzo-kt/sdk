# BotsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**visorBotAction**](BotsApi.md#visorBotAction) | **POST** /v1/bots/{id}/{action} | Act on a bot (stop, pause, or message) |
| [**visorDeleteBot**](BotsApi.md#visorDeleteBot) | **DELETE** /v1/bots/{id} | Terminate a bot (unbind agent + delete machine) |
| [**visorGetBot**](BotsApi.md#visorGetBot) | **GET** /v1/bots/{id} | Get one bot by id |
| [**visorLaunchBot**](BotsApi.md#visorLaunchBot) | **POST** /v1/bots/launch | Launch a bot (machine + agent binding), or dryRun for a quote |
| [**visorListBots**](BotsApi.md#visorListBots) | **GET** /v1/bots | List the org&#39;s bots |


<a id="visorBotAction"></a>
# **visorBotAction**
> kotlin.Any visorBotAction(id, action, body)

Act on a bot (stop, pause, or message)

&#x60;stop&#x60; and &#x60;pause&#x60; both halt the bot&#39;s agent runtime (one honest capability). &#x60;message&#x60; runs the bot&#39;s bound agent via the agent runner and returns that run&#39;s output verbatim. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BotsApi()
val id : kotlin.String = id_example // kotlin.String | 
val action : kotlin.String = action_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.visorBotAction(id, action, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BotsApi#visorBotAction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BotsApi#visorBotAction")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| **action** | **kotlin.String**|  | [enum: stop, pause, message] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | [optional] |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="visorDeleteBot"></a>
# **visorDeleteBot**
> visorDeleteBot(id)

Terminate a bot (unbind agent + delete machine)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BotsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.visorDeleteBot(id)
} catch (e: ClientException) {
    println("4xx response calling BotsApi#visorDeleteBot")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BotsApi#visorDeleteBot")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

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

<a id="visorGetBot"></a>
# **visorGetBot**
> VisorBotView visorGetBot(id)

Get one bot by id

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BotsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : VisorBotView = apiInstance.visorGetBot(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BotsApi#visorGetBot")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BotsApi#visorGetBot")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**VisorBotView**](VisorBotView.md)

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

<a id="visorLaunchBot"></a>
# **visorLaunchBot**
> kotlin.Any visorLaunchBot(visorBotLaunchRequest)

Launch a bot (machine + agent binding), or dryRun for a quote

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BotsApi()
val visorBotLaunchRequest : VisorBotLaunchRequest =  // VisorBotLaunchRequest | 
try {
    val result : kotlin.Any = apiInstance.visorLaunchBot(visorBotLaunchRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BotsApi#visorLaunchBot")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BotsApi#visorLaunchBot")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **visorBotLaunchRequest** | [**VisorBotLaunchRequest**](VisorBotLaunchRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="visorListBots"></a>
# **visorListBots**
> VisorListBots200Response visorListBots()

List the org&#39;s bots

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BotsApi()
try {
    val result : VisorListBots200Response = apiInstance.visorListBots()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BotsApi#visorListBots")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BotsApi#visorListBots")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**VisorListBots200Response**](VisorListBots200Response.md)

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

