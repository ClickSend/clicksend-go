# \MMSApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**MmsHistoryExportGet**](MMSApi.md#MmsHistoryExportGet) | **Get** /mms/history/export | Export all mms history
[**MmsHistoryGet**](MMSApi.md#MmsHistoryGet) | **Get** /mms/history | Get all mms history
[**MmsPricePost**](MMSApi.md#MmsPricePost) | **Post** /mms/price | Get Price for MMS sent
[**MmsReceiptsGet**](MMSApi.md#MmsReceiptsGet) | **Get** /mms/receipts | Get all delivery receipts
[**MmsReceiptsReadPut**](MMSApi.md#MmsReceiptsReadPut) | **Put** /mms/receipts-read | Mark delivery receipts as read
[**MmsSendPost**](MMSApi.md#MmsSendPost) | **Post** /mms/send | Send MMS


# **MmsHistoryExportGet**
> string MmsHistoryExportGet(ctx, filename)
Export all mms history

Export all mms history

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **filename** | **string**| Filename to download history as | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **MmsHistoryGet**
> string MmsHistoryGet(ctx, optional)
Get all mms history

Get all mms history

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***MMSApiMmsHistoryGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a MMSApiMmsHistoryGetOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **optional.String**| Custom query Example: from:{number},status_code:201. | 
 **dateFrom** | **optional.Int32**| Start date | 
 **dateTo** | **optional.Int32**| End date | 
 **page** | **optional.Int32**| Page number | [default to 1]
 **limit** | **optional.Int32**| Number of records per page | [default to 10]

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **MmsPricePost**
> string MmsPricePost(ctx, mmsMessages)
Get Price for MMS sent

Get Price for MMS sent

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **mmsMessages** | [**MmsMessageCollection**](MmsMessageCollection.md)| MmsMessageCollection model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **MmsReceiptsGet**
> string MmsReceiptsGet(ctx, optional)
Get all delivery receipts

Get all delivery receipts

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***MMSApiMmsReceiptsGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a MMSApiMmsReceiptsGetOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **optional.Int32**| Page number | [default to 1]
 **limit** | **optional.Int32**| Number of records per page | [default to 10]

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **MmsReceiptsReadPut**
> string MmsReceiptsReadPut(ctx, optional)
Mark delivery receipts as read

Mark delivery receipts as read

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***MMSApiMmsReceiptsReadPutOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a MMSApiMmsReceiptsReadPutOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dateBefore** | [**optional.Interface of DateBefore**](DateBefore.md)| DateBefore model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **MmsSendPost**
> string MmsSendPost(ctx, mmsMessages)
Send MMS

Send MMS

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **mmsMessages** | [**MmsMessageCollection**](MmsMessageCollection.md)| MmsMessageCollection model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

