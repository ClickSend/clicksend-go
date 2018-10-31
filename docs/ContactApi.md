# ClickSend.Client\ContactApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ListsContactsByListIdAndContactIdDelete**](ContactApi.md#ListsContactsByListIdAndContactIdDelete) | **Delete** /lists/{list_id}/contacts/{contact_id} | Delete a contact
[**ListsContactsByListIdAndContactIdGet**](ContactApi.md#ListsContactsByListIdAndContactIdGet) | **Get** /lists/{list_id}/contacts/{contact_id} | Get a specific contact
[**ListsContactsByListIdAndContactIdPut**](ContactApi.md#ListsContactsByListIdAndContactIdPut) | **Put** /lists/{list_id}/contacts/{contact_id} | Update specific contact
[**ListsContactsByListIdGet**](ContactApi.md#ListsContactsByListIdGet) | **Get** /lists/{list_id}/contacts | Get all contacts in a list
[**ListsContactsByListIdPost**](ContactApi.md#ListsContactsByListIdPost) | **Post** /lists/{list_id}/contacts | Create new contact
[**ListsRemoveOptedOutContactsByListIdAndOptOutListIdPut**](ContactApi.md#ListsRemoveOptedOutContactsByListIdAndOptOutListIdPut) | **Put** /lists/{list_id}/remove-opted-out-contacts/{opt_out_list_id} | Remove all opted out contacts
[**ListsTransferContactPut**](ContactApi.md#ListsTransferContactPut) | **Put** /lists/{from_list_id}/contacts/{contact_id}/{to_list_id} | Transfer contact to another list


# **ListsContactsByListIdAndContactIdDelete**
> string ListsContactsByListIdAndContactIdDelete(ctx, listId, contactId)
Delete a contact

Delete a contact

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **listId** | **int32**| List ID | 
  **contactId** | **int32**| Contact ID | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListsContactsByListIdAndContactIdGet**
> string ListsContactsByListIdAndContactIdGet(ctx, listId, contactId)
Get a specific contact

Get a specific contact

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **listId** | **int32**| Your contact list id you want to access. | 
  **contactId** | **int32**| Your contact id you want to access. | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListsContactsByListIdAndContactIdPut**
> string ListsContactsByListIdAndContactIdPut(ctx, listId, contactId, contact)
Update specific contact

Update specific contact

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **listId** | **int32**| Contact list id | 
  **contactId** | **int32**| Contact ID | 
  **contact** | [**Contact**](Contact.md)| Contact model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListsContactsByListIdGet**
> string ListsContactsByListIdGet(ctx, listId, optional)
Get all contacts in a list

Get all contacts in a list

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **listId** | **int32**| Contact list ID | 
 **optional** | ***ListsContactsByListIdGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ListsContactsByListIdGetOpts struct

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

# **ListsContactsByListIdPost**
> string ListsContactsByListIdPost(ctx, contact, listId, optional)
Create new contact

Create new contact

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **contact** | [**Contact**](Contact.md)| Contact model | 
  **listId** | **int32**| List id | 
 **optional** | ***ListsContactsByListIdPostOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ListsContactsByListIdPostOpts struct

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

# **ListsRemoveOptedOutContactsByListIdAndOptOutListIdPut**
> string ListsRemoveOptedOutContactsByListIdAndOptOutListIdPut(ctx, listId, optOutListId)
Remove all opted out contacts

Remove all opted out contacts

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **listId** | **int32**| Your list id | 
  **optOutListId** | **int32**| Your opt out list id | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListsTransferContactPut**
> string ListsTransferContactPut(ctx, fromListId, contactId, toListId)
Transfer contact to another list

Transfer contact to another list

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **fromListId** | **int32**| List ID for list that contains contact. | 
  **contactId** | **int32**| Contact ID | 
  **toListId** | **int32**| List ID for list you want to transfer contact to. | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

