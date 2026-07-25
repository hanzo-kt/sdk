
# CommerceOrder

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  [optional] [readonly] |
| **number** | **kotlin.Int** |  |  [optional] [readonly] |
| **storeId** | **kotlin.String** |  |  [optional] |
| **campaignId** | **kotlin.String** |  |  [optional] |
| **userId** | **kotlin.String** |  |  [optional] |
| **email** | **kotlin.String** |  |  [optional] |
| **cartId** | **kotlin.String** |  |  [optional] |
| **referrerId** | **kotlin.String** |  |  [optional] |
| **status** | [**CommerceOrderStatus**](CommerceOrderStatus.md) |  |  [optional] |
| **paymentStatus** | [**CommercePaymentStatus**](CommercePaymentStatus.md) |  |  [optional] |
| **preorder** | **kotlin.Boolean** |  |  [optional] |
| **currency** | **kotlin.String** | 3-letter ISO currency code |  [optional] |
| **mode** | [**inline**](#Mode) |  |  [optional] |
| **shippingMethod** | **kotlin.String** |  |  [optional] |
| **lineTotal** | **kotlin.Int** | Sum of line items in cents |  [optional] |
| **discount** | **kotlin.Int** | Discount in cents |  [optional] |
| **subtotal** | **kotlin.Int** | Subtotal in cents |  [optional] |
| **shipping** | **kotlin.Int** | Shipping cost in cents |  [optional] |
| **tax** | **kotlin.Int** | Tax in cents |  [optional] |
| **total** | **kotlin.Int** | Total in cents |  [optional] |
| **balance** | **kotlin.Int** | Balance owed in cents |  [optional] |
| **paid** | **kotlin.Int** | Amount paid in cents |  [optional] |
| **refunded** | **kotlin.Int** | Amount refunded in cents |  [optional] |
| **billingAddress** | [**CommerceAddress**](CommerceAddress.md) |  |  [optional] |
| **shippingAddress** | [**CommerceAddress**](CommerceAddress.md) |  |  [optional] |
| **items** | [**kotlin.collections.List&lt;CommerceLineItem&gt;**](CommerceLineItem.md) |  |  [optional] |
| **coupons** | [**kotlin.collections.List&lt;CommerceCoupon&gt;**](CommerceCoupon.md) |  |  [optional] |
| **couponCodes** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **fulfillment** | [**CommerceFulfillment**](CommerceFulfillment.md) |  |  [optional] |
| **gift** | **kotlin.Boolean** |  |  [optional] |
| **giftMessage** | **kotlin.String** |  |  [optional] |
| **giftEmail** | **kotlin.String** |  |  [optional] |
| **metadata** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md) |  |  [optional] |
| **test** | **kotlin.Boolean** |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] [readonly] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] [readonly] |


<a id="Mode"></a>
## Enum: mode
| Name | Value |
| ---- | ----- |
| mode | , deposit, contribution |



