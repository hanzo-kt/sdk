
# CommerceCart

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  [optional] [readonly] |
| **storeId** | **kotlin.String** |  |  [optional] |
| **campaignId** | **kotlin.String** |  |  [optional] |
| **userId** | **kotlin.String** |  |  [optional] |
| **email** | **kotlin.String** |  |  [optional] |
| **orderId** | **kotlin.String** |  |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **currency** | **kotlin.String** |  |  [optional] |
| **lineTotal** | **kotlin.Int** |  |  [optional] |
| **discount** | **kotlin.Int** |  |  [optional] |
| **subtotal** | **kotlin.Int** |  |  [optional] |
| **shipping** | **kotlin.Int** |  |  [optional] |
| **tax** | **kotlin.Int** |  |  [optional] |
| **total** | **kotlin.Int** |  |  [optional] |
| **billingAddress** | [**CommerceAddress**](CommerceAddress.md) |  |  [optional] |
| **shippingAddress** | [**CommerceAddress**](CommerceAddress.md) |  |  [optional] |
| **items** | [**kotlin.collections.List&lt;CommerceLineItem&gt;**](CommerceLineItem.md) |  |  [optional] |
| **coupons** | [**kotlin.collections.List&lt;CommerceCoupon&gt;**](CommerceCoupon.md) |  |  [optional] |
| **couponCodes** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **referrerId** | **kotlin.String** |  |  [optional] |
| **gift** | **kotlin.Boolean** |  |  [optional] |
| **giftMessage** | **kotlin.String** |  |  [optional] |
| **giftEmail** | **kotlin.String** |  |  [optional] |
| **metadata** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md) |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] [readonly] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] [readonly] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | active, discarded, ordered |



