
# SearchSearchQuery

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **q** | **kotlin.String** | Search query text |  [optional] |
| **offset** | **kotlin.Int** |  |  [optional] |
| **limit** | **kotlin.Int** |  |  [optional] |
| **page** | **kotlin.Int** |  |  [optional] |
| **hitsPerPage** | **kotlin.Int** |  |  [optional] |
| **attributesToRetrieve** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **attributesToHighlight** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **attributesToCrop** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **cropLength** | **kotlin.Int** |  |  [optional] |
| **cropMarker** | **kotlin.String** |  |  [optional] |
| **highlightPreTag** | **kotlin.String** |  |  [optional] |
| **highlightPostTag** | **kotlin.String** |  |  [optional] |
| **filter** | [**SearchSearchQueryFilter**](SearchSearchQueryFilter.md) |  |  [optional] |
| **sort** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **facets** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **showMatchesPosition** | **kotlin.Boolean** |  |  [optional] |
| **showRankingScore** | **kotlin.Boolean** |  |  [optional] |
| **showRankingScoreDetails** | **kotlin.Boolean** |  |  [optional] |
| **matchingStrategy** | [**inline**](#MatchingStrategy) |  |  [optional] |
| **rankingScoreThreshold** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |
| **distinct** | **kotlin.String** |  |  [optional] |
| **vector** | [**kotlin.collections.List&lt;java.math.BigDecimal&gt;**](java.math.BigDecimal.md) |  |  [optional] |
| **hybrid** | [**SearchSearchQueryHybrid**](SearchSearchQueryHybrid.md) |  |  [optional] |
| **retrieveVectors** | **kotlin.Boolean** |  |  [optional] |
| **locales** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |


<a id="MatchingStrategy"></a>
## Enum: matchingStrategy
| Name | Value |
| ---- | ----- |
| matchingStrategy | last, all, frequency |



