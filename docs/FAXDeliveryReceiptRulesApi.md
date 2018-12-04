# \FAXDeliveryReceiptRulesApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**FaxDeliveryReceiptAutomationDelete**](FAXDeliveryReceiptRulesApi.md#FaxDeliveryReceiptAutomationDelete) | **Delete** /automations/fax/receipts/{receipt_rule_id} | Delete fax delivery receipt automation
[**FaxDeliveryReceiptAutomationGet**](FAXDeliveryReceiptRulesApi.md#FaxDeliveryReceiptAutomationGet) | **Get** /automations/fax/receipts/{receipt_rule_id} | Get specific fax delivery receipt automation
[**FaxDeliveryReceiptAutomationPost**](FAXDeliveryReceiptRulesApi.md#FaxDeliveryReceiptAutomationPost) | **Post** /automations/fax/receipts | Create fax delivery receipt automations
[**FaxDeliveryReceiptAutomationPut**](FAXDeliveryReceiptRulesApi.md#FaxDeliveryReceiptAutomationPut) | **Put** /automations/fax/receipts/{receipt_rule_id} | Update fax delivery receipt automation
[**FaxDeliveryReceiptAutomationsGet**](FAXDeliveryReceiptRulesApi.md#FaxDeliveryReceiptAutomationsGet) | **Get** /automations/fax/receipts | Get all fax delivery receipt automations


# **FaxDeliveryReceiptAutomationDelete**
> string FaxDeliveryReceiptAutomationDelete(ctx, receiptRuleId)
Delete fax delivery receipt automation

Delete fax delivery receipt automation

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

# **FaxDeliveryReceiptAutomationGet**
> string FaxDeliveryReceiptAutomationGet(ctx, receiptRuleId)
Get specific fax delivery receipt automation

Get specific fax delivery receipt automation

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

# **FaxDeliveryReceiptAutomationPost**
> string FaxDeliveryReceiptAutomationPost(ctx, deliveryReceiptRule)
Create fax delivery receipt automations

Create fax delivery receipt automations

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **deliveryReceiptRule** | [**DeliveryReceiptRule**](DeliveryReceiptRule.md)| fax delivery receipt rule model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **FaxDeliveryReceiptAutomationPut**
> string FaxDeliveryReceiptAutomationPut(ctx, receiptRuleId, deliveryReceiptRule)
Update fax delivery receipt automation

Update fax delivery receipt automation

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

# **FaxDeliveryReceiptAutomationsGet**
> string FaxDeliveryReceiptAutomationsGet(ctx, q, optional)
Get all fax delivery receipt automations

Get all fax delivery receipt automations

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **q** | **string**| Your keyword or query. | 
 **optional** | ***FaxDeliveryReceiptAutomationsGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a FaxDeliveryReceiptAutomationsGetOpts struct

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

