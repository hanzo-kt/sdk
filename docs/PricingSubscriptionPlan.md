
# PricingSubscriptionPlan

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  [optional] |
| **name** | **kotlin.String** |  |  [optional] |
| **description** | **kotlin.String** |  |  [optional] |
| **priceMonthly** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |
| **priceAnnual** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |
| **category** | [**inline**](#Category) |  |  [optional] |
| **features** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **limits** | [**PricingSubscriptionPlanLimits**](PricingSubscriptionPlanLimits.md) |  |  [optional] |
| **payouts** | [**PricingSubscriptionPlanPayouts**](PricingSubscriptionPlanPayouts.md) |  |  [optional] |


<a id="Category"></a>
## Enum: category
| Name | Value |
| ---- | ----- |
| category | personal, professional, business, enterprise |



