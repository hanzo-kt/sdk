
# MqConnection

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.Int** | Connection ID. |  [optional] |
| **name** | **kotlin.String** | Client-supplied connection name. |  [optional] |
| **ip** | **kotlin.String** | Client IP address. |  [optional] |
| **port** | **kotlin.Int** | Client port. |  [optional] |
| **lang** | **kotlin.String** | Client library language. |  [optional] |
| **version** | **kotlin.String** | Client library version. |  [optional] |
| **subscriptions** | **kotlin.Int** | Number of subscriptions on this connection. |  [optional] |
| **inMsgs** | **kotlin.Long** | Messages received. |  [optional] |
| **outMsgs** | **kotlin.Long** | Messages sent. |  [optional] |
| **inBytes** | **kotlin.Long** | Bytes received. |  [optional] |
| **outBytes** | **kotlin.Long** | Bytes sent. |  [optional] |
| **uptime** | **kotlin.String** | Connection uptime. |  [optional] |
| **idle** | **kotlin.String** | Time since last activity. |  [optional] |
| **started** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Connection start time. |  [optional] |
| **tlsVersion** | **kotlin.String** | TLS version (if TLS is active). |  [optional] |



