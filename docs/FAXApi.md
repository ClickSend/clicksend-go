# \FAXApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**FaxReceiptsGet**](FAXApi.md#FaxReceiptsGet) | **Get** /fax/receipts | Get all delivery receipts
[**FaxReceiptsPost**](FAXApi.md#FaxReceiptsPost) | **Post** /fax/receipts | Add a delivery receipt
[**FaxReceiptsReadPut**](FAXApi.md#FaxReceiptsReadPut) | **Put** /fax/receipts-read | Mark delivery receipts as read


# **FaxReceiptsGet**
> string FaxReceiptsGet(ctx, optional)
Get all delivery receipts

Get all delivery receipts

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

# **FaxReceiptsPost**
> string FaxReceiptsPost(ctx, url)
Add a delivery receipt

Add a delivery receipt

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **url** | [**Url**](Url.md)| Url model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **FaxReceiptsReadPut**
> string FaxReceiptsReadPut(ctx, optional)
Mark delivery receipts as read

Mark delivery receipts as read

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***FaxReceiptsReadPutOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a FaxReceiptsReadPutOpts struct

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

