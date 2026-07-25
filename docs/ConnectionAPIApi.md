# ConnectionAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerAddConnection**](ConnectionAPIApi.md#cloudApiControllerAddConnection) | **POST** /v1/cloud/add-connection | Api Controller Add Connection |
| [**cloudApiControllerAddNodeTunnel**](ConnectionAPIApi.md#cloudApiControllerAddNodeTunnel) | **GET** /v1/cloud/add-node-tunnel | Api Controller Add Node Tunnel |
| [**cloudApiControllerDeleteConnection**](ConnectionAPIApi.md#cloudApiControllerDeleteConnection) | **POST** /v1/cloud/delete-connection | Api Controller Delete Connection |
| [**cloudApiControllerGetConnection**](ConnectionAPIApi.md#cloudApiControllerGetConnection) | **GET** /v1/cloud/get-connection | Api Controller Get Connection |
| [**cloudApiControllerGetConnections**](ConnectionAPIApi.md#cloudApiControllerGetConnections) | **GET** /v1/cloud/get-connections | Api Controller Get Connections |
| [**cloudApiControllerGetNodeTunnel**](ConnectionAPIApi.md#cloudApiControllerGetNodeTunnel) | **GET** /v1/cloud/get-node-tunnel | Api Controller Get Node Tunnel |
| [**cloudApiControllerStartConnection**](ConnectionAPIApi.md#cloudApiControllerStartConnection) | **POST** /v1/cloud/start-connection | Api Controller Start Connection |
| [**cloudApiControllerStopConnection**](ConnectionAPIApi.md#cloudApiControllerStopConnection) | **POST** /v1/cloud/stop-connection | Api Controller Stop Connection |
| [**cloudApiControllerUpdateConnection**](ConnectionAPIApi.md#cloudApiControllerUpdateConnection) | **POST** /v1/cloud/update-connection | Api Controller Update Connection |
| [**nexusAddConnection**](ConnectionAPIApi.md#nexusAddConnection) | **POST** /v1/nexus/add-connection | add Connection |
| [**nexusAddNodeTunnel**](ConnectionAPIApi.md#nexusAddNodeTunnel) | **GET** /v1/nexus/add-node-tunnel | add Node Tunnel |
| [**nexusDeleteConnection**](ConnectionAPIApi.md#nexusDeleteConnection) | **POST** /v1/nexus/delete-connection | delete Connection |
| [**nexusGetConnection**](ConnectionAPIApi.md#nexusGetConnection) | **GET** /v1/nexus/get-connection | get Connection |
| [**nexusGetConnections**](ConnectionAPIApi.md#nexusGetConnections) | **GET** /v1/nexus/get-connections | get Connections |
| [**nexusGetNodeTunnel**](ConnectionAPIApi.md#nexusGetNodeTunnel) | **GET** /v1/nexus/get-node-tunnel | get Node Tunnel |
| [**nexusStartConnection**](ConnectionAPIApi.md#nexusStartConnection) | **POST** /v1/nexus/start-connection | start Connection |
| [**nexusStopConnection**](ConnectionAPIApi.md#nexusStopConnection) | **POST** /v1/nexus/stop-connection | stop Connection |
| [**nexusUpdateConnection**](ConnectionAPIApi.md#nexusUpdateConnection) | **POST** /v1/nexus/update-connection | update Connection |


<a id="cloudApiControllerAddConnection"></a>
# **cloudApiControllerAddConnection**
> kotlin.Any cloudApiControllerAddConnection(cloudObjectConnection)

Api Controller Add Connection

add connection

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConnectionAPIApi()
val cloudObjectConnection : CloudObjectConnection =  // CloudObjectConnection | The connection object
try {
    val result : kotlin.Any = apiInstance.cloudApiControllerAddConnection(cloudObjectConnection)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConnectionAPIApi#cloudApiControllerAddConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConnectionAPIApi#cloudApiControllerAddConnection")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectConnection** | [**CloudObjectConnection**](CloudObjectConnection.md)| The connection object | |

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

<a id="cloudApiControllerAddNodeTunnel"></a>
# **cloudApiControllerAddNodeTunnel**
> kotlin.Any cloudApiControllerAddNodeTunnel(nodeId)

Api Controller Add Node Tunnel

add node tunnel session

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConnectionAPIApi()
val nodeId : kotlin.String = nodeId_example // kotlin.String | The id of node
try {
    val result : kotlin.Any = apiInstance.cloudApiControllerAddNodeTunnel(nodeId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConnectionAPIApi#cloudApiControllerAddNodeTunnel")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConnectionAPIApi#cloudApiControllerAddNodeTunnel")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nodeId** | **kotlin.String**| The id of node | |

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

<a id="cloudApiControllerDeleteConnection"></a>
# **cloudApiControllerDeleteConnection**
> kotlin.Any cloudApiControllerDeleteConnection(id)

Api Controller Delete Connection

delete connection

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConnectionAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id of connection
try {
    val result : kotlin.Any = apiInstance.cloudApiControllerDeleteConnection(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConnectionAPIApi#cloudApiControllerDeleteConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConnectionAPIApi#cloudApiControllerDeleteConnection")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id of connection | |

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

<a id="cloudApiControllerGetConnection"></a>
# **cloudApiControllerGetConnection**
> CloudObjectConnection cloudApiControllerGetConnection(id)

Api Controller Get Connection

get connection

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConnectionAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id of connection
try {
    val result : CloudObjectConnection = apiInstance.cloudApiControllerGetConnection(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConnectionAPIApi#cloudApiControllerGetConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConnectionAPIApi#cloudApiControllerGetConnection")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id of connection | |

### Return type

[**CloudObjectConnection**](CloudObjectConnection.md)

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

<a id="cloudApiControllerGetConnections"></a>
# **cloudApiControllerGetConnections**
> CloudObjectConnection cloudApiControllerGetConnections(pageSize, p)

Api Controller Get Connections

get all connections

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConnectionAPIApi()
val pageSize : kotlin.String = pageSize_example // kotlin.String | The size of each page
val p : kotlin.String = p_example // kotlin.String | The number of the page
try {
    val result : CloudObjectConnection = apiInstance.cloudApiControllerGetConnections(pageSize, p)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConnectionAPIApi#cloudApiControllerGetConnections")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConnectionAPIApi#cloudApiControllerGetConnections")
    e.printStackTrace()
}
```

### Parameters
| **pageSize** | **kotlin.String**| The size of each page | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **p** | **kotlin.String**| The number of the page | |

### Return type

[**CloudObjectConnection**](CloudObjectConnection.md)

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

<a id="cloudApiControllerGetNodeTunnel"></a>
# **cloudApiControllerGetNodeTunnel**
> kotlin.Any cloudApiControllerGetNodeTunnel(width, height, dpi, connectionId, username, password)

Api Controller Get Node Tunnel

get node tunnel session

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConnectionAPIApi()
val width : kotlin.String = width_example // kotlin.String | The width of the tunnel
val height : kotlin.String = height_example // kotlin.String | The height of the tunnel
val dpi : kotlin.String = dpi_example // kotlin.String | The dpi of the tunnel
val connectionId : kotlin.String = connectionId_example // kotlin.String | The id of the connectionId
val username : kotlin.String = username_example // kotlin.String | The username for the tunnel
val password : kotlin.String = password_example // kotlin.String | The password for the tunnel
try {
    val result : kotlin.Any = apiInstance.cloudApiControllerGetNodeTunnel(width, height, dpi, connectionId, username, password)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConnectionAPIApi#cloudApiControllerGetNodeTunnel")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConnectionAPIApi#cloudApiControllerGetNodeTunnel")
    e.printStackTrace()
}
```

### Parameters
| **width** | **kotlin.String**| The width of the tunnel | |
| **height** | **kotlin.String**| The height of the tunnel | |
| **dpi** | **kotlin.String**| The dpi of the tunnel | |
| **connectionId** | **kotlin.String**| The id of the connectionId | |
| **username** | **kotlin.String**| The username for the tunnel | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **password** | **kotlin.String**| The password for the tunnel | |

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

<a id="cloudApiControllerStartConnection"></a>
# **cloudApiControllerStartConnection**
> kotlin.Any cloudApiControllerStartConnection(id)

Api Controller Start Connection

start connection

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConnectionAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id of connection
try {
    val result : kotlin.Any = apiInstance.cloudApiControllerStartConnection(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConnectionAPIApi#cloudApiControllerStartConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConnectionAPIApi#cloudApiControllerStartConnection")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id of connection | |

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

<a id="cloudApiControllerStopConnection"></a>
# **cloudApiControllerStopConnection**
> kotlin.Any cloudApiControllerStopConnection(id)

Api Controller Stop Connection

stop connection

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConnectionAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id of connection
try {
    val result : kotlin.Any = apiInstance.cloudApiControllerStopConnection(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConnectionAPIApi#cloudApiControllerStopConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConnectionAPIApi#cloudApiControllerStopConnection")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id of connection | |

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

<a id="cloudApiControllerUpdateConnection"></a>
# **cloudApiControllerUpdateConnection**
> kotlin.Any cloudApiControllerUpdateConnection(id, cloudObjectConnection)

Api Controller Update Connection

update connection

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConnectionAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id of connection
val cloudObjectConnection : CloudObjectConnection =  // CloudObjectConnection | The connection object
try {
    val result : kotlin.Any = apiInstance.cloudApiControllerUpdateConnection(id, cloudObjectConnection)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConnectionAPIApi#cloudApiControllerUpdateConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConnectionAPIApi#cloudApiControllerUpdateConnection")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id of connection | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectConnection** | [**CloudObjectConnection**](CloudObjectConnection.md)| The connection object | |

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

<a id="nexusAddConnection"></a>
# **nexusAddConnection**
> kotlin.Any nexusAddConnection(cloudObjectConnection)

add Connection

Add a connection

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConnectionAPIApi()
val cloudObjectConnection : CloudObjectConnection =  // CloudObjectConnection | The connection object
try {
    val result : kotlin.Any = apiInstance.nexusAddConnection(cloudObjectConnection)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConnectionAPIApi#nexusAddConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConnectionAPIApi#nexusAddConnection")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectConnection** | [**CloudObjectConnection**](CloudObjectConnection.md)| The connection object | |

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

<a id="nexusAddNodeTunnel"></a>
# **nexusAddNodeTunnel**
> kotlin.Any nexusAddNodeTunnel(nodeId)

add Node Tunnel

Add a node tunnel session

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConnectionAPIApi()
val nodeId : kotlin.String = nodeId_example // kotlin.String | The id of the node
try {
    val result : kotlin.Any = apiInstance.nexusAddNodeTunnel(nodeId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConnectionAPIApi#nexusAddNodeTunnel")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConnectionAPIApi#nexusAddNodeTunnel")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nodeId** | **kotlin.String**| The id of the node | |

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

<a id="nexusDeleteConnection"></a>
# **nexusDeleteConnection**
> kotlin.Any nexusDeleteConnection(id)

delete Connection

Delete a connection

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConnectionAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id of the connection
try {
    val result : kotlin.Any = apiInstance.nexusDeleteConnection(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConnectionAPIApi#nexusDeleteConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConnectionAPIApi#nexusDeleteConnection")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id of the connection | |

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

<a id="nexusGetConnection"></a>
# **nexusGetConnection**
> CloudObjectConnection nexusGetConnection(id)

get Connection

Get a connection

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConnectionAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id of the connection
try {
    val result : CloudObjectConnection = apiInstance.nexusGetConnection(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConnectionAPIApi#nexusGetConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConnectionAPIApi#nexusGetConnection")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id of the connection | |

### Return type

[**CloudObjectConnection**](CloudObjectConnection.md)

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

<a id="nexusGetConnections"></a>
# **nexusGetConnections**
> CloudObjectConnection nexusGetConnections(pageSize, p)

get Connections

Get all connections

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConnectionAPIApi()
val pageSize : kotlin.String = pageSize_example // kotlin.String | The size of each page
val p : kotlin.String = p_example // kotlin.String | The page number
try {
    val result : CloudObjectConnection = apiInstance.nexusGetConnections(pageSize, p)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConnectionAPIApi#nexusGetConnections")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConnectionAPIApi#nexusGetConnections")
    e.printStackTrace()
}
```

### Parameters
| **pageSize** | **kotlin.String**| The size of each page | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **p** | **kotlin.String**| The page number | |

### Return type

[**CloudObjectConnection**](CloudObjectConnection.md)

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

<a id="nexusGetNodeTunnel"></a>
# **nexusGetNodeTunnel**
> kotlin.Any nexusGetNodeTunnel(width, height, dpi, connectionId, username, password)

get Node Tunnel

Get a node tunnel session

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConnectionAPIApi()
val width : kotlin.String = width_example // kotlin.String | The width of the tunnel
val height : kotlin.String = height_example // kotlin.String | The height of the tunnel
val dpi : kotlin.String = dpi_example // kotlin.String | The dpi of the tunnel
val connectionId : kotlin.String = connectionId_example // kotlin.String | The id of the connection
val username : kotlin.String = username_example // kotlin.String | The username for the tunnel
val password : kotlin.String = password_example // kotlin.String | The password for the tunnel
try {
    val result : kotlin.Any = apiInstance.nexusGetNodeTunnel(width, height, dpi, connectionId, username, password)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConnectionAPIApi#nexusGetNodeTunnel")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConnectionAPIApi#nexusGetNodeTunnel")
    e.printStackTrace()
}
```

### Parameters
| **width** | **kotlin.String**| The width of the tunnel | |
| **height** | **kotlin.String**| The height of the tunnel | |
| **dpi** | **kotlin.String**| The dpi of the tunnel | |
| **connectionId** | **kotlin.String**| The id of the connection | |
| **username** | **kotlin.String**| The username for the tunnel | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **password** | **kotlin.String**| The password for the tunnel | |

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

<a id="nexusStartConnection"></a>
# **nexusStartConnection**
> kotlin.Any nexusStartConnection(id)

start Connection

Start a connection

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConnectionAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id of the connection
try {
    val result : kotlin.Any = apiInstance.nexusStartConnection(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConnectionAPIApi#nexusStartConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConnectionAPIApi#nexusStartConnection")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id of the connection | |

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

<a id="nexusStopConnection"></a>
# **nexusStopConnection**
> kotlin.Any nexusStopConnection(id)

stop Connection

Stop a connection

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConnectionAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id of the connection
try {
    val result : kotlin.Any = apiInstance.nexusStopConnection(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConnectionAPIApi#nexusStopConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConnectionAPIApi#nexusStopConnection")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id of the connection | |

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

<a id="nexusUpdateConnection"></a>
# **nexusUpdateConnection**
> kotlin.Any nexusUpdateConnection(id, cloudObjectConnection)

update Connection

Update a connection

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConnectionAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id of the connection
val cloudObjectConnection : CloudObjectConnection =  // CloudObjectConnection | The connection object
try {
    val result : kotlin.Any = apiInstance.nexusUpdateConnection(id, cloudObjectConnection)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConnectionAPIApi#nexusUpdateConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConnectionAPIApi#nexusUpdateConnection")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id of the connection | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectConnection** | [**CloudObjectConnection**](CloudObjectConnection.md)| The connection object | |

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

