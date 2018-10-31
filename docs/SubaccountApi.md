# ClickSend.Client\SubaccountApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**SubaccountsBySubaccountIdDelete**](SubaccountApi.md#SubaccountsBySubaccountIdDelete) | **Delete** /subaccounts/{subaccount_id} | Delete a subaccount
[**SubaccountsBySubaccountIdGet**](SubaccountApi.md#SubaccountsBySubaccountIdGet) | **Get** /subaccounts/{subaccount_id} | Get specific subaccount
[**SubaccountsBySubaccountIdPut**](SubaccountApi.md#SubaccountsBySubaccountIdPut) | **Put** /subaccounts/{subaccount_id} | Update subaccount
[**SubaccountsGet**](SubaccountApi.md#SubaccountsGet) | **Get** /subaccounts | Get all subaccounts
[**SubaccountsPost**](SubaccountApi.md#SubaccountsPost) | **Post** /subaccounts | Create new subaccount
[**SubaccountsRegenApiKeyBySubaccountIdPut**](SubaccountApi.md#SubaccountsRegenApiKeyBySubaccountIdPut) | **Put** /subaccounts/{subaccount_id}/regen-api-key | Regenerate an API Key


# **SubaccountsBySubaccountIdDelete**
> string SubaccountsBySubaccountIdDelete(ctx, subaccountId)
Delete a subaccount

Delete a subaccount

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **subaccountId** | **int32**| ID of subaccount to delete | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SubaccountsBySubaccountIdGet**
> string SubaccountsBySubaccountIdGet(ctx, subaccountId)
Get specific subaccount

Get specific subaccount

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **subaccountId** | **int32**| ID of subaccount to get | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SubaccountsBySubaccountIdPut**
> string SubaccountsBySubaccountIdPut(ctx, subaccountId, subaccount)
Update subaccount

Update subaccount

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **subaccountId** | **int32**| ID of subaccount to update | 
  **subaccount** | [**Subaccount**](Subaccount.md)| Subaccount model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SubaccountsGet**
> string SubaccountsGet(ctx, optional)
Get all subaccounts

Get all subaccounts

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SubaccountsGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SubaccountsGetOpts struct

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

# **SubaccountsPost**
> string SubaccountsPost(ctx, subaccount)
Create new subaccount

Create new subaccount

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **subaccount** | [**Subaccount**](Subaccount.md)| Subaccount model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SubaccountsRegenApiKeyBySubaccountIdPut**
> string SubaccountsRegenApiKeyBySubaccountIdPut(ctx, subaccountId)
Regenerate an API Key

Regenerate an API Key

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **subaccountId** | **int32**| ID of subaccount to regenerate API key for | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

