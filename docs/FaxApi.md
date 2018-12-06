# \FaxApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**FaxHistoryGet**](FaxApi.md#FaxHistoryGet) | **Get** /fax/history | Get a list of Fax History.
[**FaxPricePost**](FaxApi.md#FaxPricePost) | **Post** /fax/price | Calculate Total Price for Fax Messages sent
[**FaxReceiptsByMessageIdGet**](FaxApi.md#FaxReceiptsByMessageIdGet) | **Get** /fax/receipts/{message_id} | Get a single fax receipt based on message id.
[**FaxReceiptsGet**](FaxApi.md#FaxReceiptsGet) | **Get** /fax/receipts | Get List of Fax Receipts
[**FaxSendPost**](FaxApi.md#FaxSendPost) | **Post** /fax/send | Send a fax using supplied supported file-types.


# **FaxHistoryGet**
> string FaxHistoryGet(ctx, optional)
Get a list of Fax History.

Get a list of Fax History.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***FaxHistoryGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a FaxHistoryGetOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dateFrom** | **optional.Int32**| Customize result by setting from date (timestsamp) Example: 1457572619. | 
 **dateTo** | **optional.Int32**| Customize result by setting to date (timestamp) Example: 1457573000. | 
 **q** | **optional.String**| Custom query Example: status:Sent,status_code:201. | 
 **order** | **optional.String**| Order result by Example: date_added:desc,list_id:desc. | 
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

# **FaxPricePost**
> string FaxPricePost(ctx, faxMessage)
Calculate Total Price for Fax Messages sent

Calculate Total Price for Fax Messages sent

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **faxMessage** | [**FaxMessageCollection**](FaxMessageCollection.md)| FaxMessageCollection model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **FaxReceiptsByMessageIdGet**
> string FaxReceiptsByMessageIdGet(ctx, messageId)
Get a single fax receipt based on message id.

Get a single fax receipt based on message id.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **messageId** | **string**| ID of the message receipt to retrieve | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **FaxReceiptsGet**
> string FaxReceiptsGet(ctx, optional)
Get List of Fax Receipts

Get List of Fax Receipts

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***FaxReceiptsGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a FaxReceiptsGetOpts struct

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

# **FaxSendPost**
> string FaxSendPost(ctx, faxMessage)
Send a fax using supplied supported file-types.

Send a fax using supplied supported file-types.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **faxMessage** | [**FaxMessageCollection**](FaxMessageCollection.md)| FaxMessageCollection model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

