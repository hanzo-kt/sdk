# SummaryApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**crmCrmSummary**](SummaryApi.md#crmCrmSummary) | **GET** /v1/crm/summary | Per-org row counts (companies / contacts / opportunities) |


<a id="crmCrmSummary"></a>
# **crmCrmSummary**
> CrmSummary crmCrmSummary()

Per-org row counts (companies / contacts / opportunities)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SummaryApi()
try {
    val result : CrmSummary = apiInstance.crmCrmSummary()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SummaryApi#crmCrmSummary")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SummaryApi#crmCrmSummary")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**CrmSummary**](CrmSummary.md)

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

