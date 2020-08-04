# \DeliveryIssuesApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DeliveryIssuesGet**](DeliveryIssuesApi.md#DeliveryIssuesGet) | **Get** /delivery-issues | Get all delivery issues
[**DeliveryIssuesPost**](DeliveryIssuesApi.md#DeliveryIssuesPost) | **Post** /delivery-issues | Create delivery Issue


# **DeliveryIssuesGet**
> string DeliveryIssuesGet(ctx, optional)
Get all delivery issues

Get all delivery issues

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***DeliveryIssuesApiDeliveryIssuesGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a DeliveryIssuesApiDeliveryIssuesGetOpts struct

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

# **DeliveryIssuesPost**
> string DeliveryIssuesPost(ctx, deliveryIssue)
Create delivery Issue

Create delivery Issue

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **deliveryIssue** | [**DeliveryIssue**](DeliveryIssue.md)| DeliveryIssue model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

