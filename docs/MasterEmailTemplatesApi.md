# ClickSend.Client\MasterEmailTemplatesApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**MasterEmailTemplateCategoriesGet**](MasterEmailTemplatesApi.md#MasterEmailTemplateCategoriesGet) | **Get** /email/master-templates-categories | Get all master email template categories
[**MasterEmailTemplateCategoryGet**](MasterEmailTemplatesApi.md#MasterEmailTemplateCategoryGet) | **Get** /email/master-templates-categories/{category_id} | Get specific master email template category
[**MasterEmailTemplateGet**](MasterEmailTemplatesApi.md#MasterEmailTemplateGet) | **Get** /email/master-templates/{template_id} | Get specific master email template
[**MasterEmailTemplatesGet**](MasterEmailTemplatesApi.md#MasterEmailTemplatesGet) | **Get** /email/master-templates | Get all master email templates
[**MasterEmailTemplatesInCategoryGet**](MasterEmailTemplatesApi.md#MasterEmailTemplatesInCategoryGet) | **Get** /email/master-templates-categories/{category_id}/master-templates | Get all master email templates in a category


# **MasterEmailTemplateCategoriesGet**
> string MasterEmailTemplateCategoriesGet(ctx, optional)
Get all master email template categories

Get all master email template categories

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***MasterEmailTemplateCategoriesGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a MasterEmailTemplateCategoriesGetOpts struct

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

# **MasterEmailTemplateCategoryGet**
> string MasterEmailTemplateCategoryGet(ctx, categoryId)
Get specific master email template category

Get specific master email template category

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **categoryId** | **int32**| Email category id | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **MasterEmailTemplateGet**
> string MasterEmailTemplateGet(ctx, templateId)
Get specific master email template

Get specific master email template

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

# **MasterEmailTemplatesGet**
> string MasterEmailTemplatesGet(ctx, optional)
Get all master email templates

Get all master email templates

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***MasterEmailTemplatesGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a MasterEmailTemplatesGetOpts struct

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

# **MasterEmailTemplatesInCategoryGet**
> string MasterEmailTemplatesInCategoryGet(ctx, categoryId, optional)
Get all master email templates in a category

Get all master email templates in a category

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **categoryId** | **int32**| Email category id | 
 **optional** | ***MasterEmailTemplatesInCategoryGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a MasterEmailTemplatesInCategoryGetOpts struct

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

