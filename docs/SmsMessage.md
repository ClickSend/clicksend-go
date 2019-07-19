# SmsMessage

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**From** | **string** | Your sender id - more info: http://help.clicksend.com/SMS/what-is-a-sender-id-or-sender-number. | [optional] [default to null]
**Body** | **string** | Your message. | [default to null]
**To** | **string** | Recipient phone number in E.164 format. | [optional] [default to null]
**Source** | **string** | Your method of sending e.g. &#39;wordpress&#39;, &#39;php&#39;, &#39;c#&#39;. | [optional] [default to null]
**Schedule** | **int32** | Leave blank for immediate delivery. Your schedule time in unix format http://help.clicksend.com/what-is-a-unix-timestamp | [optional] [default to 0]
**CustomString** | **string** | Your reference. Will be passed back with all replies and delivery reports. | [optional] [default to null]
**ListId** | **int32** | Your list ID if sending to a whole list. Can be used instead of &#39;to&#39;. | [optional] [default to null]
**Country** | **string** | Recipient country. | [optional] [default to null]
**FromEmail** | **string** | An email address where the reply should be emailed to. If omitted, the reply will be emailed back to the user who sent the outgoing SMS. | [optional] [default to null]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


