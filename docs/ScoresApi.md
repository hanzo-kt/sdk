# ScoresApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**consoleCreateScore**](ScoresApi.md#consoleCreateScore) | **POST** /v1/console/scores | Create a score |
| [**consoleDeleteScore**](ScoresApi.md#consoleDeleteScore) | **DELETE** /v1/console/scores/{scoreId} | Delete a score |
| [**consoleGetScore**](ScoresApi.md#consoleGetScore) | **GET** /v1/console/scores/{scoreId} | Get a score by ID |
| [**consoleListScores**](ScoresApi.md#consoleListScores) | **GET** /v1/console/scores | Get all scores |
| [**evalsGetV1EvalsScores**](ScoresApi.md#evalsGetV1EvalsScores) | **GET** /v1/evals/scores | List scores |


<a id="consoleCreateScore"></a>
# **consoleCreateScore**
> ConsoleCreateComment200Response consoleCreateScore(consoleCreateScoreRequest)

Create a score

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ScoresApi()
val consoleCreateScoreRequest : ConsoleCreateScoreRequest =  // ConsoleCreateScoreRequest | 
try {
    val result : ConsoleCreateComment200Response = apiInstance.consoleCreateScore(consoleCreateScoreRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ScoresApi#consoleCreateScore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScoresApi#consoleCreateScore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **consoleCreateScoreRequest** | [**ConsoleCreateScoreRequest**](ConsoleCreateScoreRequest.md)|  | |

### Return type

[**ConsoleCreateComment200Response**](ConsoleCreateComment200Response.md)

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

<a id="consoleDeleteScore"></a>
# **consoleDeleteScore**
> kotlin.Any consoleDeleteScore(scoreId)

Delete a score

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ScoresApi()
val scoreId : kotlin.String = scoreId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.consoleDeleteScore(scoreId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ScoresApi#consoleDeleteScore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScoresApi#consoleDeleteScore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **scoreId** | **kotlin.String**|  | |

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

<a id="consoleGetScore"></a>
# **consoleGetScore**
> ConsoleScore consoleGetScore(scoreId)

Get a score by ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ScoresApi()
val scoreId : kotlin.String = scoreId_example // kotlin.String | 
try {
    val result : ConsoleScore = apiInstance.consoleGetScore(scoreId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ScoresApi#consoleGetScore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScoresApi#consoleGetScore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **scoreId** | **kotlin.String**|  | |

### Return type

[**ConsoleScore**](ConsoleScore.md)

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

<a id="consoleListScores"></a>
# **consoleListScores**
> ConsoleListScores200Response consoleListScores(page, limit, userId, name, fromTimestamp, toTimestamp, source, `operator`, `value`, scoreIds, configId, dataType, environment)

Get all scores

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ScoresApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val userId : kotlin.String = userId_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val fromTimestamp : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
val toTimestamp : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
val source : kotlin.String = source_example // kotlin.String | 
val `operator` : kotlin.String = `operator`_example // kotlin.String | 
val `value` : java.math.BigDecimal = 8.14 // java.math.BigDecimal | 
val scoreIds : kotlin.String = scoreIds_example // kotlin.String | 
val configId : kotlin.String = configId_example // kotlin.String | 
val dataType : kotlin.String = dataType_example // kotlin.String | 
val environment : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
try {
    val result : ConsoleListScores200Response = apiInstance.consoleListScores(page, limit, userId, name, fromTimestamp, toTimestamp, source, `operator`, `value`, scoreIds, configId, dataType, environment)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ScoresApi#consoleListScores")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScoresApi#consoleListScores")
    e.printStackTrace()
}
```

### Parameters
| **page** | **kotlin.Int**|  | [optional] [default to 1] |
| **limit** | **kotlin.Int**|  | [optional] [default to 50] |
| **userId** | **kotlin.String**|  | [optional] |
| **name** | **kotlin.String**|  | [optional] |
| **fromTimestamp** | **java.time.OffsetDateTime**|  | [optional] |
| **toTimestamp** | **java.time.OffsetDateTime**|  | [optional] |
| **source** | **kotlin.String**|  | [optional] [enum: API, EVAL, ANNOTATION] |
| **&#x60;operator&#x60;** | **kotlin.String**|  | [optional] |
| **&#x60;value&#x60;** | **java.math.BigDecimal**|  | [optional] |
| **scoreIds** | **kotlin.String**|  | [optional] |
| **configId** | **kotlin.String**|  | [optional] |
| **dataType** | **kotlin.String**|  | [optional] [enum: NUMERIC, CATEGORICAL, BOOLEAN] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **environment** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional] |

### Return type

[**ConsoleListScores200Response**](ConsoleListScores200Response.md)

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

<a id="evalsGetV1EvalsScores"></a>
# **evalsGetV1EvalsScores**
> EvalsGetV1EvalsScores200Response evalsGetV1EvalsScores(runName, limit)

List scores

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ScoresApi()
val runName : kotlin.String = runName_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : EvalsGetV1EvalsScores200Response = apiInstance.evalsGetV1EvalsScores(runName, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ScoresApi#evalsGetV1EvalsScores")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScoresApi#evalsGetV1EvalsScores")
    e.printStackTrace()
}
```

### Parameters
| **runName** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] [default to 50] |

### Return type

[**EvalsGetV1EvalsScores200Response**](EvalsGetV1EvalsScores200Response.md)

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

