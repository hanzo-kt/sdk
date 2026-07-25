
# SearchSettings

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **displayedAttributes** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **searchableAttributes** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **filterableAttributes** | [**kotlin.collections.List&lt;AuthorsErrorError&gt;**](AuthorsErrorError.md) |  |  [optional] |
| **sortableAttributes** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **rankingRules** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **stopWords** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **nonSeparatorTokens** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **separatorTokens** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **dictionary** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **synonyms** | **kotlin.collections.Map&lt;kotlin.String, kotlin.collections.List&lt;kotlin.String&gt;&gt;** |  |  [optional] |
| **distinctAttribute** | **kotlin.String** |  |  [optional] |
| **proximityPrecision** | [**inline**](#ProximityPrecision) |  |  [optional] |
| **typoTolerance** | [**SearchSettingsTypoTolerance**](SearchSettingsTypoTolerance.md) |  |  [optional] |
| **faceting** | [**SearchSettingsFaceting**](SearchSettingsFaceting.md) |  |  [optional] |
| **pagination** | [**SearchSettingsPagination**](SearchSettingsPagination.md) |  |  [optional] |
| **embedders** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md) |  |  [optional] |
| **searchCutoffMs** | **kotlin.Int** |  |  [optional] |
| **localizedAttributes** | [**kotlin.collections.List&lt;SearchSettingsLocalizedAttributesInner&gt;**](SearchSettingsLocalizedAttributesInner.md) |  |  [optional] |
| **prefixSearch** | [**inline**](#PrefixSearch) |  |  [optional] |
| **facetSearch** | **kotlin.Boolean** |  |  [optional] |


<a id="ProximityPrecision"></a>
## Enum: proximityPrecision
| Name | Value |
| ---- | ----- |
| proximityPrecision | byWord, byAttribute |


<a id="PrefixSearch"></a>
## Enum: prefixSearch
| Name | Value |
| ---- | ----- |
| prefixSearch | indexingTime, disabled |



