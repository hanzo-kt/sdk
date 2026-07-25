# SecretsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**edgeCreateSecret**](SecretsApi.md#edgeCreateSecret) | **POST** /v1/edge/secrets | Create secret |
| [**edgeDeleteSecret**](SecretsApi.md#edgeDeleteSecret) | **DELETE** /v1/edge/secrets/{name} | Delete secret |
| [**edgeListSecrets**](SecretsApi.md#edgeListSecrets) | **GET** /v1/edge/secrets | List secrets |
| [**edgeUpdateSecret**](SecretsApi.md#edgeUpdateSecret) | **PUT** /v1/edge/secrets/{name} | Update secret |
| [**kmsBatchSecrets**](SecretsApi.md#kmsBatchSecrets) | **POST** /v1/kms/v4/secrets/batch | Batch create, update, and delete secrets |
| [**kmsCreateSecret**](SecretsApi.md#kmsCreateSecret) | **POST** /v1/kms/v4/secrets/{secretKey} | Create a secret |
| [**kmsDeleteSecret**](SecretsApi.md#kmsDeleteSecret) | **DELETE** /v1/kms/v4/secrets/{secretKey} | Delete a secret |
| [**kmsGetSecret**](SecretsApi.md#kmsGetSecret) | **GET** /v1/kms/v4/secrets/{secretKey} | Get a secret by key |
| [**kmsKmsDeleteOrgSecret**](SecretsApi.md#kmsKmsDeleteOrgSecret) | **DELETE** /v1/kms/orgs/{org}/secrets/{rest} | Delete a secret |
| [**kmsKmsGetOrgSecret**](SecretsApi.md#kmsKmsGetOrgSecret) | **GET** /v1/kms/orgs/{org}/secrets/{rest} | Reveal one secret value |
| [**kmsKmsListOrgSecrets**](SecretsApi.md#kmsKmsListOrgSecrets) | **GET** /v1/kms/orgs/{org}/secrets | List an org&#39;s secret metadata (names only, never values) |
| [**kmsKmsPutOrgSecret**](SecretsApi.md#kmsKmsPutOrgSecret) | **POST** /v1/kms/orgs/{org}/secrets | Create or upsert a secret (value write-only; version bumps) |
| [**kmsKmsRotateOrgSecret**](SecretsApi.md#kmsKmsRotateOrgSecret) | **PATCH** /v1/kms/orgs/{org}/secrets/{rest} | Rotate a secret (compare-and-set on version) |
| [**kmsListSecrets**](SecretsApi.md#kmsListSecrets) | **GET** /v1/kms/v4/secrets | List secrets |
| [**kmsUpdateSecret**](SecretsApi.md#kmsUpdateSecret) | **PATCH** /v1/kms/v4/secrets/{secretKey} | Update a secret |


<a id="edgeCreateSecret"></a>
# **edgeCreateSecret**
> EdgeSecret edgeCreateSecret(edgeSecretCreate)

Create secret

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretsApi()
val edgeSecretCreate : EdgeSecretCreate =  // EdgeSecretCreate | 
try {
    val result : EdgeSecret = apiInstance.edgeCreateSecret(edgeSecretCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretsApi#edgeCreateSecret")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretsApi#edgeCreateSecret")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **edgeSecretCreate** | [**EdgeSecretCreate**](EdgeSecretCreate.md)|  | |

### Return type

[**EdgeSecret**](EdgeSecret.md)

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

<a id="edgeDeleteSecret"></a>
# **edgeDeleteSecret**
> kotlin.Any edgeDeleteSecret(name)

Delete secret

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretsApi()
val name : kotlin.String = name_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.edgeDeleteSecret(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretsApi#edgeDeleteSecret")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretsApi#edgeDeleteSecret")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | |

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

<a id="edgeListSecrets"></a>
# **edgeListSecrets**
> kotlin.collections.List&lt;EdgeListSecrets200ResponseInner&gt; edgeListSecrets()

List secrets

Returns secret names only; values are never exposed after creation.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretsApi()
try {
    val result : kotlin.collections.List<EdgeListSecrets200ResponseInner> = apiInstance.edgeListSecrets()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretsApi#edgeListSecrets")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretsApi#edgeListSecrets")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;EdgeListSecrets200ResponseInner&gt;**](EdgeListSecrets200ResponseInner.md)

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

<a id="edgeUpdateSecret"></a>
# **edgeUpdateSecret**
> kotlin.Any edgeUpdateSecret(name, edgeUpdateSecretRequest)

Update secret

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretsApi()
val name : kotlin.String = name_example // kotlin.String | 
val edgeUpdateSecretRequest : EdgeUpdateSecretRequest =  // EdgeUpdateSecretRequest | 
try {
    val result : kotlin.Any = apiInstance.edgeUpdateSecret(name, edgeUpdateSecretRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretsApi#edgeUpdateSecret")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretsApi#edgeUpdateSecret")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **edgeUpdateSecretRequest** | [**EdgeUpdateSecretRequest**](EdgeUpdateSecretRequest.md)|  | |

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

<a id="kmsBatchSecrets"></a>
# **kmsBatchSecrets**
> KmsBatchSecrets200Response kmsBatchSecrets(workspaceId, kmsBatchSecretRequest)

Batch create, update, and delete secrets

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretsApi()
val workspaceId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val kmsBatchSecretRequest : KmsBatchSecretRequest =  // KmsBatchSecretRequest | 
try {
    val result : KmsBatchSecrets200Response = apiInstance.kmsBatchSecrets(workspaceId, kmsBatchSecretRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretsApi#kmsBatchSecrets")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretsApi#kmsBatchSecrets")
    e.printStackTrace()
}
```

### Parameters
| **workspaceId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsBatchSecretRequest** | [**KmsBatchSecretRequest**](KmsBatchSecretRequest.md)|  | |

### Return type

[**KmsBatchSecrets200Response**](KmsBatchSecrets200Response.md)

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

<a id="kmsCreateSecret"></a>
# **kmsCreateSecret**
> KmsGetSecret200Response kmsCreateSecret(secretKey, kmsCreateSecretRequest)

Create a secret

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretsApi()
val secretKey : kotlin.String = secretKey_example // kotlin.String | 
val kmsCreateSecretRequest : KmsCreateSecretRequest =  // KmsCreateSecretRequest | 
try {
    val result : KmsGetSecret200Response = apiInstance.kmsCreateSecret(secretKey, kmsCreateSecretRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretsApi#kmsCreateSecret")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretsApi#kmsCreateSecret")
    e.printStackTrace()
}
```

### Parameters
| **secretKey** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsCreateSecretRequest** | [**KmsCreateSecretRequest**](KmsCreateSecretRequest.md)|  | |

### Return type

[**KmsGetSecret200Response**](KmsGetSecret200Response.md)

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

<a id="kmsDeleteSecret"></a>
# **kmsDeleteSecret**
> KmsGetSecret200Response kmsDeleteSecret(secretKey, workspaceId, environment, secretPath)

Delete a secret

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretsApi()
val secretKey : kotlin.String = secretKey_example // kotlin.String | 
val workspaceId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val environment : kotlin.String = environment_example // kotlin.String | 
val secretPath : kotlin.String = secretPath_example // kotlin.String | 
try {
    val result : KmsGetSecret200Response = apiInstance.kmsDeleteSecret(secretKey, workspaceId, environment, secretPath)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretsApi#kmsDeleteSecret")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretsApi#kmsDeleteSecret")
    e.printStackTrace()
}
```

### Parameters
| **secretKey** | **kotlin.String**|  | |
| **workspaceId** | **java.util.UUID**|  | |
| **environment** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **secretPath** | **kotlin.String**|  | [optional] [default to &quot;/&quot;] |

### Return type

[**KmsGetSecret200Response**](KmsGetSecret200Response.md)

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

<a id="kmsGetSecret"></a>
# **kmsGetSecret**
> KmsGetSecret200Response kmsGetSecret(secretKey, workspaceId, environment, secretPath, expandSecretReferences, version)

Get a secret by key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretsApi()
val secretKey : kotlin.String = secretKey_example // kotlin.String | 
val workspaceId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val environment : kotlin.String = environment_example // kotlin.String | 
val secretPath : kotlin.String = secretPath_example // kotlin.String | 
val expandSecretReferences : kotlin.Boolean = true // kotlin.Boolean | 
val version : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : KmsGetSecret200Response = apiInstance.kmsGetSecret(secretKey, workspaceId, environment, secretPath, expandSecretReferences, version)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretsApi#kmsGetSecret")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretsApi#kmsGetSecret")
    e.printStackTrace()
}
```

### Parameters
| **secretKey** | **kotlin.String**|  | |
| **workspaceId** | **java.util.UUID**|  | |
| **environment** | **kotlin.String**|  | |
| **secretPath** | **kotlin.String**|  | [optional] [default to &quot;/&quot;] |
| **expandSecretReferences** | **kotlin.Boolean**|  | [optional] [default to true] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **version** | **kotlin.Int**|  | [optional] |

### Return type

[**KmsGetSecret200Response**](KmsGetSecret200Response.md)

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

<a id="kmsKmsDeleteOrgSecret"></a>
# **kmsKmsDeleteOrgSecret**
> AnalyticsHeartbeat200Response kmsKmsDeleteOrgSecret(org, rest, env)

Delete a secret

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretsApi()
val org : kotlin.String = org_example // kotlin.String | 
val rest : kotlin.String = rest_example // kotlin.String | The secret's path + name joined (a/b/c/name).
val env : kotlin.String = env_example // kotlin.String | 
try {
    val result : AnalyticsHeartbeat200Response = apiInstance.kmsKmsDeleteOrgSecret(org, rest, env)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretsApi#kmsKmsDeleteOrgSecret")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretsApi#kmsKmsDeleteOrgSecret")
    e.printStackTrace()
}
```

### Parameters
| **org** | **kotlin.String**|  | |
| **rest** | **kotlin.String**| The secret&#39;s path + name joined (a/b/c/name). | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **env** | **kotlin.String**|  | [optional] |

### Return type

[**AnalyticsHeartbeat200Response**](AnalyticsHeartbeat200Response.md)

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

<a id="kmsKmsGetOrgSecret"></a>
# **kmsKmsGetOrgSecret**
> KmsKmsGetOrgSecret200Response kmsKmsGetOrgSecret(org, rest, env)

Reveal one secret value

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretsApi()
val org : kotlin.String = org_example // kotlin.String | 
val rest : kotlin.String = rest_example // kotlin.String | The secret's path + name joined (a/b/c/name).
val env : kotlin.String = env_example // kotlin.String | 
try {
    val result : KmsKmsGetOrgSecret200Response = apiInstance.kmsKmsGetOrgSecret(org, rest, env)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretsApi#kmsKmsGetOrgSecret")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretsApi#kmsKmsGetOrgSecret")
    e.printStackTrace()
}
```

### Parameters
| **org** | **kotlin.String**|  | |
| **rest** | **kotlin.String**| The secret&#39;s path + name joined (a/b/c/name). | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **env** | **kotlin.String**|  | [optional] |

### Return type

[**KmsKmsGetOrgSecret200Response**](KmsKmsGetOrgSecret200Response.md)

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

<a id="kmsKmsListOrgSecrets"></a>
# **kmsKmsListOrgSecrets**
> KmsKmsListOrgSecrets200Response kmsKmsListOrgSecrets(org, env, prefix)

List an org&#39;s secret metadata (names only, never values)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretsApi()
val org : kotlin.String = org_example // kotlin.String | 
val env : kotlin.String = env_example // kotlin.String | Environment slug (devnet, testnet, mainnet, production, …). Default \"default\".
val prefix : kotlin.String = prefix_example // kotlin.String | Restrict the scan to a subpath within brand/{org}.
try {
    val result : KmsKmsListOrgSecrets200Response = apiInstance.kmsKmsListOrgSecrets(org, env, prefix)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretsApi#kmsKmsListOrgSecrets")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretsApi#kmsKmsListOrgSecrets")
    e.printStackTrace()
}
```

### Parameters
| **org** | **kotlin.String**|  | |
| **env** | **kotlin.String**| Environment slug (devnet, testnet, mainnet, production, …). Default \&quot;default\&quot;. | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **prefix** | **kotlin.String**| Restrict the scan to a subpath within brand/{org}. | [optional] |

### Return type

[**KmsKmsListOrgSecrets200Response**](KmsKmsListOrgSecrets200Response.md)

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

<a id="kmsKmsPutOrgSecret"></a>
# **kmsKmsPutOrgSecret**
> KmsKmsPutOrgSecret200Response kmsKmsPutOrgSecret(org, kmsKmsPutOrgSecretRequest)

Create or upsert a secret (value write-only; version bumps)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretsApi()
val org : kotlin.String = org_example // kotlin.String | 
val kmsKmsPutOrgSecretRequest : KmsKmsPutOrgSecretRequest =  // KmsKmsPutOrgSecretRequest | 
try {
    val result : KmsKmsPutOrgSecret200Response = apiInstance.kmsKmsPutOrgSecret(org, kmsKmsPutOrgSecretRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretsApi#kmsKmsPutOrgSecret")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretsApi#kmsKmsPutOrgSecret")
    e.printStackTrace()
}
```

### Parameters
| **org** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsKmsPutOrgSecretRequest** | [**KmsKmsPutOrgSecretRequest**](KmsKmsPutOrgSecretRequest.md)|  | |

### Return type

[**KmsKmsPutOrgSecret200Response**](KmsKmsPutOrgSecret200Response.md)

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

<a id="kmsKmsRotateOrgSecret"></a>
# **kmsKmsRotateOrgSecret**
> KmsKmsPutOrgSecret200Response kmsKmsRotateOrgSecret(org, rest, kmsKmsRotateOrgSecretRequest, ifMatch)

Rotate a secret (compare-and-set on version)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretsApi()
val org : kotlin.String = org_example // kotlin.String | 
val rest : kotlin.String = rest_example // kotlin.String | The secret's path + name joined (a/b/c/name).
val kmsKmsRotateOrgSecretRequest : KmsKmsRotateOrgSecretRequest =  // KmsKmsRotateOrgSecretRequest | 
val ifMatch : kotlin.String = ifMatch_example // kotlin.String | Current version for the compare-and-set (replay protection).
try {
    val result : KmsKmsPutOrgSecret200Response = apiInstance.kmsKmsRotateOrgSecret(org, rest, kmsKmsRotateOrgSecretRequest, ifMatch)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretsApi#kmsKmsRotateOrgSecret")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretsApi#kmsKmsRotateOrgSecret")
    e.printStackTrace()
}
```

### Parameters
| **org** | **kotlin.String**|  | |
| **rest** | **kotlin.String**| The secret&#39;s path + name joined (a/b/c/name). | |
| **kmsKmsRotateOrgSecretRequest** | [**KmsKmsRotateOrgSecretRequest**](KmsKmsRotateOrgSecretRequest.md)|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **ifMatch** | **kotlin.String**| Current version for the compare-and-set (replay protection). | [optional] |

### Return type

[**KmsKmsPutOrgSecret200Response**](KmsKmsPutOrgSecret200Response.md)

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

<a id="kmsListSecrets"></a>
# **kmsListSecrets**
> KmsListSecrets200Response kmsListSecrets(workspaceId, environment, secretPath, expandSecretReferences, recursive, includeImports, tagSlugs, metadataFilter)

List secrets

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretsApi()
val workspaceId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val environment : kotlin.String = environment_example // kotlin.String | 
val secretPath : kotlin.String = secretPath_example // kotlin.String | 
val expandSecretReferences : kotlin.Boolean = true // kotlin.Boolean | 
val recursive : kotlin.Boolean = true // kotlin.Boolean | 
val includeImports : kotlin.Boolean = true // kotlin.Boolean | 
val tagSlugs : kotlin.String = tagSlugs_example // kotlin.String | 
val metadataFilter : kotlin.String = metadataFilter_example // kotlin.String | 
try {
    val result : KmsListSecrets200Response = apiInstance.kmsListSecrets(workspaceId, environment, secretPath, expandSecretReferences, recursive, includeImports, tagSlugs, metadataFilter)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretsApi#kmsListSecrets")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretsApi#kmsListSecrets")
    e.printStackTrace()
}
```

### Parameters
| **workspaceId** | **java.util.UUID**|  | |
| **environment** | **kotlin.String**|  | |
| **secretPath** | **kotlin.String**|  | [optional] [default to &quot;/&quot;] |
| **expandSecretReferences** | **kotlin.Boolean**|  | [optional] [default to true] |
| **recursive** | **kotlin.Boolean**|  | [optional] [default to false] |
| **includeImports** | **kotlin.Boolean**|  | [optional] [default to false] |
| **tagSlugs** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **metadataFilter** | **kotlin.String**|  | [optional] |

### Return type

[**KmsListSecrets200Response**](KmsListSecrets200Response.md)

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

<a id="kmsUpdateSecret"></a>
# **kmsUpdateSecret**
> KmsGetSecret200Response kmsUpdateSecret(secretKey, kmsUpdateSecretRequest)

Update a secret

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretsApi()
val secretKey : kotlin.String = secretKey_example // kotlin.String | 
val kmsUpdateSecretRequest : KmsUpdateSecretRequest =  // KmsUpdateSecretRequest | 
try {
    val result : KmsGetSecret200Response = apiInstance.kmsUpdateSecret(secretKey, kmsUpdateSecretRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretsApi#kmsUpdateSecret")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretsApi#kmsUpdateSecret")
    e.printStackTrace()
}
```

### Parameters
| **secretKey** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsUpdateSecretRequest** | [**KmsUpdateSecretRequest**](KmsUpdateSecretRequest.md)|  | |

### Return type

[**KmsGetSecret200Response**](KmsGetSecret200Response.md)

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

