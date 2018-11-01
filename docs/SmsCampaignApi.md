# clicksend\SmsCampaignApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**SmsCampaignBySmsCampaignIdGet**](SmsCampaignApi.md#SmsCampaignBySmsCampaignIdGet) | **Get** /sms-campaign/{sms_campaign_id} | Get specific sms campaign
[**SmsCampaignsBySmsCampaignIdPut**](SmsCampaignApi.md#SmsCampaignsBySmsCampaignIdPut) | **Put** /sms-campaigns/{sms_campaign_id} | Update sms campaign
[**SmsCampaignsCancelBySmsCampaignIdPut**](SmsCampaignApi.md#SmsCampaignsCancelBySmsCampaignIdPut) | **Put** /sms-campaigns/{sms_campaign_id}/cancel | Cancel sms campaign
[**SmsCampaignsGet**](SmsCampaignApi.md#SmsCampaignsGet) | **Get** /sms-campaigns | Get list of sms campaigns
[**SmsCampaignsPricePost**](SmsCampaignApi.md#SmsCampaignsPricePost) | **Post** /sms-campaigns/price | Calculate price for sms campaign
[**SmsCampaignsSendPost**](SmsCampaignApi.md#SmsCampaignsSendPost) | **Post** /sms-campaigns/send | Create sms campaign


# **SmsCampaignBySmsCampaignIdGet**
> string SmsCampaignBySmsCampaignIdGet(ctx, smsCampaignId)
Get specific sms campaign

Get specific sms campaign

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **smsCampaignId** | **int32**| ID of SMS campaign to retrieve | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SmsCampaignsBySmsCampaignIdPut**
> string SmsCampaignsBySmsCampaignIdPut(ctx, smsCampaignId, campaign)
Update sms campaign

Update sms campaign

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **smsCampaignId** | **int32**| ID of SMS campaign to update | 
  **campaign** | [**SmsCampaign**](SmsCampaign.md)| SmsCampaign model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SmsCampaignsCancelBySmsCampaignIdPut**
> string SmsCampaignsCancelBySmsCampaignIdPut(ctx, smsCampaignId)
Cancel sms campaign

Cancel sms campaign

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **smsCampaignId** | **int32**| ID of SMS Campaign to cancel | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SmsCampaignsGet**
> string SmsCampaignsGet(ctx, optional)
Get list of sms campaigns

Get list of sms campaigns

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SmsCampaignsGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SmsCampaignsGetOpts struct

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

# **SmsCampaignsPricePost**
> string SmsCampaignsPricePost(ctx, campaign)
Calculate price for sms campaign

Calculate price for sms campaign

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **campaign** | [**SmsCampaign**](SmsCampaign.md)| SmsCampaign model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SmsCampaignsSendPost**
> string SmsCampaignsSendPost(ctx, campaign)
Create sms campaign

Create sms campaign

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **campaign** | [**SmsCampaign**](SmsCampaign.md)| SmsCampaign model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

