# NodeAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerAddNode**](NodeAPIApi.md#cloudApiControllerAddNode) | **POST** /v1/cloud/add-node | Api Controller Add Node |
| [**cloudApiControllerDeleteNode**](NodeAPIApi.md#cloudApiControllerDeleteNode) | **POST** /v1/cloud/delete-node | Api Controller Delete Node |
| [**cloudApiControllerGetNode**](NodeAPIApi.md#cloudApiControllerGetNode) | **GET** /v1/cloud/get-node | Api Controller Get Node |
| [**cloudApiControllerGetNodes**](NodeAPIApi.md#cloudApiControllerGetNodes) | **GET** /v1/cloud/get-nodes | Api Controller Get Nodes |
| [**cloudApiControllerUpdateNode**](NodeAPIApi.md#cloudApiControllerUpdateNode) | **POST** /v1/cloud/update-node | Api Controller Update Node |
| [**nexusAddNode**](NodeAPIApi.md#nexusAddNode) | **POST** /v1/nexus/add-node | add Node |
| [**nexusDeleteNode**](NodeAPIApi.md#nexusDeleteNode) | **POST** /v1/nexus/delete-node | delete Node |
| [**nexusGetNode**](NodeAPIApi.md#nexusGetNode) | **GET** /v1/nexus/get-node | get Node |
| [**nexusGetNodes**](NodeAPIApi.md#nexusGetNodes) | **GET** /v1/nexus/get-nodes | get Nodes |
| [**nexusUpdateNode**](NodeAPIApi.md#nexusUpdateNode) | **POST** /v1/nexus/update-node | update Node |


<a id="cloudApiControllerAddNode"></a>
# **cloudApiControllerAddNode**
> CloudControllersResponse cloudApiControllerAddNode(cloudObjectNode)

Api Controller Add Node

add a node

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NodeAPIApi()
val cloudObjectNode : CloudObjectNode =  // CloudObjectNode | The details of the node
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerAddNode(cloudObjectNode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NodeAPIApi#cloudApiControllerAddNode")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NodeAPIApi#cloudApiControllerAddNode")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectNode** | [**CloudObjectNode**](CloudObjectNode.md)| The details of the node | |

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

<a id="cloudApiControllerDeleteNode"></a>
# **cloudApiControllerDeleteNode**
> CloudControllersResponse cloudApiControllerDeleteNode(cloudObjectNode)

Api Controller Delete Node

delete a node

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NodeAPIApi()
val cloudObjectNode : CloudObjectNode =  // CloudObjectNode | The details of the node
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerDeleteNode(cloudObjectNode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NodeAPIApi#cloudApiControllerDeleteNode")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NodeAPIApi#cloudApiControllerDeleteNode")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectNode** | [**CloudObjectNode**](CloudObjectNode.md)| The details of the node | |

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

<a id="cloudApiControllerGetNode"></a>
# **cloudApiControllerGetNode**
> CloudObjectNode cloudApiControllerGetNode(id)

Api Controller Get Node

get node

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NodeAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the node
try {
    val result : CloudObjectNode = apiInstance.cloudApiControllerGetNode(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NodeAPIApi#cloudApiControllerGetNode")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NodeAPIApi#cloudApiControllerGetNode")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the node | |

### Return type

[**CloudObjectNode**](CloudObjectNode.md)

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

<a id="cloudApiControllerGetNodes"></a>
# **cloudApiControllerGetNodes**
> CloudObjectNode cloudApiControllerGetNodes(pageSize, p)

Api Controller Get Nodes

get all nodes

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NodeAPIApi()
val pageSize : kotlin.String = pageSize_example // kotlin.String | The size of each page
val p : kotlin.String = p_example // kotlin.String | The number of the page
try {
    val result : CloudObjectNode = apiInstance.cloudApiControllerGetNodes(pageSize, p)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NodeAPIApi#cloudApiControllerGetNodes")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NodeAPIApi#cloudApiControllerGetNodes")
    e.printStackTrace()
}
```

### Parameters
| **pageSize** | **kotlin.String**| The size of each page | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **p** | **kotlin.String**| The number of the page | |

### Return type

[**CloudObjectNode**](CloudObjectNode.md)

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

<a id="cloudApiControllerUpdateNode"></a>
# **cloudApiControllerUpdateNode**
> CloudControllersResponse cloudApiControllerUpdateNode(id, cloudObjectNode)

Api Controller Update Node

update node

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NodeAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the node
val cloudObjectNode : CloudObjectNode =  // CloudObjectNode | The details of the node
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerUpdateNode(id, cloudObjectNode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NodeAPIApi#cloudApiControllerUpdateNode")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NodeAPIApi#cloudApiControllerUpdateNode")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the node | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectNode** | [**CloudObjectNode**](CloudObjectNode.md)| The details of the node | |

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

<a id="nexusAddNode"></a>
# **nexusAddNode**
> NexusResponse nexusAddNode(nexusNode)

add Node

Add a node

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NodeAPIApi()
val nexusNode : NexusNode =  // NexusNode | The details of the node
try {
    val result : NexusResponse = apiInstance.nexusAddNode(nexusNode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NodeAPIApi#nexusAddNode")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NodeAPIApi#nexusAddNode")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusNode** | [**NexusNode**](NexusNode.md)| The details of the node | |

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

<a id="nexusDeleteNode"></a>
# **nexusDeleteNode**
> NexusResponse nexusDeleteNode(nexusNode)

delete Node

Delete a node

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NodeAPIApi()
val nexusNode : NexusNode =  // NexusNode | The details of the node
try {
    val result : NexusResponse = apiInstance.nexusDeleteNode(nexusNode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NodeAPIApi#nexusDeleteNode")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NodeAPIApi#nexusDeleteNode")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusNode** | [**NexusNode**](NexusNode.md)| The details of the node | |

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

<a id="nexusGetNode"></a>
# **nexusGetNode**
> NexusNode nexusGetNode(id)

get Node

Get a node

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NodeAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the node
try {
    val result : NexusNode = apiInstance.nexusGetNode(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NodeAPIApi#nexusGetNode")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NodeAPIApi#nexusGetNode")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id (owner/name) of the node | |

### Return type

[**NexusNode**](NexusNode.md)

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

<a id="nexusGetNodes"></a>
# **nexusGetNodes**
> NexusNode nexusGetNodes(pageSize, p)

get Nodes

Get all nodes

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NodeAPIApi()
val pageSize : kotlin.String = pageSize_example // kotlin.String | The size of each page
val p : kotlin.String = p_example // kotlin.String | The page number
try {
    val result : NexusNode = apiInstance.nexusGetNodes(pageSize, p)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NodeAPIApi#nexusGetNodes")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NodeAPIApi#nexusGetNodes")
    e.printStackTrace()
}
```

### Parameters
| **pageSize** | **kotlin.String**| The size of each page | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **p** | **kotlin.String**| The page number | |

### Return type

[**NexusNode**](NexusNode.md)

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

<a id="nexusUpdateNode"></a>
# **nexusUpdateNode**
> NexusResponse nexusUpdateNode(id, nexusNode)

update Node

Update a node

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NodeAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the node
val nexusNode : NexusNode =  // NexusNode | The details of the node
try {
    val result : NexusResponse = apiInstance.nexusUpdateNode(id, nexusNode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NodeAPIApi#nexusUpdateNode")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NodeAPIApi#nexusUpdateNode")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the node | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusNode** | [**NexusNode**](NexusNode.md)| The details of the node | |

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

