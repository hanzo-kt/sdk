# ObjectStoreApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**mqCreateObjectStore**](ObjectStoreApi.md#mqCreateObjectStore) | **POST** /v1/mq/objects | Create object store |
| [**mqDeleteObject**](ObjectStoreApi.md#mqDeleteObject) | **DELETE** /v1/mq/objects/{store}/{name} | Delete object |
| [**mqDeleteObjectStore**](ObjectStoreApi.md#mqDeleteObjectStore) | **DELETE** /v1/mq/objects/{store} | Delete object store |
| [**mqGetObject**](ObjectStoreApi.md#mqGetObject) | **GET** /v1/mq/objects/{store}/{name} | Download object |
| [**mqGetObjectStore**](ObjectStoreApi.md#mqGetObjectStore) | **GET** /v1/mq/objects/{store} | Get store info |
| [**mqListObjectStores**](ObjectStoreApi.md#mqListObjectStores) | **GET** /v1/mq/objects | List object stores |
| [**mqListObjects**](ObjectStoreApi.md#mqListObjects) | **GET** /v1/mq/objects/{store}/list | List objects in store |
| [**mqPutObject**](ObjectStoreApi.md#mqPutObject) | **PUT** /v1/mq/objects/{store}/{name} | Upload object |
| [**pubsubDeleteObject**](ObjectStoreApi.md#pubsubDeleteObject) | **DELETE** /v1/pubsub/objects/{bucket}/{name} | Delete an object |
| [**pubsubGetObject**](ObjectStoreApi.md#pubsubGetObject) | **GET** /v1/pubsub/objects/{bucket}/{name} | Download an object |
| [**pubsubListObjects**](ObjectStoreApi.md#pubsubListObjects) | **GET** /v1/pubsub/objects/{bucket} | List objects in a bucket |
| [**pubsubPutObject**](ObjectStoreApi.md#pubsubPutObject) | **PUT** /v1/pubsub/objects/{bucket}/{name} | Upload an object |


<a id="mqCreateObjectStore"></a>
# **mqCreateObjectStore**
> MqObjectStoreInfo mqCreateObjectStore(mqObjectStoreConfig)

Create object store

Creates a new object store backed by JetStream. Large objects are automatically chunked and stored across the stream. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ObjectStoreApi()
val mqObjectStoreConfig : MqObjectStoreConfig =  // MqObjectStoreConfig | 
try {
    val result : MqObjectStoreInfo = apiInstance.mqCreateObjectStore(mqObjectStoreConfig)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ObjectStoreApi#mqCreateObjectStore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ObjectStoreApi#mqCreateObjectStore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **mqObjectStoreConfig** | [**MqObjectStoreConfig**](MqObjectStoreConfig.md)|  | |

### Return type

[**MqObjectStoreInfo**](MqObjectStoreInfo.md)

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

<a id="mqDeleteObject"></a>
# **mqDeleteObject**
> mqDeleteObject(store, name)

Delete object

Deletes the object and its chunks from the store.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ObjectStoreApi()
val store : kotlin.String = store_example // kotlin.String | Object store name.
val name : kotlin.String = name_example // kotlin.String | Object name.
try {
    apiInstance.mqDeleteObject(store, name)
} catch (e: ClientException) {
    println("4xx response calling ObjectStoreApi#mqDeleteObject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ObjectStoreApi#mqDeleteObject")
    e.printStackTrace()
}
```

### Parameters
| **store** | **kotlin.String**| Object store name. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**| Object name. | |

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
 - **Accept**: application/json

<a id="mqDeleteObjectStore"></a>
# **mqDeleteObjectStore**
> mqDeleteObjectStore(store)

Delete object store

Deletes the store and all objects. Irreversible.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ObjectStoreApi()
val store : kotlin.String = store_example // kotlin.String | Object store name.
try {
    apiInstance.mqDeleteObjectStore(store)
} catch (e: ClientException) {
    println("4xx response calling ObjectStoreApi#mqDeleteObjectStore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ObjectStoreApi#mqDeleteObjectStore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **store** | **kotlin.String**| Object store name. | |

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
 - **Accept**: application/json

<a id="mqGetObject"></a>
# **mqGetObject**
> java.io.File mqGetObject(store, name)

Download object

Downloads the object as a binary stream. Chunks are reassembled transparently. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ObjectStoreApi()
val store : kotlin.String = store_example // kotlin.String | Object store name.
val name : kotlin.String = name_example // kotlin.String | Object name.
try {
    val result : java.io.File = apiInstance.mqGetObject(store, name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ObjectStoreApi#mqGetObject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ObjectStoreApi#mqGetObject")
    e.printStackTrace()
}
```

### Parameters
| **store** | **kotlin.String**| Object store name. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**| Object name. | |

### Return type

[**java.io.File**](java.io.File.md)

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
 - **Accept**: application/octet-stream, application/json

<a id="mqGetObjectStore"></a>
# **mqGetObjectStore**
> MqObjectStoreInfo mqGetObjectStore(store)

Get store info

Returns object store configuration and state.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ObjectStoreApi()
val store : kotlin.String = store_example // kotlin.String | Object store name.
try {
    val result : MqObjectStoreInfo = apiInstance.mqGetObjectStore(store)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ObjectStoreApi#mqGetObjectStore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ObjectStoreApi#mqGetObjectStore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **store** | **kotlin.String**| Object store name. | |

### Return type

[**MqObjectStoreInfo**](MqObjectStoreInfo.md)

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

<a id="mqListObjectStores"></a>
# **mqListObjectStores**
> MqListObjectStores200Response mqListObjectStores(limit, offset)

List object stores

Returns all object stores for the authenticated account.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ObjectStoreApi()
val limit : kotlin.Int = 56 // kotlin.Int | Maximum number of items to return.
val offset : kotlin.Int = 56 // kotlin.Int | Number of items to skip.
try {
    val result : MqListObjectStores200Response = apiInstance.mqListObjectStores(limit, offset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ObjectStoreApi#mqListObjectStores")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ObjectStoreApi#mqListObjectStores")
    e.printStackTrace()
}
```

### Parameters
| **limit** | **kotlin.Int**| Maximum number of items to return. | [optional] [default to 100] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **offset** | **kotlin.Int**| Number of items to skip. | [optional] [default to 0] |

### Return type

[**MqListObjectStores200Response**](MqListObjectStores200Response.md)

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

<a id="mqListObjects"></a>
# **mqListObjects**
> MqListObjects200Response mqListObjects(store, limit, offset)

List objects in store

Returns metadata for all objects in the store.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ObjectStoreApi()
val store : kotlin.String = store_example // kotlin.String | Object store name.
val limit : kotlin.Int = 56 // kotlin.Int | Maximum number of items to return.
val offset : kotlin.Int = 56 // kotlin.Int | Number of items to skip.
try {
    val result : MqListObjects200Response = apiInstance.mqListObjects(store, limit, offset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ObjectStoreApi#mqListObjects")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ObjectStoreApi#mqListObjects")
    e.printStackTrace()
}
```

### Parameters
| **store** | **kotlin.String**| Object store name. | |
| **limit** | **kotlin.Int**| Maximum number of items to return. | [optional] [default to 100] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **offset** | **kotlin.Int**| Number of items to skip. | [optional] [default to 0] |

### Return type

[**MqListObjects200Response**](MqListObjects200Response.md)

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

<a id="mqPutObject"></a>
# **mqPutObject**
> MqObjectInfo mqPutObject(store, name, body, xMQObjectDescription)

Upload object

Uploads an object to the store. The object is automatically chunked for storage. Use multipart/form-data for file uploads or application/octet-stream for raw binary. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ObjectStoreApi()
val store : kotlin.String = store_example // kotlin.String | Object store name.
val name : kotlin.String = name_example // kotlin.String | Object name.
val body : java.io.File = BINARY_DATA_HERE // java.io.File | 
val xMQObjectDescription : kotlin.String = xMQObjectDescription_example // kotlin.String | Optional description for the object.
try {
    val result : MqObjectInfo = apiInstance.mqPutObject(store, name, body, xMQObjectDescription)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ObjectStoreApi#mqPutObject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ObjectStoreApi#mqPutObject")
    e.printStackTrace()
}
```

### Parameters
| **store** | **kotlin.String**| Object store name. | |
| **name** | **kotlin.String**| Object name. | |
| **body** | **java.io.File**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **xMQObjectDescription** | **kotlin.String**| Optional description for the object. | [optional] |

### Return type

[**MqObjectInfo**](MqObjectInfo.md)

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

 - **Content-Type**: application/octet-stream
 - **Accept**: application/json

<a id="pubsubDeleteObject"></a>
# **pubsubDeleteObject**
> pubsubDeleteObject(bucket, name)

Delete an object

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ObjectStoreApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
try {
    apiInstance.pubsubDeleteObject(bucket, name)
} catch (e: ClientException) {
    println("4xx response calling ObjectStoreApi#pubsubDeleteObject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ObjectStoreApi#pubsubDeleteObject")
    e.printStackTrace()
}
```

### Parameters
| **bucket** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | |

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

<a id="pubsubGetObject"></a>
# **pubsubGetObject**
> java.io.File pubsubGetObject(bucket, name)

Download an object

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ObjectStoreApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
try {
    val result : java.io.File = apiInstance.pubsubGetObject(bucket, name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ObjectStoreApi#pubsubGetObject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ObjectStoreApi#pubsubGetObject")
    e.printStackTrace()
}
```

### Parameters
| **bucket** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | |

### Return type

[**java.io.File**](java.io.File.md)

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
 - **Accept**: application/octet-stream

<a id="pubsubListObjects"></a>
# **pubsubListObjects**
> PubsubListObjects200Response pubsubListObjects(bucket)

List objects in a bucket

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ObjectStoreApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
try {
    val result : PubsubListObjects200Response = apiInstance.pubsubListObjects(bucket)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ObjectStoreApi#pubsubListObjects")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ObjectStoreApi#pubsubListObjects")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **bucket** | **kotlin.String**|  | |

### Return type

[**PubsubListObjects200Response**](PubsubListObjects200Response.md)

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

<a id="pubsubPutObject"></a>
# **pubsubPutObject**
> PubsubObjectMeta pubsubPutObject(bucket, name, body, description)

Upload an object

Upload a large object with automatic chunking and SHA-256 integrity.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ObjectStoreApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val body : java.io.File = BINARY_DATA_HERE // java.io.File | 
val description : kotlin.String = description_example // kotlin.String | 
try {
    val result : PubsubObjectMeta = apiInstance.pubsubPutObject(bucket, name, body, description)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ObjectStoreApi#pubsubPutObject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ObjectStoreApi#pubsubPutObject")
    e.printStackTrace()
}
```

### Parameters
| **bucket** | **kotlin.String**|  | |
| **name** | **kotlin.String**|  | |
| **body** | **java.io.File**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **description** | **kotlin.String**|  | [optional] |

### Return type

[**PubsubObjectMeta**](PubsubObjectMeta.md)

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

 - **Content-Type**: application/octet-stream
 - **Accept**: application/json

