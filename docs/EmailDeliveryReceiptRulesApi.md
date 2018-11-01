# clicksend\EmailDeliveryReceiptRulesApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**EmailDeliveryReceiptAutomationDelete**](EmailDeliveryReceiptRulesApi.md#EmailDeliveryReceiptAutomationDelete) | **Delete** /automations/email/receipts/{receipt_rule_id} | Delete email delivery receipt automation
[**EmailDeliveryReceiptAutomationGet**](EmailDeliveryReceiptRulesApi.md#EmailDeliveryReceiptAutomationGet) | **Get** /automations/email/receipts/{receipt_rule_id} | Get specific email delivery receipt automation
[**EmailDeliveryReceiptAutomationPost**](EmailDeliveryReceiptRulesApi.md#EmailDeliveryReceiptAutomationPost) | **Post** /automations/email/receipts | Create email delivery receipt automations
[**EmailDeliveryReceiptAutomationPut**](EmailDeliveryReceiptRulesApi.md#EmailDeliveryReceiptAutomationPut) | **Put** /automations/email/receipts/{receipt_rule_id} | Update email delivery receipt automation
[**EmailDeliveryReceiptAutomationsGet**](EmailDeliveryReceiptRulesApi.md#EmailDeliveryReceiptAutomationsGet) | **Get** /automations/email/receipts | Get all email delivery receipt automations


# **EmailDeliveryReceiptAutomationDelete**
> string EmailDeliveryReceiptAutomationDelete(ctx, receiptRuleId)
Delete email delivery receipt automation

Delete email delivery receipt automation

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **receiptRuleId** | **int32**| Receipt rule id | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **EmailDeliveryReceiptAutomationGet**
> string EmailDeliveryReceiptAutomationGet(ctx, receiptRuleId)
Get specific email delivery receipt automation

Get specific email delivery receipt automation

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **receiptRuleId** | **int32**| Receipt rule id | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **EmailDeliveryReceiptAutomationPost**
> string EmailDeliveryReceiptAutomationPost(ctx, deliveryReceiptRule)
Create email delivery receipt automations

Create email delivery receipt automations

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **deliveryReceiptRule** | [**DeliveryReceiptRule**](DeliveryReceiptRule.md)| Email delivery receipt rule model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **EmailDeliveryReceiptAutomationPut**
> string EmailDeliveryReceiptAutomationPut(ctx, receiptRuleId, deliveryReceiptRule)
Update email delivery receipt automation

Update email delivery receipt automation

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **receiptRuleId** | **int32**| Receipt rule id | 
  **deliveryReceiptRule** | [**DeliveryReceiptRule**](DeliveryReceiptRule.md)| Delivery receipt rule model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **EmailDeliveryReceiptAutomationsGet**
> string EmailDeliveryReceiptAutomationsGet(ctx, optional)
Get all email delivery receipt automations

Get all email delivery receipt automations

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***EmailDeliveryReceiptAutomationsGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a EmailDeliveryReceiptAutomationsGetOpts struct

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

