# RecordsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoCreateRecord**](RecordsApi.md#autoCreateRecord) | **POST** /v1/auto/records | Create a record |
| [**autoListRecords**](RecordsApi.md#autoListRecords) | **GET** /v1/auto/records | List records in a table |
| [**baseCreateRecord**](RecordsApi.md#baseCreateRecord) | **POST** /v1/collections/{collection}/records | Create a record |
| [**baseDeleteRecord**](RecordsApi.md#baseDeleteRecord) | **DELETE** /v1/collections/{collection}/records/{id} | Delete a record |
| [**baseGetRecord**](RecordsApi.md#baseGetRecord) | **GET** /v1/collections/{collection}/records/{id} | Get a record |
| [**baseListRecords**](RecordsApi.md#baseListRecords) | **GET** /v1/collections/{collection}/records | List records |
| [**baseUpdateRecord**](RecordsApi.md#baseUpdateRecord) | **PATCH** /v1/collections/{collection}/records/{id} | Update a record |
| [**dnsCreateRecord**](RecordsApi.md#dnsCreateRecord) | **POST** /v1/dns/zones/{zone}/records | Create DNS record |
| [**dnsDeleteRecord**](RecordsApi.md#dnsDeleteRecord) | **DELETE** /v1/dns/zones/{zone}/records/{id} | Delete DNS record |
| [**dnsGetRecord**](RecordsApi.md#dnsGetRecord) | **GET** /v1/dns/zones/{zone}/records/{id} | Get DNS record |
| [**dnsListRecords**](RecordsApi.md#dnsListRecords) | **GET** /v1/dns/zones/{zone}/records | List DNS records |
| [**dnsUpdateRecord**](RecordsApi.md#dnsUpdateRecord) | **PUT** /v1/dns/zones/{zone}/records/{id} | Update DNS record |
| [**flowCreateRecord**](RecordsApi.md#flowCreateRecord) | **POST** /v1/flow/records | Create a record |
| [**flowDeleteRecord**](RecordsApi.md#flowDeleteRecord) | **DELETE** /v1/flow/records/{id} | Delete a record |
| [**flowGetRecord**](RecordsApi.md#flowGetRecord) | **GET** /v1/flow/records/{id} | Get a record |
| [**flowListRecords**](RecordsApi.md#flowListRecords) | **GET** /v1/flow/records | List records in a table |
| [**flowUpdateRecord**](RecordsApi.md#flowUpdateRecord) | **PATCH** /v1/flow/records/{id} | Update a record |


<a id="autoCreateRecord"></a>
# **autoCreateRecord**
> kotlin.Any autoCreateRecord(autoCreateRecordRequest)

Create a record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordsApi()
val autoCreateRecordRequest : AutoCreateRecordRequest =  // AutoCreateRecordRequest | 
try {
    val result : kotlin.Any = apiInstance.autoCreateRecord(autoCreateRecordRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordsApi#autoCreateRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordsApi#autoCreateRecord")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoCreateRecordRequest** | [**AutoCreateRecordRequest**](AutoCreateRecordRequest.md)|  | |

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

<a id="autoListRecords"></a>
# **autoListRecords**
> kotlin.Any autoListRecords(tableId)

List records in a table

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordsApi()
val tableId : kotlin.String = tableId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.autoListRecords(tableId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordsApi#autoListRecords")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordsApi#autoListRecords")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **tableId** | **kotlin.String**|  | |

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

<a id="baseCreateRecord"></a>
# **baseCreateRecord**
> BaseRecord baseCreateRecord(collection, baseRecord)

Create a record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordsApi()
val collection : kotlin.String = collection_example // kotlin.String | Collection name or id (e.g. `site_drafts`).
val baseRecord : BaseRecord =  // BaseRecord | 
try {
    val result : BaseRecord = apiInstance.baseCreateRecord(collection, baseRecord)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordsApi#baseCreateRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordsApi#baseCreateRecord")
    e.printStackTrace()
}
```

### Parameters
| **collection** | **kotlin.String**| Collection name or id (e.g. &#x60;site_drafts&#x60;). | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **baseRecord** | [**BaseRecord**](BaseRecord.md)|  | |

### Return type

[**BaseRecord**](BaseRecord.md)

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

<a id="baseDeleteRecord"></a>
# **baseDeleteRecord**
> baseDeleteRecord(collection, id)

Delete a record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordsApi()
val collection : kotlin.String = collection_example // kotlin.String | 
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.baseDeleteRecord(collection, id)
} catch (e: ClientException) {
    println("4xx response calling RecordsApi#baseDeleteRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordsApi#baseDeleteRecord")
    e.printStackTrace()
}
```

### Parameters
| **collection** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

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

<a id="baseGetRecord"></a>
# **baseGetRecord**
> BaseRecord baseGetRecord(collection, id)

Get a record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordsApi()
val collection : kotlin.String = collection_example // kotlin.String | 
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : BaseRecord = apiInstance.baseGetRecord(collection, id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordsApi#baseGetRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordsApi#baseGetRecord")
    e.printStackTrace()
}
```

### Parameters
| **collection** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**BaseRecord**](BaseRecord.md)

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

<a id="baseListRecords"></a>
# **baseListRecords**
> BaseRecordList baseListRecords(collection, filter, sort, page, perPage)

List records

List rows in a collection. Supports a PocketBase-style &#x60;filter&#x60; expression, &#x60;sort&#x60;, and page controls. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordsApi()
val collection : kotlin.String = collection_example // kotlin.String | Collection name or id (e.g. `site_drafts`).
val filter : kotlin.String = filter_example // kotlin.String | Filter expression, e.g. org='hanzo' && slug='home'.
val sort : kotlin.String = sort_example // kotlin.String | 
val page : kotlin.Int = 56 // kotlin.Int | 
val perPage : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : BaseRecordList = apiInstance.baseListRecords(collection, filter, sort, page, perPage)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordsApi#baseListRecords")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordsApi#baseListRecords")
    e.printStackTrace()
}
```

### Parameters
| **collection** | **kotlin.String**| Collection name or id (e.g. &#x60;site_drafts&#x60;). | |
| **filter** | **kotlin.String**| Filter expression, e.g. org&#x3D;&#39;hanzo&#39; &amp;&amp; slug&#x3D;&#39;home&#39;. | [optional] |
| **sort** | **kotlin.String**|  | [optional] |
| **page** | **kotlin.Int**|  | [optional] [default to 1] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **perPage** | **kotlin.Int**|  | [optional] [default to 30] |

### Return type

[**BaseRecordList**](BaseRecordList.md)

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

<a id="baseUpdateRecord"></a>
# **baseUpdateRecord**
> BaseRecord baseUpdateRecord(collection, id, baseRecord)

Update a record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordsApi()
val collection : kotlin.String = collection_example // kotlin.String | 
val id : kotlin.String = id_example // kotlin.String | 
val baseRecord : BaseRecord =  // BaseRecord | 
try {
    val result : BaseRecord = apiInstance.baseUpdateRecord(collection, id, baseRecord)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordsApi#baseUpdateRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordsApi#baseUpdateRecord")
    e.printStackTrace()
}
```

### Parameters
| **collection** | **kotlin.String**|  | |
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **baseRecord** | [**BaseRecord**](BaseRecord.md)|  | |

### Return type

[**BaseRecord**](BaseRecord.md)

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

<a id="dnsCreateRecord"></a>
# **dnsCreateRecord**
> DnsRecord dnsCreateRecord(zone, dnsRecordCreate)

Create DNS record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordsApi()
val zone : kotlin.String = zone_example // kotlin.String | 
val dnsRecordCreate : DnsRecordCreate =  // DnsRecordCreate | 
try {
    val result : DnsRecord = apiInstance.dnsCreateRecord(zone, dnsRecordCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordsApi#dnsCreateRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordsApi#dnsCreateRecord")
    e.printStackTrace()
}
```

### Parameters
| **zone** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **dnsRecordCreate** | [**DnsRecordCreate**](DnsRecordCreate.md)|  | |

### Return type

[**DnsRecord**](DnsRecord.md)

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

<a id="dnsDeleteRecord"></a>
# **dnsDeleteRecord**
> kotlin.Any dnsDeleteRecord(zone, id)

Delete DNS record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordsApi()
val zone : kotlin.String = zone_example // kotlin.String | 
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.dnsDeleteRecord(zone, id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordsApi#dnsDeleteRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordsApi#dnsDeleteRecord")
    e.printStackTrace()
}
```

### Parameters
| **zone** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

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

<a id="dnsGetRecord"></a>
# **dnsGetRecord**
> DnsRecord dnsGetRecord(zone, id)

Get DNS record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordsApi()
val zone : kotlin.String = zone_example // kotlin.String | 
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : DnsRecord = apiInstance.dnsGetRecord(zone, id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordsApi#dnsGetRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordsApi#dnsGetRecord")
    e.printStackTrace()
}
```

### Parameters
| **zone** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**DnsRecord**](DnsRecord.md)

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

<a id="dnsListRecords"></a>
# **dnsListRecords**
> DnsListRecords200Response dnsListRecords(zone, type, name, page, pageSize)

List DNS records

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordsApi()
val zone : kotlin.String = zone_example // kotlin.String | 
val type : kotlin.String = type_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | Filter by record name
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : DnsListRecords200Response = apiInstance.dnsListRecords(zone, type, name, page, pageSize)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordsApi#dnsListRecords")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordsApi#dnsListRecords")
    e.printStackTrace()
}
```

### Parameters
| **zone** | **kotlin.String**|  | |
| **type** | **kotlin.String**|  | [optional] [enum: A, AAAA, CNAME, MX, TXT, SRV, NS, SOA, CAA] |
| **name** | **kotlin.String**| Filter by record name | [optional] |
| **page** | **kotlin.Int**|  | [optional] [default to 1] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **pageSize** | **kotlin.Int**|  | [optional] [default to 100] |

### Return type

[**DnsListRecords200Response**](DnsListRecords200Response.md)

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

<a id="dnsUpdateRecord"></a>
# **dnsUpdateRecord**
> DnsRecord dnsUpdateRecord(zone, id, dnsUpdateRecordRequest)

Update DNS record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordsApi()
val zone : kotlin.String = zone_example // kotlin.String | 
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val dnsUpdateRecordRequest : DnsUpdateRecordRequest =  // DnsUpdateRecordRequest | 
try {
    val result : DnsRecord = apiInstance.dnsUpdateRecord(zone, id, dnsUpdateRecordRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordsApi#dnsUpdateRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordsApi#dnsUpdateRecord")
    e.printStackTrace()
}
```

### Parameters
| **zone** | **kotlin.String**|  | |
| **id** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **dnsUpdateRecordRequest** | [**DnsUpdateRecordRequest**](DnsUpdateRecordRequest.md)|  | |

### Return type

[**DnsRecord**](DnsRecord.md)

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

<a id="flowCreateRecord"></a>
# **flowCreateRecord**
> kotlin.Any flowCreateRecord(autoCreateRecordRequest)

Create a record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordsApi()
val autoCreateRecordRequest : AutoCreateRecordRequest =  // AutoCreateRecordRequest | 
try {
    val result : kotlin.Any = apiInstance.flowCreateRecord(autoCreateRecordRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordsApi#flowCreateRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordsApi#flowCreateRecord")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoCreateRecordRequest** | [**AutoCreateRecordRequest**](AutoCreateRecordRequest.md)|  | |

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

<a id="flowDeleteRecord"></a>
# **flowDeleteRecord**
> flowDeleteRecord(id)

Delete a record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.flowDeleteRecord(id)
} catch (e: ClientException) {
    println("4xx response calling RecordsApi#flowDeleteRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordsApi#flowDeleteRecord")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

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

<a id="flowGetRecord"></a>
# **flowGetRecord**
> kotlin.Any flowGetRecord(id)

Get a record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.flowGetRecord(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordsApi#flowGetRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordsApi#flowGetRecord")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

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

<a id="flowListRecords"></a>
# **flowListRecords**
> kotlin.Any flowListRecords(tableId, cursor, limit)

List records in a table

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordsApi()
val tableId : kotlin.String = tableId_example // kotlin.String | 
val cursor : kotlin.String = cursor_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : kotlin.Any = apiInstance.flowListRecords(tableId, cursor, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordsApi#flowListRecords")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordsApi#flowListRecords")
    e.printStackTrace()
}
```

### Parameters
| **tableId** | **kotlin.String**|  | |
| **cursor** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] |

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

<a id="flowUpdateRecord"></a>
# **flowUpdateRecord**
> kotlin.Any flowUpdateRecord(id, flowUpdateRecordRequest)

Update a record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordsApi()
val id : kotlin.String = id_example // kotlin.String | 
val flowUpdateRecordRequest : FlowUpdateRecordRequest =  // FlowUpdateRecordRequest | 
try {
    val result : kotlin.Any = apiInstance.flowUpdateRecord(id, flowUpdateRecordRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordsApi#flowUpdateRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordsApi#flowUpdateRecord")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **flowUpdateRecordRequest** | [**FlowUpdateRecordRequest**](FlowUpdateRecordRequest.md)|  | |

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

