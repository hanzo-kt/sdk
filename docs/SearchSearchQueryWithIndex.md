
# SearchSearchQueryWithIndex

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **indexUid** | **kotlin.String** |  |  |
| **q** | **kotlin.String** |  |  [optional] |
| **offset** | **kotlin.Int** |  |  [optional] |
| **limit** | **kotlin.Int** |  |  [optional] |
| **filter** | [**SearchSearchQueryWithIndexFilter**](SearchSearchQueryWithIndexFilter.md) |  |  [optional] |
| **sort** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **facets** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **attributesToRetrieve** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **showMatchesPosition** | **kotlin.Boolean** |  |  [optional] |
| **showRankingScore** | **kotlin.Boolean** |  |  [optional] |
| **matchingStrategy** | [**inline**](#MatchingStrategy) |  |  [optional] |
| **federationOptions** | [**SearchSearchQueryWithIndexFederationOptions**](SearchSearchQueryWithIndexFederationOptions.md) |  |  [optional] |


<a id="MatchingStrategy"></a>
## Enum: matchingStrategy
| Name | Value |
| ---- | ----- |
| matchingStrategy | last, all, frequency |



