# ClickSend.Client\ResellerAccountApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ResellerAccountsByClientUserIdGet**](ResellerAccountApi.md#ResellerAccountsByClientUserIdGet) | **Get** /reseller/accounts/{client_user_id} | Get Reseller clients Account
[**ResellerAccountsByClientUserIdPut**](ResellerAccountApi.md#ResellerAccountsByClientUserIdPut) | **Put** /reseller/accounts/{client_user_id} | Update Reseller clients Account
[**ResellerAccountsGet**](ResellerAccountApi.md#ResellerAccountsGet) | **Get** /reseller/accounts | Get list of reseller accounts
[**ResellerAccountsPost**](ResellerAccountApi.md#ResellerAccountsPost) | **Post** /reseller/accounts | Create reseller account


# **ResellerAccountsByClientUserIdGet**
> string ResellerAccountsByClientUserIdGet(ctx, clientUserId)
Get Reseller clients Account

Get Reseller clients Account

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **clientUserId** | **int32**| User ID of client | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ResellerAccountsByClientUserIdPut**
> string ResellerAccountsByClientUserIdPut(ctx, clientUserId, resellerAccount)
Update Reseller clients Account

Update Reseller clients Account

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **clientUserId** | **int32**| User ID of client | 
  **resellerAccount** | [**ResellerAccount**](ResellerAccount.md)| ResellerAccount model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ResellerAccountsGet**
> string ResellerAccountsGet(ctx, optional)
Get list of reseller accounts

Get list of reseller accounts

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***ResellerAccountsGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ResellerAccountsGetOpts struct

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

# **ResellerAccountsPost**
> string ResellerAccountsPost(ctx, resellerAccount)
Create reseller account

Create reseller account

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **resellerAccount** | [**ResellerAccount**](ResellerAccount.md)| ResellerAccount model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

