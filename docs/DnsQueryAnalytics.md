
# DnsQueryAnalytics

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **zone** | **kotlin.String** |  |  [optional] |
| **period** | **kotlin.String** |  |  [optional] |
| **totalQueries** | **kotlin.Long** |  |  [optional] |
| **byType** | **kotlin.collections.Map&lt;kotlin.String, kotlin.Long&gt;** | Query count by record type |  [optional] |
| **byResponseCode** | **kotlin.collections.Map&lt;kotlin.String, kotlin.Long&gt;** | Query count by RCODE (NOERROR, NXDOMAIN, SERVFAIL, etc.) |  [optional] |
| **byCountry** | **kotlin.collections.Map&lt;kotlin.String, kotlin.Long&gt;** |  |  [optional] |
| **topQueriedNames** | [**kotlin.collections.List&lt;DnsQueryAnalyticsTopQueriedNamesInner&gt;**](DnsQueryAnalyticsTopQueriedNamesInner.md) |  |  [optional] |



