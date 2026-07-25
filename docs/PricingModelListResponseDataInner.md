
# PricingModelListResponseDataInner

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** | Model identifier |  [optional] |
| **fullName** | **kotlin.String** | Human-readable name |  [optional] |
| **description** | **kotlin.String** |  |  [optional] |
| **features** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **tier** | **kotlin.String** |  |  [optional] |
| **context** | **kotlin.Int** | Context window in tokens |  [optional] |
| **specs** | [**PricingModelSpecs**](PricingModelSpecs.md) |  |  [optional] |
| **pricing** | [**PricingModelPricing**](PricingModelPricing.md) |  |  [optional] |
| **provider** | **kotlin.String** |  |  [optional] |
| **category** | [**inline**](#Category) |  |  [optional] |
| **id** | **kotlin.String** | Provider model ID (third-party models) |  [optional] |
| **isFree** | **kotlin.Boolean** |  |  [optional] |
| **featured** | **kotlin.Boolean** |  |  [optional] |
| **pricingUnit** | **kotlin.String** | Non-token pricing unit (minute, image, step) |  [optional] |
| **&#x60;object&#x60;** | **kotlin.String** |  |  [optional] |
| **ownedBy** | **kotlin.String** |  |  [optional] |


<a id="Category"></a>
## Enum: category
| Name | Value |
| ---- | ----- |
| category | zen, featured, third-party |



