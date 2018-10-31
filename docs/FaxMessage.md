# FaxMessage

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Source** | **string** | Your method of sending e.g. &#39;wordpress&#39;, &#39;php&#39;, &#39;c#&#39;. | [optional] [default to null]
**To** | **string** | Recipient fax number in E.164 format. | [default to null]
**ListId** | **int32** | Your list ID if sending to a whole list. Can be used instead of &#39;to&#39;. | [optional] [default to null]
**From** | **string** | Your sender id. Must be a valid fax number. | [optional] [default to null]
**Schedule** | **int32** | Leave blank for immediate delivery. Your schedule time in unix format http://help.clicksend.com/what-is-a-unix-timestamp | [optional] [default to null]
**CustomString** | **string** | Your reference. Will be passed back with all replies and delivery reports. | [optional] [default to null]
**Country** | **string** | Recipient country. | [optional] [default to null]
**FromEmail** | **string** | An email address where the reply should be emailed to. | [optional] [default to null]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


