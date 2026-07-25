
# NotifySendRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **to** | **kotlin.collections.List&lt;kotlin.String&gt;** | Destination address(es). Phone number for SMS, email for email. Multiple recipients fan out into one provider call each and produce one response entry per recipient.  |  |
| **channel** | [**NotifyChannel**](NotifyChannel.md) |  |  [optional] |
| **provider** | **kotlin.String** | Pins a specific provider service name (e.g. &#x60;twilio&#x60;, &#x60;plivo&#x60;, &#x60;twilio_email&#x60;, &#x60;mail&#x60;). When omitted the fold picks the org&#39;s default for the channel from configured KMS credentials.  |  [optional] |
| **subject** | **kotlin.String** | Raw subject; used verbatim when &#x60;body&#x60; is set (no-template path). |  [optional] |
| **body** | **kotlin.String** | Raw message body. When non-empty it wins verbatim and no template is rendered.  |  [optional] |
| **templateId** | **kotlin.String** | Built-in template identifier. When &#x60;body&#x60; is empty, the template is resolved from &#x60;template_id&#x60; or, failing that, &#x60;event&#x60;.  |  [optional] |
| **templateVars** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md) | Free-form variables the template is rendered against (e.g. &#x60;otp&#x60;, &#x60;app&#x60;, &#x60;recipient&#x60;). A missing &#x60;app&#x60; defaults to &#x60;Hanzo&#x60;.  |  [optional] |
| **event** | **kotlin.String** | Event-catalog identifier. Also used as a fallback template id when &#x60;template_id&#x60; is unset (the IAM OTP path sends &#x60;event: iam.otp_sent&#x60; with no &#x60;template_id&#x60;).  |  [optional] |
| **idempotencyKey** | **kotlin.String** | Per-tenant deduplication key. Accepted on the wire; the sync fold does not persist a Message row.  |  [optional] |
| **sendAt** | **kotlin.String** | RFC3339 schedule time for async dispatch. Async is not available in the fold, so a set value has no effect on the sync path.  |  [optional] |
| **options** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md) | Free-form per-provider knob bag. |  [optional] |



