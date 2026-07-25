# ConflictApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**worldWorldAcled**](ConflictApi.md#worldWorldAcled) | **GET** /v1/world/acled | ACLED conflict events (requires ACLED_ACCESS_TOKEN) |
| [**worldWorldAcledConflict**](ConflictApi.md#worldWorldAcledConflict) | **GET** /v1/world/acled-conflict | ACLED conflict summary (requires ACLED_ACCESS_TOKEN) |
| [**worldWorldCyberThreats**](ConflictApi.md#worldWorldCyberThreats) | **GET** /v1/world/cyber-threats | Cyber threat feed |
| [**worldWorldHapi**](ConflictApi.md#worldWorldHapi) | **GET** /v1/world/hapi | Humanitarian API (HDX HAPI) |
| [**worldWorldUcdp**](ConflictApi.md#worldWorldUcdp) | **GET** /v1/world/ucdp | UCDP conflict data |
| [**worldWorldUcdpEvents**](ConflictApi.md#worldWorldUcdpEvents) | **GET** /v1/world/ucdp-events | UCDP georeferenced events |
| [**worldWorldUnhcrPopulation**](ConflictApi.md#worldWorldUnhcrPopulation) | **GET** /v1/world/unhcr-population | UNHCR displacement/population |


<a id="worldWorldAcled"></a>
# **worldWorldAcled**
> kotlin.Any worldWorldAcled()

ACLED conflict events (requires ACLED_ACCESS_TOKEN)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConflictApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldAcled()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConflictApi#worldWorldAcled")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConflictApi#worldWorldAcled")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

<a id="worldWorldAcledConflict"></a>
# **worldWorldAcledConflict**
> kotlin.Any worldWorldAcledConflict()

ACLED conflict summary (requires ACLED_ACCESS_TOKEN)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConflictApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldAcledConflict()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConflictApi#worldWorldAcledConflict")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConflictApi#worldWorldAcledConflict")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

<a id="worldWorldCyberThreats"></a>
# **worldWorldCyberThreats**
> kotlin.Any worldWorldCyberThreats()

Cyber threat feed

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConflictApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldCyberThreats()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConflictApi#worldWorldCyberThreats")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConflictApi#worldWorldCyberThreats")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

<a id="worldWorldHapi"></a>
# **worldWorldHapi**
> kotlin.Any worldWorldHapi()

Humanitarian API (HDX HAPI)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConflictApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldHapi()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConflictApi#worldWorldHapi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConflictApi#worldWorldHapi")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

<a id="worldWorldUcdp"></a>
# **worldWorldUcdp**
> kotlin.Any worldWorldUcdp()

UCDP conflict data

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConflictApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldUcdp()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConflictApi#worldWorldUcdp")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConflictApi#worldWorldUcdp")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

<a id="worldWorldUcdpEvents"></a>
# **worldWorldUcdpEvents**
> kotlin.Any worldWorldUcdpEvents()

UCDP georeferenced events

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConflictApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldUcdpEvents()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConflictApi#worldWorldUcdpEvents")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConflictApi#worldWorldUcdpEvents")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

<a id="worldWorldUnhcrPopulation"></a>
# **worldWorldUnhcrPopulation**
> kotlin.Any worldWorldUnhcrPopulation()

UNHCR displacement/population

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConflictApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldUnhcrPopulation()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConflictApi#worldWorldUnhcrPopulation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConflictApi#worldWorldUnhcrPopulation")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

