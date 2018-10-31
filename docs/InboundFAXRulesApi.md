# \InboundFAXRulesApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**FaxInboundAutomationDelete**](InboundFAXRulesApi.md#FaxInboundAutomationDelete) | **Delete** /automations/fax/inbound/{inbound_rule_id} | Delete inbound fax automation
[**FaxInboundAutomationGet**](InboundFAXRulesApi.md#FaxInboundAutomationGet) | **Get** /automations/fax/inbound/{inbound_rule_id} | Get specific inbound fax automation
[**FaxInboundAutomationPost**](InboundFAXRulesApi.md#FaxInboundAutomationPost) | **Post** /automations/fax/inbound | Create new inbound fax automation
[**FaxInboundAutomationPut**](InboundFAXRulesApi.md#FaxInboundAutomationPut) | **Put** /automations/fax/inbound/{inbound_rule_id} | Update inbound fax automation
[**FaxInboundAutomationsGet**](InboundFAXRulesApi.md#FaxInboundAutomationsGet) | **Get** /automations/fax/inbound | Get all inbound fax automations


# **FaxInboundAutomationDelete**
> string FaxInboundAutomationDelete(ctx, inboundRuleId)
Delete inbound fax automation

Delete inbound fax automation

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

# **FaxInboundAutomationGet**
> string FaxInboundAutomationGet(ctx, inboundRuleId)
Get specific inbound fax automation

Get specific inbound fax automation

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

# **FaxInboundAutomationPost**
> string FaxInboundAutomationPost(ctx, inboundFaxRule)
Create new inbound fax automation

Create new inbound fax automation

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **inboundFaxRule** | [**InboundFaxRule**](InboundFaxRule.md)| Inbound fax rule model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **FaxInboundAutomationPut**
> string FaxInboundAutomationPut(ctx, inboundRuleId, inboundFaxRule)
Update inbound fax automation

Update inbound fax automation

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **inboundRuleId** | **int32**| Inbound rule id | 
  **inboundFaxRule** | [**InboundFaxRule**](InboundFaxRule.md)| Inbound fax rule model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **FaxInboundAutomationsGet**
> string FaxInboundAutomationsGet(ctx, optional)
Get all inbound fax automations

Get all inbound fax automations

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***FaxInboundAutomationsGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a FaxInboundAutomationsGetOpts struct

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

