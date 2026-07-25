# StorageProviderAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerGetStorageProviders**](StorageProviderAPIApi.md#cloudApiControllerGetStorageProviders) | **GET** /v1/cloud/get-storage-providers | Api Controller Get Storage Providers |
| [**nexusGetStorageProviders**](StorageProviderAPIApi.md#nexusGetStorageProviders) | **GET** /v1/nexus/get-storage-providers | get Storage Providers |


<a id="cloudApiControllerGetStorageProviders"></a>
# **cloudApiControllerGetStorageProviders**
> kotlin.collections.List&lt;CloudObjectProvider&gt; cloudApiControllerGetStorageProviders()

Api Controller Get Storage Providers

get storage providers

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StorageProviderAPIApi()
try {
    val result : kotlin.collections.List<CloudObjectProvider> = apiInstance.cloudApiControllerGetStorageProviders()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StorageProviderAPIApi#cloudApiControllerGetStorageProviders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StorageProviderAPIApi#cloudApiControllerGetStorageProviders")
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

<a id="nexusGetStorageProviders"></a>
# **nexusGetStorageProviders**
> kotlin.collections.List&lt;NexusProvider&gt; nexusGetStorageProviders()

get Storage Providers

Get storage providers

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StorageProviderAPIApi()
try {
    val result : kotlin.collections.List<NexusProvider> = apiInstance.nexusGetStorageProviders()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StorageProviderAPIApi#nexusGetStorageProviders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StorageProviderAPIApi#nexusGetStorageProviders")
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

