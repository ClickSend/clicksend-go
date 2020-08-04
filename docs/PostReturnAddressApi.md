# \PostReturnAddressApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**PostReturnAddressesByReturnAddressIdDelete**](PostReturnAddressApi.md#PostReturnAddressesByReturnAddressIdDelete) | **Delete** /post/return-addresses/{return_address_id} | Delete specific post return address
[**PostReturnAddressesByReturnAddressIdGet**](PostReturnAddressApi.md#PostReturnAddressesByReturnAddressIdGet) | **Get** /post/return-addresses/{return_address_id} | Get specific post return address
[**PostReturnAddressesByReturnAddressIdPut**](PostReturnAddressApi.md#PostReturnAddressesByReturnAddressIdPut) | **Put** /post/return-addresses/{return_address_id} | Update post return address
[**PostReturnAddressesGet**](PostReturnAddressApi.md#PostReturnAddressesGet) | **Get** /post/return-addresses | Get list of post return addresses
[**PostReturnAddressesPost**](PostReturnAddressApi.md#PostReturnAddressesPost) | **Post** /post/return-addresses | Create post return address


# **PostReturnAddressesByReturnAddressIdDelete**
> string PostReturnAddressesByReturnAddressIdDelete(ctx, returnAddressId)
Delete specific post return address

Delete specific post return address

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **returnAddressId** | **int32**| Return address ID | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **PostReturnAddressesByReturnAddressIdGet**
> string PostReturnAddressesByReturnAddressIdGet(ctx, returnAddressId)
Get specific post return address

Get specific post return address

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **returnAddressId** | **int32**| Return address ID | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **PostReturnAddressesByReturnAddressIdPut**
> string PostReturnAddressesByReturnAddressIdPut(ctx, returnAddressId, returnAddress)
Update post return address

Update post return address

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **returnAddressId** | **int32**| Return address ID | 
  **returnAddress** | [**Address**](Address.md)| Address model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **PostReturnAddressesGet**
> string PostReturnAddressesGet(ctx, optional)
Get list of post return addresses

Get list of post return addresses

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***PostReturnAddressApiPostReturnAddressesGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PostReturnAddressApiPostReturnAddressesGetOpts struct

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

# **PostReturnAddressesPost**
> string PostReturnAddressesPost(ctx, returnAddress)
Create post return address

Create post return address

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **returnAddress** | [**Address**](Address.md)| Address model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

