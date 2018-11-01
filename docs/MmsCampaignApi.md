# clicksend\MmsCampaignApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**MmsCampaignByMmsCampaignIdGet**](MmsCampaignApi.md#MmsCampaignByMmsCampaignIdGet) | **Get** /mms-campaign/{mms_campaign_id} | Get specific mms campaign
[**MmsCampaignsByMmsCampaignIdPut**](MmsCampaignApi.md#MmsCampaignsByMmsCampaignIdPut) | **Put** /mms-campaigns/{mms_campaign_id} | Update mms campaign
[**MmsCampaignsCancelByMmsCampaignIdPut**](MmsCampaignApi.md#MmsCampaignsCancelByMmsCampaignIdPut) | **Put** /mms-campaigns/{mms_campaign_id}/cancel | Cancel mms campaign
[**MmsCampaignsGet**](MmsCampaignApi.md#MmsCampaignsGet) | **Get** /mms-campaigns | Get list of mms campaigns
[**MmsCampaignsPricePost**](MmsCampaignApi.md#MmsCampaignsPricePost) | **Post** /mms-campaigns/price | Calculate price for mms campaign
[**MmsCampaignsSendPost**](MmsCampaignApi.md#MmsCampaignsSendPost) | **Post** /mms-campaigns/send | Create mms campaign


# **MmsCampaignByMmsCampaignIdGet**
> string MmsCampaignByMmsCampaignIdGet(ctx, mmsCampaignId)
Get specific mms campaign

Get specific mms campaign

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **mmsCampaignId** | **int32**| ID of MMS campaign to retrieve | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **MmsCampaignsByMmsCampaignIdPut**
> string MmsCampaignsByMmsCampaignIdPut(ctx, mmsCampaignId, campaign)
Update mms campaign

Update mms campaign

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **mmsCampaignId** | **int32**| ID of MMS campaign to update | 
  **campaign** | [**MmsCampaign**](MmsCampaign.md)| MmsCampaign model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **MmsCampaignsCancelByMmsCampaignIdPut**
> string MmsCampaignsCancelByMmsCampaignIdPut(ctx, mmsCampaignId)
Cancel mms campaign

Cancel sms campaign

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **mmsCampaignId** | **int32**| ID of MMS Campaign to cancel | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **MmsCampaignsGet**
> string MmsCampaignsGet(ctx, optional)
Get list of mms campaigns

Get list of mms campaigns

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***MmsCampaignsGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a MmsCampaignsGetOpts struct

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

# **MmsCampaignsPricePost**
> string MmsCampaignsPricePost(ctx, campaign)
Calculate price for mms campaign

Calculate price for sms campaign

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **campaign** | [**MmsCampaign**](MmsCampaign.md)| MmsCampaign model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **MmsCampaignsSendPost**
> string MmsCampaignsSendPost(ctx, campaign)
Create mms campaign

Create mms campaign

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **campaign** | [**MmsCampaign**](MmsCampaign.md)| MmsCampaign model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

