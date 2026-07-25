# ProvidersApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**iamApiControllerAddProvider**](ProvidersApi.md#iamApiControllerAddProvider) | **POST** /v1/iam/providers | Api Controller Add Provider |
| [**iamApiControllerDeleteProvider**](ProvidersApi.md#iamApiControllerDeleteProvider) | **DELETE** /v1/iam/providers/{id} | Api Controller Delete Provider |
| [**iamApiControllerGetGlobalProviders**](ProvidersApi.md#iamApiControllerGetGlobalProviders) | **GET** /v1/iam/global-providers | Api Controller Get Global Providers |
| [**iamApiControllerGetProvider**](ProvidersApi.md#iamApiControllerGetProvider) | **GET** /v1/iam/providers/{id} | Api Controller Get Provider |
| [**iamApiControllerGetProviders**](ProvidersApi.md#iamApiControllerGetProviders) | **GET** /v1/iam/providers | Api Controller Get Providers |
| [**iamApiControllerUpdateProvider**](ProvidersApi.md#iamApiControllerUpdateProvider) | **PUT** /v1/iam/providers/{id} | Api Controller Update Provider |
| [**integrationsGetProvider**](ProvidersApi.md#integrationsGetProvider) | **GET** /v1/integrations/{provider} | Get one provider with this org&#39;s connection status |
| [**integrationsListProviders**](ProvidersApi.md#integrationsListProviders) | **GET** /v1/integrations | List providers with this org&#39;s connection status |


<a id="iamApiControllerAddProvider"></a>
# **iamApiControllerAddProvider**
> IamControllersResponse iamApiControllerAddProvider(iamObjectProvider)

Api Controller Add Provider

add provider

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProvidersApi()
val iamObjectProvider : IamObjectProvider =  // IamObjectProvider | The details of the provider
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddProvider(iamObjectProvider)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProvidersApi#iamApiControllerAddProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProvidersApi#iamApiControllerAddProvider")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectProvider** | [**IamObjectProvider**](IamObjectProvider.md)| The details of the provider | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerDeleteProvider"></a>
# **iamApiControllerDeleteProvider**
> IamControllersResponse iamApiControllerDeleteProvider(id, iamObjectProvider)

Api Controller Delete Provider

delete provider

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProvidersApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectProvider : IamObjectProvider =  // IamObjectProvider | The details of the provider
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeleteProvider(id, iamObjectProvider)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProvidersApi#iamApiControllerDeleteProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProvidersApi#iamApiControllerDeleteProvider")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectProvider** | [**IamObjectProvider**](IamObjectProvider.md)| The details of the provider | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerGetGlobalProviders"></a>
# **iamApiControllerGetGlobalProviders**
> kotlin.collections.List&lt;IamObjectProvider&gt; iamApiControllerGetGlobalProviders()

Api Controller Get Global Providers

get Global providers

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProvidersApi()
try {
    val result : kotlin.collections.List<IamObjectProvider> = apiInstance.iamApiControllerGetGlobalProviders()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProvidersApi#iamApiControllerGetGlobalProviders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProvidersApi#iamApiControllerGetGlobalProviders")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;IamObjectProvider&gt;**](IamObjectProvider.md)

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

<a id="iamApiControllerGetProvider"></a>
# **iamApiControllerGetProvider**
> IamObjectProvider iamApiControllerGetProvider(id)

Api Controller Get Provider

get provider

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProvidersApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the provider
try {
    val result : IamObjectProvider = apiInstance.iamApiControllerGetProvider(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProvidersApi#iamApiControllerGetProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProvidersApi#iamApiControllerGetProvider")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the provider | |

### Return type

[**IamObjectProvider**](IamObjectProvider.md)

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

<a id="iamApiControllerGetProviders"></a>
# **iamApiControllerGetProviders**
> kotlin.collections.List&lt;IamObjectProvider&gt; iamApiControllerGetProviders(owner)

Api Controller Get Providers

get providers

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProvidersApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of providers
try {
    val result : kotlin.collections.List<IamObjectProvider> = apiInstance.iamApiControllerGetProviders(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProvidersApi#iamApiControllerGetProviders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProvidersApi#iamApiControllerGetProviders")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of providers | |

### Return type

[**kotlin.collections.List&lt;IamObjectProvider&gt;**](IamObjectProvider.md)

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

<a id="iamApiControllerUpdateProvider"></a>
# **iamApiControllerUpdateProvider**
> IamControllersResponse iamApiControllerUpdateProvider(id, iamObjectProvider)

Api Controller Update Provider

update provider

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProvidersApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the provider
val iamObjectProvider : IamObjectProvider =  // IamObjectProvider | The details of the provider
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdateProvider(id, iamObjectProvider)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProvidersApi#iamApiControllerUpdateProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProvidersApi#iamApiControllerUpdateProvider")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the provider | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectProvider** | [**IamObjectProvider**](IamObjectProvider.md)| The details of the provider | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="integrationsGetProvider"></a>
# **integrationsGetProvider**
> IntegrationsProviderView integrationsGetProvider(provider)

Get one provider with this org&#39;s connection status

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProvidersApi()
val provider : kotlin.String = provider_example // kotlin.String | Provider slug (e.g. slack, github)
try {
    val result : IntegrationsProviderView = apiInstance.integrationsGetProvider(provider)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProvidersApi#integrationsGetProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProvidersApi#integrationsGetProvider")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **provider** | **kotlin.String**| Provider slug (e.g. slack, github) | |

### Return type

[**IntegrationsProviderView**](IntegrationsProviderView.md)

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

<a id="integrationsListProviders"></a>
# **integrationsListProviders**
> IntegrationsListProviders200Response integrationsListProviders()

List providers with this org&#39;s connection status

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProvidersApi()
try {
    val result : IntegrationsListProviders200Response = apiInstance.integrationsListProviders()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProvidersApi#integrationsListProviders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProvidersApi#integrationsListProviders")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**IntegrationsListProviders200Response**](IntegrationsListProviders200Response.md)

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

