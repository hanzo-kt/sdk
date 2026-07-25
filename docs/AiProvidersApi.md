# AiProvidersApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoDeleteAiProvider**](AiProvidersApi.md#autoDeleteAiProvider) | **DELETE** /v1/auto/ai-providers/{provider} | Delete an AI provider |
| [**autoListAiProviders**](AiProvidersApi.md#autoListAiProviders) | **GET** /v1/auto/ai-providers | List configured AI providers |
| [**autoUpsertAiProvider**](AiProvidersApi.md#autoUpsertAiProvider) | **POST** /v1/auto/ai-providers | Add or update an AI provider |
| [**flowDeleteAiProvider**](AiProvidersApi.md#flowDeleteAiProvider) | **DELETE** /v1/flow/ai-providers/{provider} | Delete an AI provider |
| [**flowListAiProviders**](AiProvidersApi.md#flowListAiProviders) | **GET** /v1/flow/ai-providers | List configured AI providers |
| [**flowUpsertAiProvider**](AiProvidersApi.md#flowUpsertAiProvider) | **POST** /v1/flow/ai-providers | Add or update an AI provider |


<a id="autoDeleteAiProvider"></a>
# **autoDeleteAiProvider**
> autoDeleteAiProvider(provider)

Delete an AI provider

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AiProvidersApi()
val provider : kotlin.String = provider_example // kotlin.String | 
try {
    apiInstance.autoDeleteAiProvider(provider)
} catch (e: ClientException) {
    println("4xx response calling AiProvidersApi#autoDeleteAiProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AiProvidersApi#autoDeleteAiProvider")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **provider** | **kotlin.String**|  | |

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
 - **Accept**: Not defined

<a id="autoListAiProviders"></a>
# **autoListAiProviders**
> kotlin.Any autoListAiProviders()

List configured AI providers

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AiProvidersApi()
try {
    val result : kotlin.Any = apiInstance.autoListAiProviders()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AiProvidersApi#autoListAiProviders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AiProvidersApi#autoListAiProviders")
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

<a id="autoUpsertAiProvider"></a>
# **autoUpsertAiProvider**
> kotlin.Any autoUpsertAiProvider(autoUpsertAiProviderRequest)

Add or update an AI provider

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AiProvidersApi()
val autoUpsertAiProviderRequest : AutoUpsertAiProviderRequest =  // AutoUpsertAiProviderRequest | 
try {
    val result : kotlin.Any = apiInstance.autoUpsertAiProvider(autoUpsertAiProviderRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AiProvidersApi#autoUpsertAiProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AiProvidersApi#autoUpsertAiProvider")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoUpsertAiProviderRequest** | [**AutoUpsertAiProviderRequest**](AutoUpsertAiProviderRequest.md)|  | |

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

<a id="flowDeleteAiProvider"></a>
# **flowDeleteAiProvider**
> flowDeleteAiProvider(provider)

Delete an AI provider

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AiProvidersApi()
val provider : kotlin.String = provider_example // kotlin.String | 
try {
    apiInstance.flowDeleteAiProvider(provider)
} catch (e: ClientException) {
    println("4xx response calling AiProvidersApi#flowDeleteAiProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AiProvidersApi#flowDeleteAiProvider")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **provider** | **kotlin.String**|  | |

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
 - **Accept**: Not defined

<a id="flowListAiProviders"></a>
# **flowListAiProviders**
> kotlin.Any flowListAiProviders()

List configured AI providers

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AiProvidersApi()
try {
    val result : kotlin.Any = apiInstance.flowListAiProviders()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AiProvidersApi#flowListAiProviders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AiProvidersApi#flowListAiProviders")
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

<a id="flowUpsertAiProvider"></a>
# **flowUpsertAiProvider**
> kotlin.Any flowUpsertAiProvider(autoUpsertAiProviderRequest)

Add or update an AI provider

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AiProvidersApi()
val autoUpsertAiProviderRequest : AutoUpsertAiProviderRequest =  // AutoUpsertAiProviderRequest | 
try {
    val result : kotlin.Any = apiInstance.flowUpsertAiProvider(autoUpsertAiProviderRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AiProvidersApi#flowUpsertAiProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AiProvidersApi#flowUpsertAiProvider")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoUpsertAiProviderRequest** | [**AutoUpsertAiProviderRequest**](AutoUpsertAiProviderRequest.md)|  | |

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

