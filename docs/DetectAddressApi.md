# clicksend\DetectAddressApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DetectAddressPost**](DetectAddressApi.md#DetectAddressPost) | **Post** /post/letters/detect-address | Detects address in uploaded file.


# **DetectAddressPost**
> string DetectAddressPost(ctx, content)
Detects address in uploaded file.

Detects address in uploaded file.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **content** | **string**| Base64-encoded file contents | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

