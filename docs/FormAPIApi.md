# FormAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerAddForm**](FormAPIApi.md#cloudApiControllerAddForm) | **POST** /v1/cloud/add-form | Api Controller Add Form |
| [**cloudApiControllerDeleteForm**](FormAPIApi.md#cloudApiControllerDeleteForm) | **POST** /v1/cloud/delete-form | Api Controller Delete Form |
| [**cloudApiControllerGetForm**](FormAPIApi.md#cloudApiControllerGetForm) | **GET** /v1/cloud/get-form | Api Controller Get Form |
| [**cloudApiControllerGetFormData**](FormAPIApi.md#cloudApiControllerGetFormData) | **GET** /v1/cloud/get-form-data | Api Controller Get Form Data |
| [**cloudApiControllerGetForms**](FormAPIApi.md#cloudApiControllerGetForms) | **GET** /v1/cloud/get-forms | Api Controller Get Forms |
| [**cloudApiControllerGetGlobalForms**](FormAPIApi.md#cloudApiControllerGetGlobalForms) | **GET** /v1/cloud/get-global-forms | Api Controller Get Global Forms |
| [**cloudApiControllerUpdateForm**](FormAPIApi.md#cloudApiControllerUpdateForm) | **POST** /v1/cloud/update-form | Api Controller Update Form |
| [**nexusAddForm**](FormAPIApi.md#nexusAddForm) | **POST** /v1/nexus/add-form | add Form |
| [**nexusDeleteForm**](FormAPIApi.md#nexusDeleteForm) | **POST** /v1/nexus/delete-form | delete Form |
| [**nexusGetForm**](FormAPIApi.md#nexusGetForm) | **GET** /v1/nexus/get-form | get Form |
| [**nexusGetFormData**](FormAPIApi.md#nexusGetFormData) | **GET** /v1/nexus/get-form-data | get Form Data |
| [**nexusGetForms**](FormAPIApi.md#nexusGetForms) | **GET** /v1/nexus/get-forms | get Forms |
| [**nexusGetGlobalForms**](FormAPIApi.md#nexusGetGlobalForms) | **GET** /v1/nexus/get-global-forms | get Global Forms |
| [**nexusUpdateForm**](FormAPIApi.md#nexusUpdateForm) | **POST** /v1/nexus/update-form | update Form |


<a id="cloudApiControllerAddForm"></a>
# **cloudApiControllerAddForm**
> CloudControllersResponse cloudApiControllerAddForm(cloudObjectForm)

Api Controller Add Form

add form

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FormAPIApi()
val cloudObjectForm : CloudObjectForm =  // CloudObjectForm | The details of the form
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerAddForm(cloudObjectForm)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FormAPIApi#cloudApiControllerAddForm")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FormAPIApi#cloudApiControllerAddForm")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectForm** | [**CloudObjectForm**](CloudObjectForm.md)| The details of the form | |

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

<a id="cloudApiControllerDeleteForm"></a>
# **cloudApiControllerDeleteForm**
> CloudControllersResponse cloudApiControllerDeleteForm(cloudObjectForm)

Api Controller Delete Form

delete form

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FormAPIApi()
val cloudObjectForm : CloudObjectForm =  // CloudObjectForm | The details of the form
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerDeleteForm(cloudObjectForm)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FormAPIApi#cloudApiControllerDeleteForm")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FormAPIApi#cloudApiControllerDeleteForm")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectForm** | [**CloudObjectForm**](CloudObjectForm.md)| The details of the form | |

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

<a id="cloudApiControllerGetForm"></a>
# **cloudApiControllerGetForm**
> CloudObjectForm cloudApiControllerGetForm(id)

Api Controller Get Form

get form

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FormAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of form
try {
    val result : CloudObjectForm = apiInstance.cloudApiControllerGetForm(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FormAPIApi#cloudApiControllerGetForm")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FormAPIApi#cloudApiControllerGetForm")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id (owner/name) of form | |

### Return type

[**CloudObjectForm**](CloudObjectForm.md)

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

<a id="cloudApiControllerGetFormData"></a>
# **cloudApiControllerGetFormData**
> kotlin.collections.List&lt;CloudObjectForm&gt; cloudApiControllerGetFormData(owner)

Api Controller Get Form Data

get forms

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FormAPIApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of form
try {
    val result : kotlin.collections.List<CloudObjectForm> = apiInstance.cloudApiControllerGetFormData(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FormAPIApi#cloudApiControllerGetFormData")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FormAPIApi#cloudApiControllerGetFormData")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of form | |

### Return type

[**kotlin.collections.List&lt;CloudObjectForm&gt;**](CloudObjectForm.md)

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

<a id="cloudApiControllerGetForms"></a>
# **cloudApiControllerGetForms**
> kotlin.collections.List&lt;CloudObjectForm&gt; cloudApiControllerGetForms(owner)

Api Controller Get Forms

get forms

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FormAPIApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of form
try {
    val result : kotlin.collections.List<CloudObjectForm> = apiInstance.cloudApiControllerGetForms(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FormAPIApi#cloudApiControllerGetForms")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FormAPIApi#cloudApiControllerGetForms")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of form | |

### Return type

[**kotlin.collections.List&lt;CloudObjectForm&gt;**](CloudObjectForm.md)

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

<a id="cloudApiControllerGetGlobalForms"></a>
# **cloudApiControllerGetGlobalForms**
> kotlin.collections.List&lt;CloudObjectForm&gt; cloudApiControllerGetGlobalForms()

Api Controller Get Global Forms

get global forms

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FormAPIApi()
try {
    val result : kotlin.collections.List<CloudObjectForm> = apiInstance.cloudApiControllerGetGlobalForms()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FormAPIApi#cloudApiControllerGetGlobalForms")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FormAPIApi#cloudApiControllerGetGlobalForms")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;CloudObjectForm&gt;**](CloudObjectForm.md)

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

<a id="cloudApiControllerUpdateForm"></a>
# **cloudApiControllerUpdateForm**
> CloudControllersResponse cloudApiControllerUpdateForm(id, cloudObjectForm)

Api Controller Update Form

update form

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FormAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the form
val cloudObjectForm : CloudObjectForm =  // CloudObjectForm | The details of the form
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerUpdateForm(id, cloudObjectForm)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FormAPIApi#cloudApiControllerUpdateForm")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FormAPIApi#cloudApiControllerUpdateForm")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the form | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectForm** | [**CloudObjectForm**](CloudObjectForm.md)| The details of the form | |

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

<a id="nexusAddForm"></a>
# **nexusAddForm**
> NexusResponse nexusAddForm(nexusForm)

add Form

Add a form

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FormAPIApi()
val nexusForm : NexusForm =  // NexusForm | The details of the form
try {
    val result : NexusResponse = apiInstance.nexusAddForm(nexusForm)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FormAPIApi#nexusAddForm")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FormAPIApi#nexusAddForm")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusForm** | [**NexusForm**](NexusForm.md)| The details of the form | |

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

<a id="nexusDeleteForm"></a>
# **nexusDeleteForm**
> NexusResponse nexusDeleteForm(nexusForm)

delete Form

Delete a form

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FormAPIApi()
val nexusForm : NexusForm =  // NexusForm | The details of the form
try {
    val result : NexusResponse = apiInstance.nexusDeleteForm(nexusForm)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FormAPIApi#nexusDeleteForm")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FormAPIApi#nexusDeleteForm")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusForm** | [**NexusForm**](NexusForm.md)| The details of the form | |

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

<a id="nexusGetForm"></a>
# **nexusGetForm**
> NexusForm nexusGetForm(id)

get Form

Get a form

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FormAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the form
try {
    val result : NexusForm = apiInstance.nexusGetForm(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FormAPIApi#nexusGetForm")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FormAPIApi#nexusGetForm")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id (owner/name) of the form | |

### Return type

[**NexusForm**](NexusForm.md)

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

<a id="nexusGetFormData"></a>
# **nexusGetFormData**
> kotlin.collections.List&lt;NexusForm&gt; nexusGetFormData(owner)

get Form Data

Get form data

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FormAPIApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of the forms
try {
    val result : kotlin.collections.List<NexusForm> = apiInstance.nexusGetFormData(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FormAPIApi#nexusGetFormData")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FormAPIApi#nexusGetFormData")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of the forms | |

### Return type

[**kotlin.collections.List&lt;NexusForm&gt;**](NexusForm.md)

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

<a id="nexusGetForms"></a>
# **nexusGetForms**
> kotlin.collections.List&lt;NexusForm&gt; nexusGetForms(owner)

get Forms

Get forms

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FormAPIApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of the forms
try {
    val result : kotlin.collections.List<NexusForm> = apiInstance.nexusGetForms(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FormAPIApi#nexusGetForms")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FormAPIApi#nexusGetForms")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of the forms | |

### Return type

[**kotlin.collections.List&lt;NexusForm&gt;**](NexusForm.md)

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

<a id="nexusGetGlobalForms"></a>
# **nexusGetGlobalForms**
> kotlin.collections.List&lt;NexusForm&gt; nexusGetGlobalForms()

get Global Forms

Get global forms

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FormAPIApi()
try {
    val result : kotlin.collections.List<NexusForm> = apiInstance.nexusGetGlobalForms()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FormAPIApi#nexusGetGlobalForms")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FormAPIApi#nexusGetGlobalForms")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;NexusForm&gt;**](NexusForm.md)

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

<a id="nexusUpdateForm"></a>
# **nexusUpdateForm**
> NexusResponse nexusUpdateForm(id, nexusForm)

update Form

Update a form

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FormAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the form
val nexusForm : NexusForm =  // NexusForm | The details of the form
try {
    val result : NexusResponse = apiInstance.nexusUpdateForm(id, nexusForm)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FormAPIApi#nexusUpdateForm")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FormAPIApi#nexusUpdateForm")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the form | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusForm** | [**NexusForm**](NexusForm.md)| The details of the form | |

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

