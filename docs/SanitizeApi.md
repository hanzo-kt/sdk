# SanitizeApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**guardSanitizeInput**](SanitizeApi.md#guardSanitizeInput) | **POST** /v1/guard/sanitize/input | Sanitize user input |
| [**guardSanitizeOutput**](SanitizeApi.md#guardSanitizeOutput) | **POST** /v1/guard/sanitize/output | Sanitize LLM output |


<a id="guardSanitizeInput"></a>
# **guardSanitizeInput**
> GuardSanitizeResult guardSanitizeInput(guardSanitizeRequest)

Sanitize user input

Sanitize user input before sending to an LLM. Runs all 5 stages: rate limiting → injection detection → PII redaction → content filtering → audit logging. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SanitizeApi()
val guardSanitizeRequest : GuardSanitizeRequest = {"text":"My SSN is 123-45-6789 and my card is 4111111111111111","direction":"input","user_id":"usr_123"} // GuardSanitizeRequest | 
try {
    val result : GuardSanitizeResult = apiInstance.guardSanitizeInput(guardSanitizeRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SanitizeApi#guardSanitizeInput")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SanitizeApi#guardSanitizeInput")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **guardSanitizeRequest** | [**GuardSanitizeRequest**](GuardSanitizeRequest.md)|  | |

### Return type

[**GuardSanitizeResult**](GuardSanitizeResult.md)

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

<a id="guardSanitizeOutput"></a>
# **guardSanitizeOutput**
> GuardSanitizeResult guardSanitizeOutput(guardSanitizeRequest)

Sanitize LLM output

Sanitize LLM output before returning to the user. Runs PII redaction and content filtering stages. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SanitizeApi()
val guardSanitizeRequest : GuardSanitizeRequest =  // GuardSanitizeRequest | 
try {
    val result : GuardSanitizeResult = apiInstance.guardSanitizeOutput(guardSanitizeRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SanitizeApi#guardSanitizeOutput")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SanitizeApi#guardSanitizeOutput")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **guardSanitizeRequest** | [**GuardSanitizeRequest**](GuardSanitizeRequest.md)|  | |

### Return type

[**GuardSanitizeResult**](GuardSanitizeResult.md)

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

