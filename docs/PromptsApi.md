# PromptsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatDeletePromptsBypromptid**](PromptsApi.md#chatDeletePromptsBypromptid) | **DELETE** /v1/chat/prompts/{promptId} | Delete a prompt |
| [**chatDeletePromptsGroupsBygroupid**](PromptsApi.md#chatDeletePromptsGroupsBygroupid) | **DELETE** /v1/chat/prompts/groups/{groupId} | Delete a prompt group |
| [**chatGetPrompts**](PromptsApi.md#chatGetPrompts) | **GET** /v1/chat/prompts | List user prompts |
| [**chatGetPromptsAll**](PromptsApi.md#chatGetPromptsAll) | **GET** /v1/chat/prompts/all | Get all prompt groups (ACL-aware) |
| [**chatGetPromptsBypromptid**](PromptsApi.md#chatGetPromptsBypromptid) | **GET** /v1/chat/prompts/{promptId} | Get a prompt |
| [**chatGetPromptsGroups**](PromptsApi.md#chatGetPromptsGroups) | **GET** /v1/chat/prompts/groups | List prompt groups (paginated) |
| [**chatGetPromptsGroupsBygroupid**](PromptsApi.md#chatGetPromptsGroupsBygroupid) | **GET** /v1/chat/prompts/groups/{groupId} | Get a prompt group by ID |
| [**chatPatchPromptsBypromptidTagsProduction**](PromptsApi.md#chatPatchPromptsBypromptidTagsProduction) | **PATCH** /v1/chat/prompts/{promptId}/tags/production | Make a prompt the production version |
| [**chatPatchPromptsGroupsBygroupid**](PromptsApi.md#chatPatchPromptsGroupsBygroupid) | **PATCH** /v1/chat/prompts/groups/{groupId} | Update a prompt group |
| [**chatPostPrompts**](PromptsApi.md#chatPostPrompts) | **POST** /v1/chat/prompts | Create a new prompt group with initial prompt |
| [**chatPostPromptsGroupsBygroupidPrompts**](PromptsApi.md#chatPostPromptsGroupsBygroupidPrompts) | **POST** /v1/chat/prompts/groups/{groupId}/prompts | Add a prompt to an existing group |
| [**consoleCreatePrompt**](PromptsApi.md#consoleCreatePrompt) | **POST** /v1/console/prompts | Create a new prompt version |
| [**consoleDeletePrompt**](PromptsApi.md#consoleDeletePrompt) | **DELETE** /v1/console/prompts/{promptName} | Delete prompt versions |
| [**consoleGetPrompt**](PromptsApi.md#consoleGetPrompt) | **GET** /v1/console/prompts/{promptName} | Get a prompt by name |
| [**consoleGetPromptVersion**](PromptsApi.md#consoleGetPromptVersion) | **GET** /v1/console/prompts/{promptName}/versions/{promptVersion} | Get a specific prompt version |
| [**consoleListPrompts**](PromptsApi.md#consoleListPrompts) | **GET** /v1/console/prompts | Get a list of prompt names with versions and labels |
| [**promptsCreatePrompt**](PromptsApi.md#promptsCreatePrompt) | **POST** /v1/prompts | Create a prompt or append a new version |
| [**promptsDeletePrompt**](PromptsApi.md#promptsDeletePrompt) | **DELETE** /v1/prompts/{name} | Delete a prompt and its version history |
| [**promptsGetPrompt**](PromptsApi.md#promptsGetPrompt) | **GET** /v1/prompts/{name} | Prompt detail + version history |
| [**promptsListPrompts**](PromptsApi.md#promptsListPrompts) | **GET** /v1/prompts | List current prompts for the org |
| [**promptsPromptMetrics**](PromptsApi.md#promptsPromptMetrics) | **GET** /v1/prompts/metrics | Real per-prompt statistics |


<a id="chatDeletePromptsBypromptid"></a>
# **chatDeletePromptsBypromptid**
> kotlin.Any chatDeletePromptsBypromptid(promptId)

Delete a prompt

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PromptsApi()
val promptId : kotlin.String = promptId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatDeletePromptsBypromptid(promptId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PromptsApi#chatDeletePromptsBypromptid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PromptsApi#chatDeletePromptsBypromptid")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **promptId** | **kotlin.String**|  | |

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

<a id="chatDeletePromptsGroupsBygroupid"></a>
# **chatDeletePromptsGroupsBygroupid**
> kotlin.Any chatDeletePromptsGroupsBygroupid(groupId)

Delete a prompt group

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PromptsApi()
val groupId : kotlin.String = groupId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatDeletePromptsGroupsBygroupid(groupId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PromptsApi#chatDeletePromptsGroupsBygroupid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PromptsApi#chatDeletePromptsGroupsBygroupid")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **groupId** | **kotlin.String**|  | |

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

<a id="chatGetPrompts"></a>
# **chatGetPrompts**
> kotlin.Any chatGetPrompts(groupId)

List user prompts

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PromptsApi()
val groupId : kotlin.String = groupId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatGetPrompts(groupId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PromptsApi#chatGetPrompts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PromptsApi#chatGetPrompts")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **groupId** | **kotlin.String**|  | [optional] |

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

<a id="chatGetPromptsAll"></a>
# **chatGetPromptsAll**
> kotlin.Any chatGetPromptsAll(name, category)

Get all prompt groups (ACL-aware)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PromptsApi()
val name : kotlin.String = name_example // kotlin.String | 
val category : kotlin.String = category_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatGetPromptsAll(name, category)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PromptsApi#chatGetPromptsAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PromptsApi#chatGetPromptsAll")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **category** | **kotlin.String**|  | [optional] |

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

<a id="chatGetPromptsBypromptid"></a>
# **chatGetPromptsBypromptid**
> kotlin.Any chatGetPromptsBypromptid(promptId)

Get a prompt

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PromptsApi()
val promptId : kotlin.String = promptId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatGetPromptsBypromptid(promptId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PromptsApi#chatGetPromptsBypromptid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PromptsApi#chatGetPromptsBypromptid")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **promptId** | **kotlin.String**|  | |

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

<a id="chatGetPromptsGroups"></a>
# **chatGetPromptsGroups**
> kotlin.Any chatGetPromptsGroups(pageSize, limit, cursor, name, category)

List prompt groups (paginated)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PromptsApi()
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val cursor : kotlin.String = cursor_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val category : kotlin.String = category_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatGetPromptsGroups(pageSize, limit, cursor, name, category)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PromptsApi#chatGetPromptsGroups")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PromptsApi#chatGetPromptsGroups")
    e.printStackTrace()
}
```

### Parameters
| **pageSize** | **kotlin.Int**|  | [optional] |
| **limit** | **kotlin.Int**|  | [optional] |
| **cursor** | **kotlin.String**|  | [optional] |
| **name** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **category** | **kotlin.String**|  | [optional] |

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

<a id="chatGetPromptsGroupsBygroupid"></a>
# **chatGetPromptsGroupsBygroupid**
> kotlin.Any chatGetPromptsGroupsBygroupid(groupId)

Get a prompt group by ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PromptsApi()
val groupId : kotlin.String = groupId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatGetPromptsGroupsBygroupid(groupId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PromptsApi#chatGetPromptsGroupsBygroupid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PromptsApi#chatGetPromptsGroupsBygroupid")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **groupId** | **kotlin.String**|  | |

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

<a id="chatPatchPromptsBypromptidTagsProduction"></a>
# **chatPatchPromptsBypromptidTagsProduction**
> kotlin.Any chatPatchPromptsBypromptidTagsProduction(promptId)

Make a prompt the production version

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PromptsApi()
val promptId : kotlin.String = promptId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatPatchPromptsBypromptidTagsProduction(promptId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PromptsApi#chatPatchPromptsBypromptidTagsProduction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PromptsApi#chatPatchPromptsBypromptidTagsProduction")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **promptId** | **kotlin.String**|  | |

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

<a id="chatPatchPromptsGroupsBygroupid"></a>
# **chatPatchPromptsGroupsBygroupid**
> kotlin.Any chatPatchPromptsGroupsBygroupid(groupId, body)

Update a prompt group

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PromptsApi()
val groupId : kotlin.String = groupId_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.chatPatchPromptsGroupsBygroupid(groupId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PromptsApi#chatPatchPromptsGroupsBygroupid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PromptsApi#chatPatchPromptsGroupsBygroupid")
    e.printStackTrace()
}
```

### Parameters
| **groupId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

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

<a id="chatPostPrompts"></a>
# **chatPostPrompts**
> kotlin.Any chatPostPrompts(chatPostPromptsRequest)

Create a new prompt group with initial prompt

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PromptsApi()
val chatPostPromptsRequest : ChatPostPromptsRequest =  // ChatPostPromptsRequest | 
try {
    val result : kotlin.Any = apiInstance.chatPostPrompts(chatPostPromptsRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PromptsApi#chatPostPrompts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PromptsApi#chatPostPrompts")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostPromptsRequest** | [**ChatPostPromptsRequest**](ChatPostPromptsRequest.md)|  | |

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

<a id="chatPostPromptsGroupsBygroupidPrompts"></a>
# **chatPostPromptsGroupsBygroupidPrompts**
> kotlin.Any chatPostPromptsGroupsBygroupidPrompts(groupId, chatPostPromptsGroupsBygroupidPromptsRequest)

Add a prompt to an existing group

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PromptsApi()
val groupId : kotlin.String = groupId_example // kotlin.String | 
val chatPostPromptsGroupsBygroupidPromptsRequest : ChatPostPromptsGroupsBygroupidPromptsRequest =  // ChatPostPromptsGroupsBygroupidPromptsRequest | 
try {
    val result : kotlin.Any = apiInstance.chatPostPromptsGroupsBygroupidPrompts(groupId, chatPostPromptsGroupsBygroupidPromptsRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PromptsApi#chatPostPromptsGroupsBygroupidPrompts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PromptsApi#chatPostPromptsGroupsBygroupidPrompts")
    e.printStackTrace()
}
```

### Parameters
| **groupId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostPromptsGroupsBygroupidPromptsRequest** | [**ChatPostPromptsGroupsBygroupidPromptsRequest**](ChatPostPromptsGroupsBygroupidPromptsRequest.md)|  | |

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

<a id="consoleCreatePrompt"></a>
# **consoleCreatePrompt**
> ConsolePrompt consoleCreatePrompt(consoleCreatePromptRequest)

Create a new prompt version

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PromptsApi()
val consoleCreatePromptRequest : ConsoleCreatePromptRequest =  // ConsoleCreatePromptRequest | 
try {
    val result : ConsolePrompt = apiInstance.consoleCreatePrompt(consoleCreatePromptRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PromptsApi#consoleCreatePrompt")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PromptsApi#consoleCreatePrompt")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **consoleCreatePromptRequest** | [**ConsoleCreatePromptRequest**](ConsoleCreatePromptRequest.md)|  | |

### Return type

[**ConsolePrompt**](ConsolePrompt.md)

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

<a id="consoleDeletePrompt"></a>
# **consoleDeletePrompt**
> kotlin.Any consoleDeletePrompt(promptName, label, version)

Delete prompt versions

If neither version nor label is specified, all versions are deleted.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PromptsApi()
val promptName : kotlin.String = promptName_example // kotlin.String | 
val label : kotlin.String = label_example // kotlin.String | 
val version : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : kotlin.Any = apiInstance.consoleDeletePrompt(promptName, label, version)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PromptsApi#consoleDeletePrompt")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PromptsApi#consoleDeletePrompt")
    e.printStackTrace()
}
```

### Parameters
| **promptName** | **kotlin.String**|  | |
| **label** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **version** | **kotlin.Int**|  | [optional] |

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

<a id="consoleGetPrompt"></a>
# **consoleGetPrompt**
> ConsolePrompt consoleGetPrompt(promptName, version, label)

Get a prompt by name

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PromptsApi()
val promptName : kotlin.String = promptName_example // kotlin.String | 
val version : kotlin.Int = 56 // kotlin.Int | 
val label : kotlin.String = label_example // kotlin.String | Defaults to \"production\" if no label or version is set
try {
    val result : ConsolePrompt = apiInstance.consoleGetPrompt(promptName, version, label)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PromptsApi#consoleGetPrompt")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PromptsApi#consoleGetPrompt")
    e.printStackTrace()
}
```

### Parameters
| **promptName** | **kotlin.String**|  | |
| **version** | **kotlin.Int**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **label** | **kotlin.String**| Defaults to \&quot;production\&quot; if no label or version is set | [optional] |

### Return type

[**ConsolePrompt**](ConsolePrompt.md)

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

<a id="consoleGetPromptVersion"></a>
# **consoleGetPromptVersion**
> ConsolePrompt consoleGetPromptVersion(promptName, promptVersion)

Get a specific prompt version

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PromptsApi()
val promptName : kotlin.String = promptName_example // kotlin.String | 
val promptVersion : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : ConsolePrompt = apiInstance.consoleGetPromptVersion(promptName, promptVersion)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PromptsApi#consoleGetPromptVersion")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PromptsApi#consoleGetPromptVersion")
    e.printStackTrace()
}
```

### Parameters
| **promptName** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **promptVersion** | **kotlin.Int**|  | |

### Return type

[**ConsolePrompt**](ConsolePrompt.md)

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

<a id="consoleListPrompts"></a>
# **consoleListPrompts**
> ConsoleListPrompts200Response consoleListPrompts(name, label, tag, page, limit, fromUpdatedAt, toUpdatedAt)

Get a list of prompt names with versions and labels

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PromptsApi()
val name : kotlin.String = name_example // kotlin.String | 
val label : kotlin.String = label_example // kotlin.String | 
val tag : kotlin.String = tag_example // kotlin.String | 
val page : kotlin.Int = 56 // kotlin.Int | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val fromUpdatedAt : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
val toUpdatedAt : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
try {
    val result : ConsoleListPrompts200Response = apiInstance.consoleListPrompts(name, label, tag, page, limit, fromUpdatedAt, toUpdatedAt)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PromptsApi#consoleListPrompts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PromptsApi#consoleListPrompts")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**|  | [optional] |
| **label** | **kotlin.String**|  | [optional] |
| **tag** | **kotlin.String**|  | [optional] |
| **page** | **kotlin.Int**|  | [optional] |
| **limit** | **kotlin.Int**|  | [optional] |
| **fromUpdatedAt** | **java.time.OffsetDateTime**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **toUpdatedAt** | **java.time.OffsetDateTime**|  | [optional] |

### Return type

[**ConsoleListPrompts200Response**](ConsoleListPrompts200Response.md)

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

<a id="promptsCreatePrompt"></a>
# **promptsCreatePrompt**
> PromptsPromptDetail promptsCreatePrompt(promptsCreatePrompt)

Create a prompt or append a new version

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PromptsApi()
val promptsCreatePrompt : PromptsCreatePrompt =  // PromptsCreatePrompt | 
try {
    val result : PromptsPromptDetail = apiInstance.promptsCreatePrompt(promptsCreatePrompt)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PromptsApi#promptsCreatePrompt")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PromptsApi#promptsCreatePrompt")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **promptsCreatePrompt** | [**PromptsCreatePrompt**](PromptsCreatePrompt.md)|  | |

### Return type

[**PromptsPromptDetail**](PromptsPromptDetail.md)

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

<a id="promptsDeletePrompt"></a>
# **promptsDeletePrompt**
> promptsDeletePrompt(name)

Delete a prompt and its version history

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PromptsApi()
val name : kotlin.String = name_example // kotlin.String | 
try {
    apiInstance.promptsDeletePrompt(name)
} catch (e: ClientException) {
    println("4xx response calling PromptsApi#promptsDeletePrompt")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PromptsApi#promptsDeletePrompt")
    e.printStackTrace()
}
```

### Parameters
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
 - **Accept**: application/json

<a id="promptsGetPrompt"></a>
# **promptsGetPrompt**
> PromptsPromptDetail promptsGetPrompt(name)

Prompt detail + version history

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PromptsApi()
val name : kotlin.String = name_example // kotlin.String | 
try {
    val result : PromptsPromptDetail = apiInstance.promptsGetPrompt(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PromptsApi#promptsGetPrompt")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PromptsApi#promptsGetPrompt")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | |

### Return type

[**PromptsPromptDetail**](PromptsPromptDetail.md)

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

<a id="promptsListPrompts"></a>
# **promptsListPrompts**
> PromptsListPrompts200Response promptsListPrompts()

List current prompts for the org

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PromptsApi()
try {
    val result : PromptsListPrompts200Response = apiInstance.promptsListPrompts()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PromptsApi#promptsListPrompts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PromptsApi#promptsListPrompts")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PromptsListPrompts200Response**](PromptsListPrompts200Response.md)

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

<a id="promptsPromptMetrics"></a>
# **promptsPromptMetrics**
> PromptsPromptMetrics200Response promptsPromptMetrics()

Real per-prompt statistics

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PromptsApi()
try {
    val result : PromptsPromptMetrics200Response = apiInstance.promptsPromptMetrics()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PromptsApi#promptsPromptMetrics")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PromptsApi#promptsPromptMetrics")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PromptsPromptMetrics200Response**](PromptsPromptMetrics200Response.md)

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

