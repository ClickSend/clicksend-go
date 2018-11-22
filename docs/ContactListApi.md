# clicksend\ContactListApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ListsByListIdDelete**](ContactListApi.md#ListsByListIdDelete) | **Delete** /lists/{list_id} | ListsByListIdDelete
[**ListsByListIdGet**](ContactListApi.md#ListsByListIdGet) | **Get** /lists/{list_id} | Get specific contact list
[**ListsByListIdPut**](ContactListApi.md#ListsByListIdPut) | **Put** /lists/{list_id} | Update specific contact list
[**ListsGet**](ContactListApi.md#ListsGet) | **Get** /lists | Get all contact lists
[**ListsImportByListIdPost**](ContactListApi.md#ListsImportByListIdPost) | **Post** /lists/{list_id}/import | Import contacts to list
[**ListsPost**](ContactListApi.md#ListsPost) | **Post** /lists | Create new contact list
[**ListsRemoveDuplicatesByListIdPut**](ContactListApi.md#ListsRemoveDuplicatesByListIdPut) | **Put** /lists/{list_id}/remove-duplicates | Remove duplicate contacts


# **ListsByListIdDelete**
> string ListsByListIdDelete(ctx, listId)
ListsByListIdDelete

Delete a specific contact list

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **listId** | **int32**| List ID | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListsByListIdGet**
> string ListsByListIdGet(ctx, listId)
Get specific contact list

Get specific contact list

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **listId** | **int32**| List ID | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListsByListIdPut**
> string ListsByListIdPut(ctx, listId, list)
Update specific contact list

Update specific contact list

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **listId** | **int32**| Your list id | 
  **list** | [**List**](List.md)| List model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListsGet**
> string ListsGet(ctx, optional)
Get all contact lists

Get all contact lists

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***ListsGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ListsGetOpts struct

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

# **ListsImportByListIdPost**
> string ListsImportByListIdPost(ctx, listId, file)
Import contacts to list

Import contacts to list

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **listId** | **int32**| Your contact list id you want to access. | 
  **file** | [**ContactListImport**](ContactListImport.md)| ContactListImport model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListsPost**
> string ListsPost(ctx, list)
Create new contact list

Create new contact list

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **list** | [**List**](List.md)| List model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListsRemoveDuplicatesByListIdPut**
> string ListsRemoveDuplicatesByListIdPut(ctx, listId, fields)
Remove duplicate contacts

Remove duplicate contacts

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **listId** | **int32**| Your list id | 
  **fields** | [**Fields**](Fields.md)| Fields model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

