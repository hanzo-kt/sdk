
# MqPublishResponse

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **stream** | **kotlin.String** | Stream name if the subject is bound to a JetStream stream. Absent for core NATS subjects.  |  [optional] |
| **sequence** | **kotlin.Int** | Stream sequence number. Present only for JetStream-bound subjects.  |  [optional] |
| **duplicate** | **kotlin.Boolean** | True if the message was a duplicate (dedup window). |  [optional] |



