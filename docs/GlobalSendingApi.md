# \GlobalSendingApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ListCountriesGet**](GlobalSendingApi.md#ListCountriesGet) | **Get** /country-list | List of countries
[**UserCountriesAgreePost**](GlobalSendingApi.md#UserCountriesAgreePost) | **Post** /user-countries/agree | Agree to rules and regulation
[**UserCountriesGet**](GlobalSendingApi.md#UserCountriesGet) | **Get** /user-countries | Get Countries for Global Sending
[**UserCountriesPost**](GlobalSendingApi.md#UserCountriesPost) | **Post** /user-countries | Select Countries for Global Sending


# **ListCountriesGet**
> string ListCountriesGet(ctx, )
List of countries

List of countries with IDs that can be used in selecting countries for Global sending.

### Required Parameters
This endpoint does not need any parameter.

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UserCountriesAgreePost**
> string UserCountriesAgreePost(ctx, )
Agree to rules and regulation

To agree on rules and regulations of selected countries and confirm selection.

### Required Parameters
This endpoint does not need any parameter.

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UserCountriesGet**
> string UserCountriesGet(ctx, )
Get Countries for Global Sending

Get the list of selected countries.

### Required Parameters
This endpoint does not need any parameter.

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UserCountriesPost**
> string UserCountriesPost(ctx, countryListIds)
Select Countries for Global Sending

Use this endpoint to select countries that you intend to send sms / mms to. To remove / unselect a country, just remove the country id from the array in the payload.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **countryListIds** | [**CountryListIds**](CountryListIds.md)| Id of countr(ies) you want to select, you can get them from GET /country-list response | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

