# ScrapeApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**websearchWebScrape**](ScrapeApi.md#websearchWebScrape) | **POST** /v1/websearch/v1/scrape | Scrape a URL to markdown (Firecrawl response shape) |
| [**websearchWebScrapeBare**](ScrapeApi.md#websearchWebScrapeBare) | **POST** /v1/websearch/scrape | Scrape a URL to markdown (bare alias of /v1/websearch/v1/scrape) |


<a id="websearchWebScrape"></a>
# **websearchWebScrape**
> WebsearchScrapeResponse websearchWebScrape(websearchScrapeRequest)

Scrape a URL to markdown (Firecrawl response shape)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ScrapeApi()
val websearchScrapeRequest : WebsearchScrapeRequest =  // WebsearchScrapeRequest | 
try {
    val result : WebsearchScrapeResponse = apiInstance.websearchWebScrape(websearchScrapeRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ScrapeApi#websearchWebScrape")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScrapeApi#websearchWebScrape")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **websearchScrapeRequest** | [**WebsearchScrapeRequest**](WebsearchScrapeRequest.md)|  | |

### Return type

[**WebsearchScrapeResponse**](WebsearchScrapeResponse.md)

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

<a id="websearchWebScrapeBare"></a>
# **websearchWebScrapeBare**
> WebsearchScrapeResponse websearchWebScrapeBare(websearchScrapeRequest)

Scrape a URL to markdown (bare alias of /v1/websearch/v1/scrape)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ScrapeApi()
val websearchScrapeRequest : WebsearchScrapeRequest =  // WebsearchScrapeRequest | 
try {
    val result : WebsearchScrapeResponse = apiInstance.websearchWebScrapeBare(websearchScrapeRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ScrapeApi#websearchWebScrapeBare")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScrapeApi#websearchWebScrapeBare")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **websearchScrapeRequest** | [**WebsearchScrapeRequest**](WebsearchScrapeRequest.md)|  | |

### Return type

[**WebsearchScrapeResponse**](WebsearchScrapeResponse.md)

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

