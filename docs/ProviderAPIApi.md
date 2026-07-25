# ProviderAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerAddProvider**](ProviderAPIApi.md#cloudApiControllerAddProvider) | **POST** /v1/cloud/add-provider | Api Controller Add Provider |
| [**cloudApiControllerDeleteProvider**](ProviderAPIApi.md#cloudApiControllerDeleteProvider) | **POST** /v1/cloud/delete-provider | Api Controller Delete Provider |
| [**cloudApiControllerGetGlobalProviders**](ProviderAPIApi.md#cloudApiControllerGetGlobalProviders) | **GET** /v1/cloud/get-global-providers | Api Controller Get Global Providers |
| [**cloudApiControllerGetProvider**](ProviderAPIApi.md#cloudApiControllerGetProvider) | **GET** /v1/cloud/get-provider | Api Controller Get Provider |
| [**cloudApiControllerGetProviders**](ProviderAPIApi.md#cloudApiControllerGetProviders) | **GET** /v1/cloud/get-providers | Api Controller Get Providers |
| [**cloudApiControllerRefreshMcpTools**](ProviderAPIApi.md#cloudApiControllerRefreshMcpTools) | **POST** /v1/cloud/refresh-mcp-tools | Api Controller Refresh Mcp Tools |
| [**cloudApiControllerUpdateProvider**](ProviderAPIApi.md#cloudApiControllerUpdateProvider) | **POST** /v1/cloud/update-provider | Api Controller Update Provider |
| [**nexusAddProvider**](ProviderAPIApi.md#nexusAddProvider) | **POST** /v1/nexus/add-provider | add Provider |
| [**nexusDeleteProvider**](ProviderAPIApi.md#nexusDeleteProvider) | **POST** /v1/nexus/delete-provider | delete Provider |
| [**nexusGetGlobalProviders**](ProviderAPIApi.md#nexusGetGlobalProviders) | **GET** /v1/nexus/get-global-providers | get Global Providers |
| [**nexusGetProvider**](ProviderAPIApi.md#nexusGetProvider) | **GET** /v1/nexus/get-provider | get Provider |
| [**nexusGetProviders**](ProviderAPIApi.md#nexusGetProviders) | **GET** /v1/nexus/get-providers | get Providers |
| [**nexusRefreshMcpTools**](ProviderAPIApi.md#nexusRefreshMcpTools) | **POST** /v1/nexus/refresh-mcp-tools | refresh Mcp Tools |
| [**nexusUpdateProvider**](ProviderAPIApi.md#nexusUpdateProvider) | **POST** /v1/nexus/update-provider | update Provider |


<a id="cloudApiControllerAddProvider"></a>
# **cloudApiControllerAddProvider**
> CloudControllersResponse cloudApiControllerAddProvider(cloudObjectProvider)

Api Controller Add Provider

add provider

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProviderAPIApi()
val cloudObjectProvider : CloudObjectProvider =  // CloudObjectProvider | The details of the provider
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerAddProvider(cloudObjectProvider)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProviderAPIApi#cloudApiControllerAddProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProviderAPIApi#cloudApiControllerAddProvider")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectProvider** | [**CloudObjectProvider**](CloudObjectProvider.md)| The details of the provider | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="cloudApiControllerDeleteProvider"></a>
# **cloudApiControllerDeleteProvider**
> CloudControllersResponse cloudApiControllerDeleteProvider(cloudObjectProvider)

Api Controller Delete Provider

delete provider

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProviderAPIApi()
val cloudObjectProvider : CloudObjectProvider =  // CloudObjectProvider | The details of the provider
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerDeleteProvider(cloudObjectProvider)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProviderAPIApi#cloudApiControllerDeleteProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProviderAPIApi#cloudApiControllerDeleteProvider")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectProvider** | [**CloudObjectProvider**](CloudObjectProvider.md)| The details of the provider | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="cloudApiControllerGetGlobalProviders"></a>
# **cloudApiControllerGetGlobalProviders**
> kotlin.collections.List&lt;CloudObjectProvider&gt; cloudApiControllerGetGlobalProviders()

Api Controller Get Global Providers

get global providers

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProviderAPIApi()
try {
    val result : kotlin.collections.List<CloudObjectProvider> = apiInstance.cloudApiControllerGetGlobalProviders()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProviderAPIApi#cloudApiControllerGetGlobalProviders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProviderAPIApi#cloudApiControllerGetGlobalProviders")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;CloudObjectProvider&gt;**](CloudObjectProvider.md)

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

<a id="cloudApiControllerGetProvider"></a>
# **cloudApiControllerGetProvider**
> CloudObjectProvider cloudApiControllerGetProvider(id)

Api Controller Get Provider

get provider

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProviderAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id of provider
try {
    val result : CloudObjectProvider = apiInstance.cloudApiControllerGetProvider(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProviderAPIApi#cloudApiControllerGetProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProviderAPIApi#cloudApiControllerGetProvider")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id of provider | |

### Return type

[**CloudObjectProvider**](CloudObjectProvider.md)

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

<a id="cloudApiControllerGetProviders"></a>
# **cloudApiControllerGetProviders**
> kotlin.collections.List&lt;CloudObjectProvider&gt; cloudApiControllerGetProviders()

Api Controller Get Providers

get providers

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProviderAPIApi()
try {
    val result : kotlin.collections.List<CloudObjectProvider> = apiInstance.cloudApiControllerGetProviders()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProviderAPIApi#cloudApiControllerGetProviders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProviderAPIApi#cloudApiControllerGetProviders")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;CloudObjectProvider&gt;**](CloudObjectProvider.md)

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

<a id="cloudApiControllerRefreshMcpTools"></a>
# **cloudApiControllerRefreshMcpTools**
> CloudControllersResponse cloudApiControllerRefreshMcpTools(cloudObjectProvider)

Api Controller Refresh Mcp Tools

refresh Mcp tools

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProviderAPIApi()
val cloudObjectProvider : CloudObjectProvider =  // CloudObjectProvider | The details of the provider
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerRefreshMcpTools(cloudObjectProvider)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProviderAPIApi#cloudApiControllerRefreshMcpTools")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProviderAPIApi#cloudApiControllerRefreshMcpTools")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectProvider** | [**CloudObjectProvider**](CloudObjectProvider.md)| The details of the provider | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="cloudApiControllerUpdateProvider"></a>
# **cloudApiControllerUpdateProvider**
> CloudControllersResponse cloudApiControllerUpdateProvider(id, cloudObjectProvider)

Api Controller Update Provider

update provider

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProviderAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the provider
val cloudObjectProvider : CloudObjectProvider =  // CloudObjectProvider | The details of the provider
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerUpdateProvider(id, cloudObjectProvider)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProviderAPIApi#cloudApiControllerUpdateProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProviderAPIApi#cloudApiControllerUpdateProvider")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the provider | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectProvider** | [**CloudObjectProvider**](CloudObjectProvider.md)| The details of the provider | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="nexusAddProvider"></a>
# **nexusAddProvider**
> NexusResponse nexusAddProvider(nexusProvider)

add Provider

Add a provider

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProviderAPIApi()
val nexusProvider : NexusProvider =  // NexusProvider | The details of the provider
try {
    val result : NexusResponse = apiInstance.nexusAddProvider(nexusProvider)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProviderAPIApi#nexusAddProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProviderAPIApi#nexusAddProvider")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusProvider** | [**NexusProvider**](NexusProvider.md)| The details of the provider | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

<a id="nexusDeleteProvider"></a>
# **nexusDeleteProvider**
> NexusResponse nexusDeleteProvider(nexusProvider)

delete Provider

Delete a provider

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProviderAPIApi()
val nexusProvider : NexusProvider =  // NexusProvider | The details of the provider
try {
    val result : NexusResponse = apiInstance.nexusDeleteProvider(nexusProvider)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProviderAPIApi#nexusDeleteProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProviderAPIApi#nexusDeleteProvider")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusProvider** | [**NexusProvider**](NexusProvider.md)| The details of the provider | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

<a id="nexusGetGlobalProviders"></a>
# **nexusGetGlobalProviders**
> kotlin.collections.List&lt;NexusProvider&gt; nexusGetGlobalProviders()

get Global Providers

Get global providers

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProviderAPIApi()
try {
    val result : kotlin.collections.List<NexusProvider> = apiInstance.nexusGetGlobalProviders()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProviderAPIApi#nexusGetGlobalProviders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProviderAPIApi#nexusGetGlobalProviders")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;NexusProvider&gt;**](NexusProvider.md)

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

<a id="nexusGetProvider"></a>
# **nexusGetProvider**
> NexusProvider nexusGetProvider(id)

get Provider

Get a provider

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProviderAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id of the provider
try {
    val result : NexusProvider = apiInstance.nexusGetProvider(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProviderAPIApi#nexusGetProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProviderAPIApi#nexusGetProvider")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id of the provider | |

### Return type

[**NexusProvider**](NexusProvider.md)

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

<a id="nexusGetProviders"></a>
# **nexusGetProviders**
> kotlin.collections.List&lt;NexusProvider&gt; nexusGetProviders()

get Providers

Get providers

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProviderAPIApi()
try {
    val result : kotlin.collections.List<NexusProvider> = apiInstance.nexusGetProviders()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProviderAPIApi#nexusGetProviders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProviderAPIApi#nexusGetProviders")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;NexusProvider&gt;**](NexusProvider.md)

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

<a id="nexusRefreshMcpTools"></a>
# **nexusRefreshMcpTools**
> NexusResponse nexusRefreshMcpTools(nexusProvider)

refresh Mcp Tools

Refresh MCP tools for a provider

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProviderAPIApi()
val nexusProvider : NexusProvider =  // NexusProvider | The details of the provider
try {
    val result : NexusResponse = apiInstance.nexusRefreshMcpTools(nexusProvider)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProviderAPIApi#nexusRefreshMcpTools")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProviderAPIApi#nexusRefreshMcpTools")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusProvider** | [**NexusProvider**](NexusProvider.md)| The details of the provider | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

<a id="nexusUpdateProvider"></a>
# **nexusUpdateProvider**
> NexusResponse nexusUpdateProvider(id, nexusProvider)

update Provider

Update a provider

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProviderAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the provider
val nexusProvider : NexusProvider =  // NexusProvider | The details of the provider
try {
    val result : NexusResponse = apiInstance.nexusUpdateProvider(id, nexusProvider)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProviderAPIApi#nexusUpdateProvider")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProviderAPIApi#nexusUpdateProvider")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the provider | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusProvider** | [**NexusProvider**](NexusProvider.md)| The details of the provider | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

