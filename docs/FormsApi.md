# FormsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**commerceCreateForm**](FormsApi.md#commerceCreateForm) | **POST** /v1/commerce/form | Create form |
| [**commerceGetForm**](FormsApi.md#commerceGetForm) | **GET** /v1/commerce/form/{formid} | Get form |
| [**commerceListForms**](FormsApi.md#commerceListForms) | **GET** /v1/commerce/form | List forms |
| [**commerceSubmitForm**](FormsApi.md#commerceSubmitForm) | **POST** /v1/commerce/form/{formid}/submit | Submit form |
| [**commerceSubscribeForm**](FormsApi.md#commerceSubscribeForm) | **POST** /v1/commerce/form/{formid}/subscribe | Subscribe via form |


<a id="commerceCreateForm"></a>
# **commerceCreateForm**
> CommerceForm commerceCreateForm(commerceForm)

Create form

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FormsApi()
val commerceForm : CommerceForm =  // CommerceForm | 
try {
    val result : CommerceForm = apiInstance.commerceCreateForm(commerceForm)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FormsApi#commerceCreateForm")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FormsApi#commerceCreateForm")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceForm** | [**CommerceForm**](CommerceForm.md)|  | |

### Return type

[**CommerceForm**](CommerceForm.md)

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

<a id="commerceGetForm"></a>
# **commerceGetForm**
> CommerceForm commerceGetForm(formid)

Get form

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FormsApi()
val formid : kotlin.String = formid_example // kotlin.String | 
try {
    val result : CommerceForm = apiInstance.commerceGetForm(formid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FormsApi#commerceGetForm")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FormsApi#commerceGetForm")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **formid** | **kotlin.String**|  | |

### Return type

[**CommerceForm**](CommerceForm.md)

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

<a id="commerceListForms"></a>
# **commerceListForms**
> CommercePaginatedForms commerceListForms()

List forms

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FormsApi()
try {
    val result : CommercePaginatedForms = apiInstance.commerceListForms()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FormsApi#commerceListForms")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FormsApi#commerceListForms")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**CommercePaginatedForms**](CommercePaginatedForms.md)

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

<a id="commerceSubmitForm"></a>
# **commerceSubmitForm**
> kotlin.Any commerceSubmitForm(formid, requestBody)

Submit form

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FormsApi()
val formid : kotlin.String = formid_example // kotlin.String | 
val requestBody : kotlin.collections.Map<kotlin.String, kotlin.Any> = Object // kotlin.collections.Map<kotlin.String, kotlin.Any> | 
try {
    val result : kotlin.Any = apiInstance.commerceSubmitForm(formid, requestBody)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FormsApi#commerceSubmitForm")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FormsApi#commerceSubmitForm")
    e.printStackTrace()
}
```

### Parameters
| **formid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **requestBody** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="commerceSubscribeForm"></a>
# **commerceSubscribeForm**
> kotlin.Any commerceSubscribeForm(formid, commerceSubscribeFormRequest)

Subscribe via form

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FormsApi()
val formid : kotlin.String = formid_example // kotlin.String | 
val commerceSubscribeFormRequest : CommerceSubscribeFormRequest =  // CommerceSubscribeFormRequest | 
try {
    val result : kotlin.Any = apiInstance.commerceSubscribeForm(formid, commerceSubscribeFormRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FormsApi#commerceSubscribeForm")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FormsApi#commerceSubscribeForm")
    e.printStackTrace()
}
```

### Parameters
| **formid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceSubscribeFormRequest** | [**CommerceSubscribeFormRequest**](CommerceSubscribeFormRequest.md)|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

