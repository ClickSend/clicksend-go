# \InboundSMSRulesApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**SmsInboundAutomationDelete**](InboundSMSRulesApi.md#SmsInboundAutomationDelete) | **Delete** /automations/sms/inbound/{inbound_rule_id} | Delete inbound sms automation
[**SmsInboundAutomationGet**](InboundSMSRulesApi.md#SmsInboundAutomationGet) | **Get** /automations/sms/inbound/{inbound_rule_id} | Get specific inbound sms automation
[**SmsInboundAutomationPost**](InboundSMSRulesApi.md#SmsInboundAutomationPost) | **Post** /automations/sms/inbound | Create new inbound sms automation
[**SmsInboundAutomationPut**](InboundSMSRulesApi.md#SmsInboundAutomationPut) | **Put** /automations/sms/inbound/{inbound_rule_id} | Update inbound sms automation
[**SmsInboundAutomationsGet**](InboundSMSRulesApi.md#SmsInboundAutomationsGet) | **Get** /automations/sms/inbound | Get all inbound sms automations


# **SmsInboundAutomationDelete**
> string SmsInboundAutomationDelete(ctx, inboundRuleId)
Delete inbound sms automation

Delete inbound sms automation

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **inboundRuleId** | **int32**| Inbound rule id | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SmsInboundAutomationGet**
> string SmsInboundAutomationGet(ctx, inboundRuleId)
Get specific inbound sms automation

Get specific inbound sms automation

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **inboundRuleId** | **int32**| Inbound rule id | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SmsInboundAutomationPost**
> string SmsInboundAutomationPost(ctx, inboundSmsRule)
Create new inbound sms automation

Create new inbound sms automation

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **inboundSmsRule** | [**InboundSmsRule**](InboundSmsRule.md)| Inbound sms rule model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SmsInboundAutomationPut**
> string SmsInboundAutomationPut(ctx, inboundRuleId, inboundSmsRule)
Update inbound sms automation

Update inbound sms automation

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **inboundRuleId** | **int32**| Inbound rule id | 
  **inboundSmsRule** | [**InboundSmsRule**](InboundSmsRule.md)| Inbound sms rule model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SmsInboundAutomationsGet**
> string SmsInboundAutomationsGet(ctx, optional)
Get all inbound sms automations

Get all inbound sms automations

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***InboundSMSRulesApiSmsInboundAutomationsGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a InboundSMSRulesApiSmsInboundAutomationsGetOpts struct

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

