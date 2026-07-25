# EmbeddingsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**gatewayCreateEmbedding**](EmbeddingsApi.md#gatewayCreateEmbedding) | **POST** /v1/gateway/embeddings | Create embeddings |


<a id="gatewayCreateEmbedding"></a>
# **gatewayCreateEmbedding**
> GatewayEmbeddingResponse gatewayCreateEmbedding(gatewayEmbeddingRequest)

Create embeddings

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EmbeddingsApi()
val gatewayEmbeddingRequest : GatewayEmbeddingRequest =  // GatewayEmbeddingRequest | 
try {
    val result : GatewayEmbeddingResponse = apiInstance.gatewayCreateEmbedding(gatewayEmbeddingRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EmbeddingsApi#gatewayCreateEmbedding")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EmbeddingsApi#gatewayCreateEmbedding")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **gatewayEmbeddingRequest** | [**GatewayEmbeddingRequest**](GatewayEmbeddingRequest.md)|  | |

### Return type

[**GatewayEmbeddingResponse**](GatewayEmbeddingResponse.md)

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

