# clicksend\TransactionalEmailApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**EmailHistoryExportGet**](TransactionalEmailApi.md#EmailHistoryExportGet) | **Get** /email/history/export | Export all Transactional Email history
[**EmailHistoryGet**](TransactionalEmailApi.md#EmailHistoryGet) | **Get** /email/history | Get all transactional email history
[**EmailPricePost**](TransactionalEmailApi.md#EmailPricePost) | **Post** /email/price | Get transactional email price
[**EmailSendPost**](TransactionalEmailApi.md#EmailSendPost) | **Post** /email/send | Send transactional email


# **EmailHistoryExportGet**
> *os.File EmailHistoryExportGet(ctx, filename, optional)
Export all Transactional Email history

Export all Transactional Email history

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **filename** | **string**| Filename to download history as | 
 **optional** | ***EmailHistoryExportGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a EmailHistoryExportGetOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **dateFrom** | **optional.Int32**| Start date | 
 **dateTo** | **optional.Int32**| End date | 

### Return type

[***os.File**](*os.File.md)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, application/csv

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **EmailHistoryGet**
> string EmailHistoryGet(ctx, optional)
Get all transactional email history

Get all transactional email history

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***EmailHistoryGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a EmailHistoryGetOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
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

# **EmailPricePost**
> string EmailPricePost(ctx, email)
Get transactional email price

Get transactional email price

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **email** | [**Email**](Email.md)| Email model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **EmailSendPost**
> string EmailSendPost(ctx, email)
Send transactional email

Send transactional email

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **email** | [**Email**](Email.md)| Email model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

