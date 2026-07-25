# KeyValueApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**mqCreateKVBucket**](KeyValueApi.md#mqCreateKVBucket) | **POST** /v1/mq/kv | Create KV bucket |
| [**mqDeleteKVBucket**](KeyValueApi.md#mqDeleteKVBucket) | **DELETE** /v1/mq/kv/{bucket} | Delete bucket |
| [**mqDeleteKVEntry**](KeyValueApi.md#mqDeleteKVEntry) | **DELETE** /v1/mq/kv/{bucket}/{key} | Delete key |
| [**mqGetKVBucket**](KeyValueApi.md#mqGetKVBucket) | **GET** /v1/mq/kv/{bucket} | Get bucket info |
| [**mqGetKVEntry**](KeyValueApi.md#mqGetKVEntry) | **GET** /v1/mq/kv/{bucket}/{key} | Get value |
| [**mqGetKVHistory**](KeyValueApi.md#mqGetKVHistory) | **GET** /v1/mq/kv/{bucket}/{key}/history | Get key history |
| [**mqListKVBuckets**](KeyValueApi.md#mqListKVBuckets) | **GET** /v1/mq/kv | List KV buckets |
| [**mqListKVKeys**](KeyValueApi.md#mqListKVKeys) | **GET** /v1/mq/kv/{bucket}/keys | List keys in bucket |
| [**mqPutKVEntry**](KeyValueApi.md#mqPutKVEntry) | **PUT** /v1/mq/kv/{bucket}/{key} | Put value |
| [**mqWatchKVBucket**](KeyValueApi.md#mqWatchKVBucket) | **GET** /v1/mq/kv/{bucket}/watch | Watch bucket changes via SSE |
| [**pubsubCreateKVBucket**](KeyValueApi.md#pubsubCreateKVBucket) | **POST** /v1/pubsub/kv/{bucket} | Create a KV bucket |
| [**pubsubDeleteKVBucket**](KeyValueApi.md#pubsubDeleteKVBucket) | **DELETE** /v1/pubsub/kv/{bucket} | Delete a KV bucket |
| [**pubsubKvDelete**](KeyValueApi.md#pubsubKvDelete) | **DELETE** /v1/pubsub/kv/{bucket}/{key} | Delete a key |
| [**pubsubKvGet**](KeyValueApi.md#pubsubKvGet) | **GET** /v1/pubsub/kv/{bucket}/{key} | Get a value |
| [**pubsubKvHistory**](KeyValueApi.md#pubsubKvHistory) | **GET** /v1/pubsub/kv/{bucket}/{key}/history | Get key history |
| [**pubsubKvPut**](KeyValueApi.md#pubsubKvPut) | **PUT** /v1/pubsub/kv/{bucket}/{key} | Set a value |


<a id="mqCreateKVBucket"></a>
# **mqCreateKVBucket**
> MqKVBucket mqCreateKVBucket(mqKVBucketConfig)

Create KV bucket

Creates a new key-value bucket backed by a JetStream stream. Supports configurable history depth, TTL, and replication. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeyValueApi()
val mqKVBucketConfig : MqKVBucketConfig =  // MqKVBucketConfig | 
try {
    val result : MqKVBucket = apiInstance.mqCreateKVBucket(mqKVBucketConfig)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeyValueApi#mqCreateKVBucket")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeyValueApi#mqCreateKVBucket")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **mqKVBucketConfig** | [**MqKVBucketConfig**](MqKVBucketConfig.md)|  | |

### Return type

[**MqKVBucket**](MqKVBucket.md)

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

<a id="mqDeleteKVBucket"></a>
# **mqDeleteKVBucket**
> mqDeleteKVBucket(bucket)

Delete bucket

Deletes the bucket and all its keys. Irreversible.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeyValueApi()
val bucket : kotlin.String = bucket_example // kotlin.String | KV bucket name.
try {
    apiInstance.mqDeleteKVBucket(bucket)
} catch (e: ClientException) {
    println("4xx response calling KeyValueApi#mqDeleteKVBucket")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeyValueApi#mqDeleteKVBucket")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **bucket** | **kotlin.String**| KV bucket name. | |

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

<a id="mqDeleteKVEntry"></a>
# **mqDeleteKVEntry**
> mqDeleteKVEntry(bucket, key)

Delete key

Deletes the key by writing a tombstone marker. The key&#39;s history is preserved according to the bucket&#39;s history setting. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeyValueApi()
val bucket : kotlin.String = bucket_example // kotlin.String | KV bucket name.
val key : kotlin.String = key_example // kotlin.String | Key name (supports dotted hierarchy).
try {
    apiInstance.mqDeleteKVEntry(bucket, key)
} catch (e: ClientException) {
    println("4xx response calling KeyValueApi#mqDeleteKVEntry")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeyValueApi#mqDeleteKVEntry")
    e.printStackTrace()
}
```

### Parameters
| **bucket** | **kotlin.String**| KV bucket name. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key** | **kotlin.String**| Key name (supports dotted hierarchy). | |

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

<a id="mqGetKVBucket"></a>
# **mqGetKVBucket**
> MqKVBucket mqGetKVBucket(bucket)

Get bucket info

Returns bucket configuration and current state.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeyValueApi()
val bucket : kotlin.String = bucket_example // kotlin.String | KV bucket name.
try {
    val result : MqKVBucket = apiInstance.mqGetKVBucket(bucket)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeyValueApi#mqGetKVBucket")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeyValueApi#mqGetKVBucket")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **bucket** | **kotlin.String**| KV bucket name. | |

### Return type

[**MqKVBucket**](MqKVBucket.md)

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

<a id="mqGetKVEntry"></a>
# **mqGetKVEntry**
> MqKVEntry mqGetKVEntry(bucket, key)

Get value

Returns the current value for the key. The revision number is included in the X-MQ-Revision response header. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeyValueApi()
val bucket : kotlin.String = bucket_example // kotlin.String | KV bucket name.
val key : kotlin.String = key_example // kotlin.String | Key name (supports dotted hierarchy).
try {
    val result : MqKVEntry = apiInstance.mqGetKVEntry(bucket, key)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeyValueApi#mqGetKVEntry")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeyValueApi#mqGetKVEntry")
    e.printStackTrace()
}
```

### Parameters
| **bucket** | **kotlin.String**| KV bucket name. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key** | **kotlin.String**| Key name (supports dotted hierarchy). | |

### Return type

[**MqKVEntry**](MqKVEntry.md)

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

<a id="mqGetKVHistory"></a>
# **mqGetKVHistory**
> MqGetKVHistory200Response mqGetKVHistory(bucket, key)

Get key history

Returns all revisions of the key, from oldest to newest. The number of revisions kept is determined by the bucket&#39;s history setting. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeyValueApi()
val bucket : kotlin.String = bucket_example // kotlin.String | KV bucket name.
val key : kotlin.String = key_example // kotlin.String | Key name (supports dotted hierarchy).
try {
    val result : MqGetKVHistory200Response = apiInstance.mqGetKVHistory(bucket, key)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeyValueApi#mqGetKVHistory")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeyValueApi#mqGetKVHistory")
    e.printStackTrace()
}
```

### Parameters
| **bucket** | **kotlin.String**| KV bucket name. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key** | **kotlin.String**| Key name (supports dotted hierarchy). | |

### Return type

[**MqGetKVHistory200Response**](MqGetKVHistory200Response.md)

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

<a id="mqListKVBuckets"></a>
# **mqListKVBuckets**
> MqListKVBuckets200Response mqListKVBuckets(limit, offset)

List KV buckets

Returns all key-value buckets for the authenticated account.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeyValueApi()
val limit : kotlin.Int = 56 // kotlin.Int | Maximum number of items to return.
val offset : kotlin.Int = 56 // kotlin.Int | Number of items to skip.
try {
    val result : MqListKVBuckets200Response = apiInstance.mqListKVBuckets(limit, offset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeyValueApi#mqListKVBuckets")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeyValueApi#mqListKVBuckets")
    e.printStackTrace()
}
```

### Parameters
| **limit** | **kotlin.Int**| Maximum number of items to return. | [optional] [default to 100] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **offset** | **kotlin.Int**| Number of items to skip. | [optional] [default to 0] |

### Return type

[**MqListKVBuckets200Response**](MqListKVBuckets200Response.md)

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

<a id="mqListKVKeys"></a>
# **mqListKVKeys**
> MqListKVKeys200Response mqListKVKeys(bucket, filter, limit, offset)

List keys in bucket

Returns all keys in the bucket, optionally filtered by pattern.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeyValueApi()
val bucket : kotlin.String = bucket_example // kotlin.String | KV bucket name.
val filter : kotlin.String = filter_example // kotlin.String | Key filter pattern (supports wildcards).
val limit : kotlin.Int = 56 // kotlin.Int | Maximum number of items to return.
val offset : kotlin.Int = 56 // kotlin.Int | Number of items to skip.
try {
    val result : MqListKVKeys200Response = apiInstance.mqListKVKeys(bucket, filter, limit, offset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeyValueApi#mqListKVKeys")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeyValueApi#mqListKVKeys")
    e.printStackTrace()
}
```

### Parameters
| **bucket** | **kotlin.String**| KV bucket name. | |
| **filter** | **kotlin.String**| Key filter pattern (supports wildcards). | [optional] |
| **limit** | **kotlin.Int**| Maximum number of items to return. | [optional] [default to 100] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **offset** | **kotlin.Int**| Number of items to skip. | [optional] [default to 0] |

### Return type

[**MqListKVKeys200Response**](MqListKVKeys200Response.md)

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

<a id="mqPutKVEntry"></a>
# **mqPutKVEntry**
> MqPutKVEntry200Response mqPutKVEntry(bucket, key, mqPutKVEntryRequest, xMQExpectedRevision)

Put value

Sets the value for the key. Returns the new revision number. Use the X-MQ-Expected-Revision header for optimistic concurrency (CAS operation). 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeyValueApi()
val bucket : kotlin.String = bucket_example // kotlin.String | KV bucket name.
val key : kotlin.String = key_example // kotlin.String | Key name (supports dotted hierarchy).
val mqPutKVEntryRequest : MqPutKVEntryRequest =  // MqPutKVEntryRequest | 
val xMQExpectedRevision : kotlin.Int = 56 // kotlin.Int | Expected current revision for CAS. The put fails with 409 if the current revision does not match. 
try {
    val result : MqPutKVEntry200Response = apiInstance.mqPutKVEntry(bucket, key, mqPutKVEntryRequest, xMQExpectedRevision)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeyValueApi#mqPutKVEntry")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeyValueApi#mqPutKVEntry")
    e.printStackTrace()
}
```

### Parameters
| **bucket** | **kotlin.String**| KV bucket name. | |
| **key** | **kotlin.String**| Key name (supports dotted hierarchy). | |
| **mqPutKVEntryRequest** | [**MqPutKVEntryRequest**](MqPutKVEntryRequest.md)|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **xMQExpectedRevision** | **kotlin.Int**| Expected current revision for CAS. The put fails with 409 if the current revision does not match.  | [optional] |

### Return type

[**MqPutKVEntry200Response**](MqPutKVEntry200Response.md)

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

<a id="mqWatchKVBucket"></a>
# **mqWatchKVBucket**
> MqKVEntry mqWatchKVBucket(bucket, key, includeHistory)

Watch bucket changes via SSE

Opens a Server-Sent Events stream that emits KVEntry events for every change in the bucket. Optionally filter by key pattern. Delivers initial values followed by real-time updates. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeyValueApi()
val bucket : kotlin.String = bucket_example // kotlin.String | KV bucket name.
val key : kotlin.String = key_example // kotlin.String | Key pattern filter (supports wildcards).
val includeHistory : kotlin.Boolean = true // kotlin.Boolean | Include all historical revisions before live updates.
try {
    val result : MqKVEntry = apiInstance.mqWatchKVBucket(bucket, key, includeHistory)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeyValueApi#mqWatchKVBucket")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeyValueApi#mqWatchKVBucket")
    e.printStackTrace()
}
```

### Parameters
| **bucket** | **kotlin.String**| KV bucket name. | |
| **key** | **kotlin.String**| Key pattern filter (supports wildcards). | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **includeHistory** | **kotlin.Boolean**| Include all historical revisions before live updates. | [optional] [default to false] |

### Return type

[**MqKVEntry**](MqKVEntry.md)

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

<a id="pubsubCreateKVBucket"></a>
# **pubsubCreateKVBucket**
> pubsubCreateKVBucket(bucket, pubsubKVBucketConfig)

Create a KV bucket

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeyValueApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
val pubsubKVBucketConfig : PubsubKVBucketConfig =  // PubsubKVBucketConfig | 
try {
    apiInstance.pubsubCreateKVBucket(bucket, pubsubKVBucketConfig)
} catch (e: ClientException) {
    println("4xx response calling KeyValueApi#pubsubCreateKVBucket")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeyValueApi#pubsubCreateKVBucket")
    e.printStackTrace()
}
```

### Parameters
| **bucket** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **pubsubKVBucketConfig** | [**PubsubKVBucketConfig**](PubsubKVBucketConfig.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="pubsubDeleteKVBucket"></a>
# **pubsubDeleteKVBucket**
> pubsubDeleteKVBucket(bucket)

Delete a KV bucket

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeyValueApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
try {
    apiInstance.pubsubDeleteKVBucket(bucket)
} catch (e: ClientException) {
    println("4xx response calling KeyValueApi#pubsubDeleteKVBucket")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeyValueApi#pubsubDeleteKVBucket")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **bucket** | **kotlin.String**|  | |

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

<a id="pubsubKvDelete"></a>
# **pubsubKvDelete**
> pubsubKvDelete(bucket, key)

Delete a key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeyValueApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
val key : kotlin.String = key_example // kotlin.String | 
try {
    apiInstance.pubsubKvDelete(bucket, key)
} catch (e: ClientException) {
    println("4xx response calling KeyValueApi#pubsubKvDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeyValueApi#pubsubKvDelete")
    e.printStackTrace()
}
```

### Parameters
| **bucket** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key** | **kotlin.String**|  | |

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

<a id="pubsubKvGet"></a>
# **pubsubKvGet**
> PubsubKVEntry pubsubKvGet(bucket, key, revision)

Get a value

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeyValueApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
val key : kotlin.String = key_example // kotlin.String | 
val revision : kotlin.Int = 56 // kotlin.Int | Specific revision to retrieve
try {
    val result : PubsubKVEntry = apiInstance.pubsubKvGet(bucket, key, revision)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeyValueApi#pubsubKvGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeyValueApi#pubsubKvGet")
    e.printStackTrace()
}
```

### Parameters
| **bucket** | **kotlin.String**|  | |
| **key** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **revision** | **kotlin.Int**| Specific revision to retrieve | [optional] |

### Return type

[**PubsubKVEntry**](PubsubKVEntry.md)

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

<a id="pubsubKvHistory"></a>
# **pubsubKvHistory**
> PubsubKvHistory200Response pubsubKvHistory(bucket, key)

Get key history

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeyValueApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
val key : kotlin.String = key_example // kotlin.String | 
try {
    val result : PubsubKvHistory200Response = apiInstance.pubsubKvHistory(bucket, key)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeyValueApi#pubsubKvHistory")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeyValueApi#pubsubKvHistory")
    e.printStackTrace()
}
```

### Parameters
| **bucket** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key** | **kotlin.String**|  | |

### Return type

[**PubsubKvHistory200Response**](PubsubKvHistory200Response.md)

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

<a id="pubsubKvPut"></a>
# **pubsubKvPut**
> PubsubKvPut200Response pubsubKvPut(bucket, key, body)

Set a value

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KeyValueApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
val key : kotlin.String = key_example // kotlin.String | 
val body : java.io.File = BINARY_DATA_HERE // java.io.File | 
try {
    val result : PubsubKvPut200Response = apiInstance.pubsubKvPut(bucket, key, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KeyValueApi#pubsubKvPut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KeyValueApi#pubsubKvPut")
    e.printStackTrace()
}
```

### Parameters
| **bucket** | **kotlin.String**|  | |
| **key** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **java.io.File**|  | |

### Return type

[**PubsubKvPut200Response**](PubsubKvPut200Response.md)

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

