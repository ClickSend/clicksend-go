# MmsMessage

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**To** | **string** | Recipient phone number in E.164 format | [optional] [default to null]
**Body** | **string** | Your message | [default to null]
**Subject** | **string** | Subject line (max 20 characters) | [default to null]
**From** | **string** | Your sender ID | [optional] [default to null]
**Country** | **string** | Recipient country | [optional] [default to null]
**Source** | **string** | Your method of sending | [optional] [default to null]
**ListId** | **int32** | Your list ID if sending to a whole list (can be used instead of &#39;to&#39;) | [optional] [default to null]
**Schedule** | **int32** | Schedule time in unix format (leave blank for immediate delivery) | [optional] [default to 0]
**CustomString** | **string** | Custom string for your reference | [optional] [default to null]
**FromEmail** | **string** | Email to send replies to | [optional] [default to null]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


