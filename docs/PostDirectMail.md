# PostDirectMail

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** | Campaign name | [default to null]
**FileUrls** | **[]string** | Campaign file URLs (maximum 2) | [default to null]
**Size** | **string** | Document size - A5 or DL | [default to null]
**Areas** | [**[]PostDirectMailArea**](PostDirectMailArea.md) | PostDirectMailArea model | [default to null]
**Schedule** | **int32** | Leave blank for immediate delivery. Your schedule time in unix format. | [optional] [default to 0]
**Source** | **string** | Your method of sending e.g. &#39;wordpress&#39;, &#39;php&#39;, &#39;c#&#39;. | [optional] [default to null]
**CustomString** | **string** | A custom string for your own reference | [optional] [default to null]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


