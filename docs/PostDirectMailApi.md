# ClickSend.Client\PostDirectMailApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**PostDirectMailCampaignsGet**](PostDirectMailApi.md#PostDirectMailCampaignsGet) | **Get** /post/direct-mail/campaigns | Get direct mail campaigns
[**PostDirectMailCampaignsPricePost**](PostDirectMailApi.md#PostDirectMailCampaignsPricePost) | **Post** /post/direct-mail/campaigns/price | Calculate direct mail campaign price
[**PostDirectMailCampaignsSendPost**](PostDirectMailApi.md#PostDirectMailCampaignsSendPost) | **Post** /post/direct-mail/campaigns/send | Send direct mail campaign
[**PostDirectMailLocationsSearchByCountryGet**](PostDirectMailApi.md#PostDirectMailLocationsSearchByCountryGet) | **Get** /post/direct-mail/locations/search/{country} | Search for a location


# **PostDirectMailCampaignsGet**
> string PostDirectMailCampaignsGet(ctx, optional)
Get direct mail campaigns

Get direct mail campaigns

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***PostDirectMailCampaignsGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PostDirectMailCampaignsGetOpts struct

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

# **PostDirectMailCampaignsPricePost**
> string PostDirectMailCampaignsPricePost(ctx, postDirectMail)
Calculate direct mail campaign price

Calculate direct mail campaign price

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **postDirectMail** | [**PostDirectMail**](PostDirectMail.md)| PostDirectMail model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **PostDirectMailCampaignsSendPost**
> string PostDirectMailCampaignsSendPost(ctx, postDirectMail)
Send direct mail campaign

Send direct mail campaign

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **postDirectMail** | [**PostDirectMail**](PostDirectMail.md)| PostDirectMail model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **PostDirectMailLocationsSearchByCountryGet**
> string PostDirectMailLocationsSearchByCountryGet(ctx, country, q, optional)
Search for a location

Search for a location

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **country** | **string**| Country Code to search | 
  **q** | **string**| Search term (e.g. post code, city name) | 
 **optional** | ***PostDirectMailLocationsSearchByCountryGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PostDirectMailLocationsSearchByCountryGetOpts struct

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

