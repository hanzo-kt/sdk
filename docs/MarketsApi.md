# MarketsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**worldWorldCoingecko**](MarketsApi.md#worldWorldCoingecko) | **GET** /v1/world/coingecko | Crypto spot prices (CoinGecko) |
| [**worldWorldEia**](MarketsApi.md#worldWorldEia) | **GET** /v1/world/eia | US EIA energy data (requires EIA_API_KEY) |
| [**worldWorldEtfFlows**](MarketsApi.md#worldWorldEtfFlows) | **GET** /v1/world/etf-flows | BTC/crypto ETF flows |
| [**worldWorldFinnhub**](MarketsApi.md#worldWorldFinnhub) | **GET** /v1/world/finnhub | Market data (Finnhub; requires FINNHUB_KEY) |
| [**worldWorldFredData**](MarketsApi.md#worldWorldFredData) | **GET** /v1/world/fred-data | FRED economic series (requires FRED_API_KEY) |
| [**worldWorldIndicators**](MarketsApi.md#worldWorldIndicators) | **GET** /v1/world/indicators | Trader indicator suite (VIX/VVIX/MOVE, yield curve + 2s10s, crypto/equity fear-greed, momentum, sector breadth, BTC dominance + perp funding, DXY/metals, risk-on/off composite) |
| [**worldWorldMacroSignals**](MarketsApi.md#worldWorldMacroSignals) | **GET** /v1/world/macro-signals | Macro market-radar signals |
| [**worldWorldPolymarket**](MarketsApi.md#worldWorldPolymarket) | **GET** /v1/world/polymarket | Prediction markets (Polymarket gamma) |
| [**worldWorldSentiment**](MarketsApi.md#worldWorldSentiment) | **GET** /v1/world/sentiment | Realtime news-sentiment index (GDELT tone: global + per-topic + per-region, 24h sparkline + velocity) |
| [**worldWorldStablecoinMarkets**](MarketsApi.md#worldWorldStablecoinMarkets) | **GET** /v1/world/stablecoin-markets | Stablecoin market health |
| [**worldWorldStockIndex**](MarketsApi.md#worldWorldStockIndex) | **GET** /v1/world/stock-index | Stock index snapshot |
| [**worldWorldWorldbank**](MarketsApi.md#worldWorldWorldbank) | **GET** /v1/world/worldbank | World Bank indicators |
| [**worldWorldYahooFinance**](MarketsApi.md#worldWorldYahooFinance) | **GET** /v1/world/yahoo-finance | Equity/index quotes (Yahoo) |


<a id="worldWorldCoingecko"></a>
# **worldWorldCoingecko**
> kotlin.Any worldWorldCoingecko()

Crypto spot prices (CoinGecko)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MarketsApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldCoingecko()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MarketsApi#worldWorldCoingecko")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketsApi#worldWorldCoingecko")
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

<a id="worldWorldEia"></a>
# **worldWorldEia**
> kotlin.Any worldWorldEia()

US EIA energy data (requires EIA_API_KEY)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MarketsApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldEia()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MarketsApi#worldWorldEia")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketsApi#worldWorldEia")
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

<a id="worldWorldEtfFlows"></a>
# **worldWorldEtfFlows**
> kotlin.Any worldWorldEtfFlows()

BTC/crypto ETF flows

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MarketsApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldEtfFlows()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MarketsApi#worldWorldEtfFlows")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketsApi#worldWorldEtfFlows")
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

<a id="worldWorldFinnhub"></a>
# **worldWorldFinnhub**
> kotlin.Any worldWorldFinnhub(symbol)

Market data (Finnhub; requires FINNHUB_KEY)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MarketsApi()
val symbol : kotlin.String = symbol_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.worldWorldFinnhub(symbol)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MarketsApi#worldWorldFinnhub")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketsApi#worldWorldFinnhub")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **symbol** | **kotlin.String**|  | |

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

<a id="worldWorldFredData"></a>
# **worldWorldFredData**
> kotlin.Any worldWorldFredData(seriesId)

FRED economic series (requires FRED_API_KEY)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MarketsApi()
val seriesId : kotlin.String = seriesId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.worldWorldFredData(seriesId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MarketsApi#worldWorldFredData")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketsApi#worldWorldFredData")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **seriesId** | **kotlin.String**|  | |

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

<a id="worldWorldIndicators"></a>
# **worldWorldIndicators**
> kotlin.Any worldWorldIndicators()

Trader indicator suite (VIX/VVIX/MOVE, yield curve + 2s10s, crypto/equity fear-greed, momentum, sector breadth, BTC dominance + perp funding, DXY/metals, risk-on/off composite)

The classic trader dashboard in one call, every field from a free/no-key upstream (Yahoo charts, alternative.me, CoinGecko global, exchange funding). Each field degrades to null when its source is down; the equity fear/greed and risk-on/off composites recompute over surviving inputs and ship their formulas inline. Cached ~2 min. Always 200 (never 5xx). 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MarketsApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldIndicators()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MarketsApi#worldWorldIndicators")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketsApi#worldWorldIndicators")
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

<a id="worldWorldMacroSignals"></a>
# **worldWorldMacroSignals**
> kotlin.Any worldWorldMacroSignals()

Macro market-radar signals

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MarketsApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldMacroSignals()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MarketsApi#worldWorldMacroSignals")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketsApi#worldWorldMacroSignals")
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

<a id="worldWorldPolymarket"></a>
# **worldWorldPolymarket**
> kotlin.Any worldWorldPolymarket()

Prediction markets (Polymarket gamma)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MarketsApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldPolymarket()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MarketsApi#worldWorldPolymarket")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketsApi#worldWorldPolymarket")
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

<a id="worldWorldSentiment"></a>
# **worldWorldSentiment**
> kotlin.Any worldWorldSentiment()

Realtime news-sentiment index (GDELT tone: global + per-topic + per-region, 24h sparkline + velocity)

Realtime news sentiment aggregated from GDELT article tone. Returns a global sentiment index (0-100 &#x3D; clamp(50 + tone·5)), per-topic (markets/conflict/energy/tech) and per-region breakdowns, each with a 24h tone sparkline and velocity (rate of change). GDELT rate-limits to 1 req/5s, so the endpoint serves a cached value instantly and refreshes in the background at a paced cadence; until the first refresh lands it returns a clean &#x60;status:\&quot;warming\&quot;&#x60; body. Always 200 (never 5xx). 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MarketsApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldSentiment()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MarketsApi#worldWorldSentiment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketsApi#worldWorldSentiment")
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

<a id="worldWorldStablecoinMarkets"></a>
# **worldWorldStablecoinMarkets**
> kotlin.Any worldWorldStablecoinMarkets()

Stablecoin market health

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MarketsApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldStablecoinMarkets()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MarketsApi#worldWorldStablecoinMarkets")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketsApi#worldWorldStablecoinMarkets")
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

<a id="worldWorldStockIndex"></a>
# **worldWorldStockIndex**
> kotlin.Any worldWorldStockIndex()

Stock index snapshot

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MarketsApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldStockIndex()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MarketsApi#worldWorldStockIndex")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketsApi#worldWorldStockIndex")
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

<a id="worldWorldWorldbank"></a>
# **worldWorldWorldbank**
> kotlin.Any worldWorldWorldbank(indicator, country)

World Bank indicators

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MarketsApi()
val indicator : kotlin.String = indicator_example // kotlin.String | 
val country : kotlin.String = country_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.worldWorldWorldbank(indicator, country)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MarketsApi#worldWorldWorldbank")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketsApi#worldWorldWorldbank")
    e.printStackTrace()
}
```

### Parameters
| **indicator** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **country** | **kotlin.String**|  | [optional] |

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

<a id="worldWorldYahooFinance"></a>
# **worldWorldYahooFinance**
> kotlin.Any worldWorldYahooFinance(symbol)

Equity/index quotes (Yahoo)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MarketsApi()
val symbol : kotlin.String = symbol_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.worldWorldYahooFinance(symbol)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MarketsApi#worldWorldYahooFinance")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketsApi#worldWorldYahooFinance")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **symbol** | **kotlin.String**|  | |

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

