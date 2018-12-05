# \VoiceDeliveryReceiptRulesApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**VoiceDeliveryReceiptAutomationDelete**](VoiceDeliveryReceiptRulesApi.md#VoiceDeliveryReceiptAutomationDelete) | **Delete** /automations/voice/receipts/{receipt_rule_id} | Delete voice delivery receipt automation
[**VoiceDeliveryReceiptAutomationGet**](VoiceDeliveryReceiptRulesApi.md#VoiceDeliveryReceiptAutomationGet) | **Get** /automations/voice/receipts/{receipt_rule_id} | Get specific voice delivery receipt automation
[**VoiceDeliveryReceiptAutomationPost**](VoiceDeliveryReceiptRulesApi.md#VoiceDeliveryReceiptAutomationPost) | **Post** /automations/voice/receipts | Create voice delivery receipt automations
[**VoiceDeliveryReceiptAutomationPut**](VoiceDeliveryReceiptRulesApi.md#VoiceDeliveryReceiptAutomationPut) | **Put** /automations/voice/receipts/{receipt_rule_id} | Update voice delivery receipt automation
[**VoiceDeliveryReceiptAutomationsGet**](VoiceDeliveryReceiptRulesApi.md#VoiceDeliveryReceiptAutomationsGet) | **Get** /automations/voice/receipts | Get all voice delivery receipt automations


# **VoiceDeliveryReceiptAutomationDelete**
> string VoiceDeliveryReceiptAutomationDelete(ctx, receiptRuleId)
Delete voice delivery receipt automation

Delete voice delivery receipt automation

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

# **VoiceDeliveryReceiptAutomationGet**
> string VoiceDeliveryReceiptAutomationGet(ctx, receiptRuleId)
Get specific voice delivery receipt automation

Get specific voice delivery receipt automation

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

# **VoiceDeliveryReceiptAutomationPost**
> string VoiceDeliveryReceiptAutomationPost(ctx, deliveryReceiptRule)
Create voice delivery receipt automations

Create voice delivery receipt automations

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **deliveryReceiptRule** | [**DeliveryReceiptRule**](DeliveryReceiptRule.md)| voice delivery receipt rule model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **VoiceDeliveryReceiptAutomationPut**
> string VoiceDeliveryReceiptAutomationPut(ctx, receiptRuleId, deliveryReceiptRule)
Update voice delivery receipt automation

Update voice delivery receipt automation

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

# **VoiceDeliveryReceiptAutomationsGet**
> string VoiceDeliveryReceiptAutomationsGet(ctx, optional)
Get all voice delivery receipt automations

Get all voice delivery receipt automations

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***VoiceDeliveryReceiptAutomationsGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a VoiceDeliveryReceiptAutomationsGetOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **optional.String**| Your keyword or query. | 
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

