# \AccountRechargeApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**RechargeCreditCardGet**](AccountRechargeApi.md#RechargeCreditCardGet) | **Get** /recharge/credit-card | Get Credit Card info
[**RechargeCreditCardPut**](AccountRechargeApi.md#RechargeCreditCardPut) | **Put** /recharge/credit-card | Update credit card info
[**RechargePackagesGet**](AccountRechargeApi.md#RechargePackagesGet) | **Get** /recharge/packages | Get list of all packages
[**RechargePurchaseByPackageIdPut**](AccountRechargeApi.md#RechargePurchaseByPackageIdPut) | **Put** /recharge/purchase/{package_id} | Purchase a package
[**RechargeTransactionsByTransactionIdGet**](AccountRechargeApi.md#RechargeTransactionsByTransactionIdGet) | **Get** /recharge/transactions/{transaction_id} | Get specific Transaction
[**RechargeTransactionsGet**](AccountRechargeApi.md#RechargeTransactionsGet) | **Get** /recharge/transactions | Purchase a package


# **RechargeCreditCardGet**
> string RechargeCreditCardGet(ctx, )
Get Credit Card info

Get Credit Card info

### Required Parameters
This endpoint does not need any parameter.

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RechargeCreditCardPut**
> string RechargeCreditCardPut(ctx, creditCard)
Update credit card info

Update credit card info

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **creditCard** | [**CreditCard**](CreditCard.md)| CreditCard model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RechargePackagesGet**
> string RechargePackagesGet(ctx, optional)
Get list of all packages

Get list of all packages

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***RechargePackagesGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RechargePackagesGetOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **country** | **optional.String**| Country code | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RechargePurchaseByPackageIdPut**
> string RechargePurchaseByPackageIdPut(ctx, packageId)
Purchase a package

Purchase a package

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **packageId** | **int32**| ID of package to purchase | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RechargeTransactionsByTransactionIdGet**
> string RechargeTransactionsByTransactionIdGet(ctx, transactionId)
Get specific Transaction

Get specific Transaction

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **transactionId** | **string**| ID of transaction to retrieve | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RechargeTransactionsGet**
> string RechargeTransactionsGet(ctx, optional)
Purchase a package

Get all transactions

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***RechargeTransactionsGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RechargeTransactionsGetOpts struct

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

