# \EmailToSmsApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**SmsEmailSmsGet**](EmailToSmsApi.md#SmsEmailSmsGet) | **Get** /sms/email-sms | Get list of email to sms allowed addresses
[**SmsEmailSmsPost**](EmailToSmsApi.md#SmsEmailSmsPost) | **Post** /sms/email-sms | Create email to sms allowed address
[**SmsEmailSmsStrippedStringDelete**](EmailToSmsApi.md#SmsEmailSmsStrippedStringDelete) | **Delete** /sms/email-sms-stripped-strings/{rule_id} | Delete email to sms stripped string rule
[**SmsEmailSmsStrippedStringGet**](EmailToSmsApi.md#SmsEmailSmsStrippedStringGet) | **Get** /sms/email-sms-stripped-strings/{rule_id} | Get email to sms stripped string rule
[**SmsEmailSmsStrippedStringPost**](EmailToSmsApi.md#SmsEmailSmsStrippedStringPost) | **Post** /sms/email-sms-stripped-strings | Create email to sms stripped string rule
[**SmsEmailSmsStrippedStringPut**](EmailToSmsApi.md#SmsEmailSmsStrippedStringPut) | **Put** /sms/email-sms-stripped-strings/{rule_id} | Update email to sms stripped string rule
[**SmsEmailSmsStrippedStringsGet**](EmailToSmsApi.md#SmsEmailSmsStrippedStringsGet) | **Get** /sms/email-sms-stripped-strings | Get list of email to sms stripped string rules


# **SmsEmailSmsGet**
> string SmsEmailSmsGet(ctx, optional)
Get list of email to sms allowed addresses

Get list of email to sms allowed addresses

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***EmailToSmsApiSmsEmailSmsGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a EmailToSmsApiSmsEmailSmsGetOpts struct

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

# **SmsEmailSmsPost**
> string SmsEmailSmsPost(ctx, emailSmsAddress)
Create email to sms allowed address

Create email to sms allowed address

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **emailSmsAddress** | [**EmailSmsAddress**](EmailSmsAddress.md)| EmailSMSAddress model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SmsEmailSmsStrippedStringDelete**
> string SmsEmailSmsStrippedStringDelete(ctx, ruleId)
Delete email to sms stripped string rule

Delete email to sms stripped string rule

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **ruleId** | **int32**| Your rule id | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SmsEmailSmsStrippedStringGet**
> string SmsEmailSmsStrippedStringGet(ctx, ruleId)
Get email to sms stripped string rule

Get email to sms stripped string rule

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **ruleId** | **int32**| Your rule id | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SmsEmailSmsStrippedStringPost**
> string SmsEmailSmsStrippedStringPost(ctx, strippedString)
Create email to sms stripped string rule

Create email to sms stripped string rules

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **strippedString** | [**StrippedString**](StrippedString.md)| StrippedString model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SmsEmailSmsStrippedStringPut**
> string SmsEmailSmsStrippedStringPut(ctx, strippedString, ruleId)
Update email to sms stripped string rule

Update email to sms stripped string rule

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **strippedString** | [**StrippedString**](StrippedString.md)| StrippedString model | 
  **ruleId** | **int32**| Your rule id | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SmsEmailSmsStrippedStringsGet**
> string SmsEmailSmsStrippedStringsGet(ctx, optional)
Get list of email to sms stripped string rules

Get list of email to sms stripped string rules

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***EmailToSmsApiSmsEmailSmsStrippedStringsGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a EmailToSmsApiSmsEmailSmsStrippedStringsGetOpts struct

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

