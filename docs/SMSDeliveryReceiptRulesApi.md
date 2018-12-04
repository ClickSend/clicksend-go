# \SMSDeliveryReceiptRulesApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**SmsDeliveryReceiptAutomationDelete**](SMSDeliveryReceiptRulesApi.md#SmsDeliveryReceiptAutomationDelete) | **Delete** /automations/sms/receipts/{receipt_rule_id} | Delete sms delivery receipt automation
[**SmsDeliveryReceiptAutomationGet**](SMSDeliveryReceiptRulesApi.md#SmsDeliveryReceiptAutomationGet) | **Get** /automations/sms/receipts/{receipt_rule_id} | Get specific sms delivery receipt automation
[**SmsDeliveryReceiptAutomationPost**](SMSDeliveryReceiptRulesApi.md#SmsDeliveryReceiptAutomationPost) | **Post** /automations/sms/receipts | Create sms delivery receipt automations
[**SmsDeliveryReceiptAutomationPut**](SMSDeliveryReceiptRulesApi.md#SmsDeliveryReceiptAutomationPut) | **Put** /automations/sms/receipts/{receipt_rule_id} | Update sms delivery receipt automation
[**SmsDeliveryReceiptAutomationsGet**](SMSDeliveryReceiptRulesApi.md#SmsDeliveryReceiptAutomationsGet) | **Get** /automations/sms/receipts | Get all sms delivery receipt automations


# **SmsDeliveryReceiptAutomationDelete**
> string SmsDeliveryReceiptAutomationDelete(ctx, receiptRuleId)
Delete sms delivery receipt automation

Delete sms delivery receipt automation

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

# **SmsDeliveryReceiptAutomationGet**
> string SmsDeliveryReceiptAutomationGet(ctx, receiptRuleId)
Get specific sms delivery receipt automation

Get specific sms delivery receipt automation

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

# **SmsDeliveryReceiptAutomationPost**
> string SmsDeliveryReceiptAutomationPost(ctx, deliveryReceiptRule)
Create sms delivery receipt automations

Create sms delivery receipt automations

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **deliveryReceiptRule** | [**DeliveryReceiptRule**](DeliveryReceiptRule.md)| sms delivery receipt rule model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SmsDeliveryReceiptAutomationPut**
> string SmsDeliveryReceiptAutomationPut(ctx, receiptRuleId, deliveryReceiptRule)
Update sms delivery receipt automation

Update sms delivery receipt automation

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

# **SmsDeliveryReceiptAutomationsGet**
> string SmsDeliveryReceiptAutomationsGet(ctx, q, optional)
Get all sms delivery receipt automations

Get all sms delivery receipt automations

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **q** | **string**| Your keyword or query. | 
 **optional** | ***SmsDeliveryReceiptAutomationsGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SmsDeliveryReceiptAutomationsGetOpts struct

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

