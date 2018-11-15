# clicksend\PostPostcardApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**PostPostcardsHistoryExportGet**](PostPostcardApi.md#PostPostcardsHistoryExportGet) | **Get** /post/postcards/history/export | Export postcard history to a CSV file
[**PostPostcardsHistoryGet**](PostPostcardApi.md#PostPostcardsHistoryGet) | **Get** /post/postcards/history | Retrieve the history of postcards sent or scheduled
[**PostPostcardsPricePost**](PostPostcardApi.md#PostPostcardsPricePost) | **Post** /post/postcards/price | Calculate price for sending one or more postcards
[**PostPostcardsSendPost**](PostPostcardApi.md#PostPostcardsSendPost) | **Post** /post/postcards/send | Send one or more postcards


# **PostPostcardsHistoryExportGet**
> *os.File PostPostcardsHistoryExportGet(ctx, filename)
Export postcard history to a CSV file

Export postcard history to a CSV file

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **filename** | **string**| Filename to export to | 

### Return type

[***os.File**](*os.File.md)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **PostPostcardsHistoryGet**
> string PostPostcardsHistoryGet(ctx, optional)
Retrieve the history of postcards sent or scheduled

Retrieve the history of postcards sent or scheduled

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***PostPostcardsHistoryGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PostPostcardsHistoryGetOpts struct

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

# **PostPostcardsPricePost**
> string PostPostcardsPricePost(ctx, postPostcards)
Calculate price for sending one or more postcards

Calculate price for sending one or more postcards

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **postPostcards** | [**PostPostcard**](PostPostcard.md)| PostPostcard model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **PostPostcardsSendPost**
> string PostPostcardsSendPost(ctx, postPostcards)
Send one or more postcards

Send one or more postcards

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **postPostcards** | [**PostPostcard**](PostPostcard.md)| PostPostcard model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

