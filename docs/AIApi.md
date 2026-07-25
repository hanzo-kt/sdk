# AIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**worldWorldClassifyBatch**](AIApi.md#worldWorldClassifyBatch) | **POST** /v1/world/classify-batch | Batch headline classification (per-user IAM token) |
| [**worldWorldClassifyEvent**](AIApi.md#worldWorldClassifyEvent) | **POST** /v1/world/classify-event | Single event classification (per-user IAM token) |
| [**worldWorldCountryIntel**](AIApi.md#worldWorldCountryIntel) | **POST** /v1/world/country-intel | AI country intelligence brief (per-user IAM token) |
| [**worldWorldGroqSummarize**](AIApi.md#worldWorldGroqSummarize) | **POST** /v1/world/groq-summarize | World-brief summary via Hanzo inference (forwards the caller IAM token → org/project/billing; anon → skipped) |
| [**worldWorldOpenrouterSummarize**](AIApi.md#worldWorldOpenrouterSummarize) | **POST** /v1/world/openrouter-summarize | Alt summary path via Hanzo inference (per-user IAM token) |


<a id="worldWorldClassifyBatch"></a>
# **worldWorldClassifyBatch**
> kotlin.Any worldWorldClassifyBatch()

Batch headline classification (per-user IAM token)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AIApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldClassifyBatch()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AIApi#worldWorldClassifyBatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AIApi#worldWorldClassifyBatch")
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

<a id="worldWorldClassifyEvent"></a>
# **worldWorldClassifyEvent**
> kotlin.Any worldWorldClassifyEvent()

Single event classification (per-user IAM token)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AIApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldClassifyEvent()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AIApi#worldWorldClassifyEvent")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AIApi#worldWorldClassifyEvent")
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

<a id="worldWorldCountryIntel"></a>
# **worldWorldCountryIntel**
> kotlin.Any worldWorldCountryIntel()

AI country intelligence brief (per-user IAM token)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AIApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldCountryIntel()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AIApi#worldWorldCountryIntel")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AIApi#worldWorldCountryIntel")
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

<a id="worldWorldGroqSummarize"></a>
# **worldWorldGroqSummarize**
> kotlin.Any worldWorldGroqSummarize()

World-brief summary via Hanzo inference (forwards the caller IAM token → org/project/billing; anon → skipped)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AIApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldGroqSummarize()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AIApi#worldWorldGroqSummarize")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AIApi#worldWorldGroqSummarize")
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

<a id="worldWorldOpenrouterSummarize"></a>
# **worldWorldOpenrouterSummarize**
> kotlin.Any worldWorldOpenrouterSummarize()

Alt summary path via Hanzo inference (per-user IAM token)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AIApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldOpenrouterSummarize()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AIApi#worldWorldOpenrouterSummarize")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AIApi#worldWorldOpenrouterSummarize")
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

