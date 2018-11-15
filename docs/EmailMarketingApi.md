# clicksend\EmailMarketingApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AllowedEmailAddressGet**](EmailMarketingApi.md#AllowedEmailAddressGet) | **Get** /email/addresses | Get all email addresses
[**AllowedEmailAddressPost**](EmailMarketingApi.md#AllowedEmailAddressPost) | **Post** /email/addresses | Create allowed Email Address
[**CancelEmailCampaignPut**](EmailMarketingApi.md#CancelEmailCampaignPut) | **Put** /email-campaigns/{email_campaign_id}/cancel | Cancel email campaign
[**EmailCampaignGet**](EmailMarketingApi.md#EmailCampaignGet) | **Get** /email-campaigns/{email_campaign_id} | Get specific email campaign
[**EmailCampaignHistoryExportGet**](EmailMarketingApi.md#EmailCampaignHistoryExportGet) | **Get** /email-campaigns/{email_campaign_id}/history/export | Export specific email campaign history
[**EmailCampaignHistoryGet**](EmailMarketingApi.md#EmailCampaignHistoryGet) | **Get** /email-campaigns/{email_campaign_id}/history | Get specific email campaign history
[**EmailCampaignPost**](EmailMarketingApi.md#EmailCampaignPost) | **Post** /email-campaigns/send | Send email campaign
[**EmailCampaignPricePost**](EmailMarketingApi.md#EmailCampaignPricePost) | **Post** /email-campaigns/price | Calculate email campaign price
[**EmailCampaignPut**](EmailMarketingApi.md#EmailCampaignPut) | **Put** /email-campaigns/{email_campaign_id} | Edit email campaign
[**EmailCampaignsGet**](EmailMarketingApi.md#EmailCampaignsGet) | **Get** /email-campaigns | Get all email campaigns
[**SendVerificationTokenGet**](EmailMarketingApi.md#SendVerificationTokenGet) | **Get** /email/address-verify/{email_address_id}/send | Send verification token
[**SpecificAllowedEmailAddressDelete**](EmailMarketingApi.md#SpecificAllowedEmailAddressDelete) | **Delete** /email/addresses/{email_address_id} | Delete specific email address
[**SpecificAllowedEmailAddressGet**](EmailMarketingApi.md#SpecificAllowedEmailAddressGet) | **Get** /email/addresses/{email_address_id} | Get specific email address
[**VerifyAllowedEmailAddressGet**](EmailMarketingApi.md#VerifyAllowedEmailAddressGet) | **Get** /email/address-verify/{email_address_id}/verify/{activation_token} | Verify email address using verification token


# **AllowedEmailAddressGet**
> string AllowedEmailAddressGet(ctx, optional)
Get all email addresses

Get all email addresses

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***AllowedEmailAddressGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a AllowedEmailAddressGetOpts struct

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

# **AllowedEmailAddressPost**
> string AllowedEmailAddressPost(ctx, emailAddress)
Create allowed Email Address

Create allowed Email Address

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **emailAddress** | **string**| Email to be allowed. | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CancelEmailCampaignPut**
> string CancelEmailCampaignPut(ctx, emailCampaignId)
Cancel email campaign

Cancel email campaign

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **emailCampaignId** | **int32**| Allowed email campaign id | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **EmailCampaignGet**
> string EmailCampaignGet(ctx, emailCampaignId)
Get specific email campaign

Get specific email campaign

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **emailCampaignId** | **int32**| Allowed email campaign id | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **EmailCampaignHistoryExportGet**
> *os.File EmailCampaignHistoryExportGet(ctx, emailCampaignId, optional)
Export specific email campaign history

Export specific email campaign history

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **emailCampaignId** | **int32**| Allowed email campaign id | 
 **optional** | ***EmailCampaignHistoryExportGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a EmailCampaignHistoryExportGetOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **dateFrom** | **optional.Int32**| Start date | 
 **dateTo** | **optional.Int32**| End date | 

### Return type

[***os.File**](*os.File.md)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **EmailCampaignHistoryGet**
> string EmailCampaignHistoryGet(ctx, emailCampaignId, optional)
Get specific email campaign history

Get specific email campaign history

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **emailCampaignId** | **int32**| Allowed email campaign id | 
 **optional** | ***EmailCampaignHistoryGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a EmailCampaignHistoryGetOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **dateFrom** | **optional.Int32**| Start date | 
 **dateTo** | **optional.Int32**| End date | 
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

# **EmailCampaignPost**
> string EmailCampaignPost(ctx, emailCampaign)
Send email campaign

Send email campaign

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **emailCampaign** | [**EmailCampaign**](EmailCampaign.md)| Email model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **EmailCampaignPricePost**
> string EmailCampaignPricePost(ctx, emailCampaign)
Calculate email campaign price

Calculate email campaign price

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **emailCampaign** | [**EmailCampaign**](EmailCampaign.md)| Email model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **EmailCampaignPut**
> string EmailCampaignPut(ctx, emailCampaignId)
Edit email campaign

Edit email campaign

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **emailCampaignId** | **int32**| Allowed email campaign id | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **EmailCampaignsGet**
> string EmailCampaignsGet(ctx, optional)
Get all email campaigns

Get all email campaigns

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***EmailCampaignsGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a EmailCampaignsGetOpts struct

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

# **SendVerificationTokenGet**
> string SendVerificationTokenGet(ctx, emailAddressId)
Send verification token

Send verification token

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **emailAddressId** | **int32**| Allowed email address id | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SpecificAllowedEmailAddressDelete**
> string SpecificAllowedEmailAddressDelete(ctx, emailAddressId)
Delete specific email address

Delete specific email address

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **emailAddressId** | **int32**| Allowed email address id | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SpecificAllowedEmailAddressGet**
> string SpecificAllowedEmailAddressGet(ctx, emailAddressId)
Get specific email address

Get specific email address

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **emailAddressId** | **int32**| Allowed email address id | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **VerifyAllowedEmailAddressGet**
> string VerifyAllowedEmailAddressGet(ctx, emailAddressId, activationToken)
Verify email address using verification token

Verify email address using verification token

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **emailAddressId** | **int32**| Allowed email address id | 
  **activationToken** | **string**| Your activation token. | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

