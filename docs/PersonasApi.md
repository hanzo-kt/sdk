# PersonasApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**botGetPersona**](PersonasApi.md#botGetPersona) | **GET** /v1/bot/personas/{slug}/detail | Get persona detail including latest version and owner |
| [**botListPersonaVersions**](PersonasApi.md#botListPersonaVersions) | **GET** /v1/bot/personas/{slug}/versions | List versions of a persona |
| [**botListPersonas**](PersonasApi.md#botListPersonas) | **GET** /v1/bot/personas | List personas (paginated) |


<a id="botGetPersona"></a>
# **botGetPersona**
> BotGetPersona200Response botGetPersona(slug)

Get persona detail including latest version and owner

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PersonasApi()
val slug : kotlin.String = slug_example // kotlin.String | 
try {
    val result : BotGetPersona200Response = apiInstance.botGetPersona(slug)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PersonasApi#botGetPersona")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PersonasApi#botGetPersona")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **slug** | **kotlin.String**|  | |

### Return type

[**BotGetPersona200Response**](BotGetPersona200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="botListPersonaVersions"></a>
# **botListPersonaVersions**
> BotListPersonaVersions200Response botListPersonaVersions(slug, limit)

List versions of a persona

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PersonasApi()
val slug : kotlin.String = slug_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : BotListPersonaVersions200Response = apiInstance.botListPersonaVersions(slug, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PersonasApi#botListPersonaVersions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PersonasApi#botListPersonaVersions")
    e.printStackTrace()
}
```

### Parameters
| **slug** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] [default to 20] |

### Return type

[**BotListPersonaVersions200Response**](BotListPersonaVersions200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="botListPersonas"></a>
# **botListPersonas**
> BotListPersonas200Response botListPersonas(sort, limit, cursor)

List personas (paginated)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PersonasApi()
val sort : kotlin.String = sort_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val cursor : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
try {
    val result : BotListPersonas200Response = apiInstance.botListPersonas(sort, limit, cursor)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PersonasApi#botListPersonas")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PersonasApi#botListPersonas")
    e.printStackTrace()
}
```

### Parameters
| **sort** | **kotlin.String**|  | [optional] [default to Sort.updated] [enum: updated, downloads, stars, created] |
| **limit** | **kotlin.Int**|  | [optional] [default to 50] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cursor** | **java.time.OffsetDateTime**|  | [optional] |

### Return type

[**BotListPersonas200Response**](BotListPersonas200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

