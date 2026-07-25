# IntegrationsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**botGetIntegration**](IntegrationsApi.md#botGetIntegration) | **GET** /v1/bot/integrations/{slug} | Get integration detail with latest version |
| [**botListIntegrations**](IntegrationsApi.md#botListIntegrations) | **GET** /v1/bot/integrations | List integrations (paginated) |
| [**kmsCreateIntegration**](IntegrationsApi.md#kmsCreateIntegration) | **POST** /v1/kms/integration | Create an integration |
| [**kmsDeleteIntegration**](IntegrationsApi.md#kmsDeleteIntegration) | **DELETE** /v1/kms/integration/{integrationId} | Delete an integration |
| [**kmsUpdateIntegration**](IntegrationsApi.md#kmsUpdateIntegration) | **PATCH** /v1/kms/integration/{integrationId} | Update an integration |


<a id="botGetIntegration"></a>
# **botGetIntegration**
> BotGetIntegration200Response botGetIntegration(slug)

Get integration detail with latest version

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IntegrationsApi()
val slug : kotlin.String = slug_example // kotlin.String | 
try {
    val result : BotGetIntegration200Response = apiInstance.botGetIntegration(slug)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IntegrationsApi#botGetIntegration")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IntegrationsApi#botGetIntegration")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **slug** | **kotlin.String**|  | |

### Return type

[**BotGetIntegration200Response**](BotGetIntegration200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="botListIntegrations"></a>
# **botListIntegrations**
> BotListIntegrations200Response botListIntegrations(sort, limit, cursor)

List integrations (paginated)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IntegrationsApi()
val sort : kotlin.String = sort_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val cursor : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
try {
    val result : BotListIntegrations200Response = apiInstance.botListIntegrations(sort, limit, cursor)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IntegrationsApi#botListIntegrations")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IntegrationsApi#botListIntegrations")
    e.printStackTrace()
}
```

### Parameters
| **sort** | **kotlin.String**|  | [optional] [default to Sort.updated] [enum: updated, downloads, name] |
| **limit** | **kotlin.Int**|  | [optional] [default to 50] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cursor** | **java.time.OffsetDateTime**|  | [optional] |

### Return type

[**BotListIntegrations200Response**](BotListIntegrations200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="kmsCreateIntegration"></a>
# **kmsCreateIntegration**
> KmsCreateIntegration200Response kmsCreateIntegration(kmsCreateIntegrationRequest)

Create an integration

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IntegrationsApi()
val kmsCreateIntegrationRequest : KmsCreateIntegrationRequest =  // KmsCreateIntegrationRequest | 
try {
    val result : KmsCreateIntegration200Response = apiInstance.kmsCreateIntegration(kmsCreateIntegrationRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IntegrationsApi#kmsCreateIntegration")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IntegrationsApi#kmsCreateIntegration")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsCreateIntegrationRequest** | [**KmsCreateIntegrationRequest**](KmsCreateIntegrationRequest.md)|  | |

### Return type

[**KmsCreateIntegration200Response**](KmsCreateIntegration200Response.md)

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

<a id="kmsDeleteIntegration"></a>
# **kmsDeleteIntegration**
> kotlin.Any kmsDeleteIntegration(integrationId)

Delete an integration

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IntegrationsApi()
val integrationId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.kmsDeleteIntegration(integrationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IntegrationsApi#kmsDeleteIntegration")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IntegrationsApi#kmsDeleteIntegration")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **integrationId** | **java.util.UUID**|  | |

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

<a id="kmsUpdateIntegration"></a>
# **kmsUpdateIntegration**
> KmsCreateIntegration200Response kmsUpdateIntegration(integrationId, kmsUpdateIntegrationRequest)

Update an integration

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IntegrationsApi()
val integrationId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val kmsUpdateIntegrationRequest : KmsUpdateIntegrationRequest =  // KmsUpdateIntegrationRequest | 
try {
    val result : KmsCreateIntegration200Response = apiInstance.kmsUpdateIntegration(integrationId, kmsUpdateIntegrationRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IntegrationsApi#kmsUpdateIntegration")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IntegrationsApi#kmsUpdateIntegration")
    e.printStackTrace()
}
```

### Parameters
| **integrationId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsUpdateIntegrationRequest** | [**KmsUpdateIntegrationRequest**](KmsUpdateIntegrationRequest.md)|  | |

### Return type

[**KmsCreateIntegration200Response**](KmsCreateIntegration200Response.md)

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

