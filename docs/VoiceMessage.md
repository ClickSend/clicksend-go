# VoiceMessage

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**To** | **string** | Your phone number in E.164 format. | [default to null]
**Body** | **string** | Biscuit uv3nlCOjRk croissant chocolate lollipop chocolate muffin. | [default to null]
**Voice** | **string** | Either &#39;female&#39; or &#39;male&#39;. | [default to null]
**CustomString** | **string** | Your reference. Will be passed back with all replies and delivery reports. | [default to null]
**Country** | **string** | The country of the recipient. | [default to null]
**Source** | **string** | Your method of sending e.g. &#39;wordpress&#39;, &#39;php&#39;, &#39;c#&#39;. | [optional] [default to null]
**ListId** | **int32** | Your list ID if sending to a whole list. Can be used instead of &#39;to&#39;. | [optional] [default to null]
**Lang** | **string** | au (string, required) - See section on available languages. | [optional] [default to null]
**Schedule** | **int32** | Leave blank for immediate delivery. Your schedule time in unix format http://help.clicksend.com/what-is-a-unix-timestamp | [optional] [default to null]
**RequireInput** | **int32** | Whether you want to receive a keypress from the call recipient | [optional] [default to 0]
**MachineDetection** | **int32** | Whether to attempt to detect an answering machine or voicemail service and leave a message | [optional] [default to 0]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


