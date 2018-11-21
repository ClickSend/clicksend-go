# clicksend\UploadApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**UploadsPost**](UploadApi.md#UploadsPost) | **Post** /uploads | Upload File


# **UploadsPost**
> string UploadsPost(ctx, convert, optional)
Upload File

Upload File

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **convert** | **string**|  | 
 **optional** | ***UploadsPostOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a UploadsPostOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **uploadFile** | [**optional.Interface of UploadFile**](UploadFile.md)|  | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

