# ClickSend.Client\UserEmailTemplatesApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**EmailTemplateDelete**](UserEmailTemplatesApi.md#EmailTemplateDelete) | **Delete** /email/templates/{template_id} | Delete user email template
[**EmailTemplateGet**](UserEmailTemplatesApi.md#EmailTemplateGet) | **Get** /email/templates/{template_id} | Get specific user email template
[**EmailTemplatePost**](UserEmailTemplatesApi.md#EmailTemplatePost) | **Post** /email/templates | Create email template
[**EmailTemplatePut**](UserEmailTemplatesApi.md#EmailTemplatePut) | **Post** /email/templates/{template_id} | Update email template
[**EmailTemplatesGet**](UserEmailTemplatesApi.md#EmailTemplatesGet) | **Get** /email/templates | Get all user email templates


# **EmailTemplateDelete**
> string EmailTemplateDelete(ctx, templateId)
Delete user email template

Delete user email template

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **templateId** | **int32**| Email template id | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **EmailTemplateGet**
> string EmailTemplateGet(ctx, templateId)
Get specific user email template

Get specific user email templates

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **templateId** | **int32**| Email template id | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **EmailTemplatePost**
> string EmailTemplatePost(ctx, emailTemplate)
Create email template

Create email template

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **emailTemplate** | [**EmailTemplateNew**](EmailTemplateNew.md)| Email template model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **EmailTemplatePut**
> string EmailTemplatePut(ctx, templateId, emailTemplate)
Update email template

Update email template

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **templateId** | **int32**| Email template id | 
  **emailTemplate** | [**EmailTemplateUpdate**](EmailTemplateUpdate.md)| Email template model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **EmailTemplatesGet**
> string EmailTemplatesGet(ctx, optional)
Get all user email templates

Get all user email templates

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***EmailTemplatesGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a EmailTemplatesGetOpts struct

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

