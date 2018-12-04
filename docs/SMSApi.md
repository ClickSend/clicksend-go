# \SMSApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**SmsCancelAllPut**](SMSApi.md#SmsCancelAllPut) | **Put** /sms/cancel-all | Update all scheduled message as cancelled
[**SmsCancelByMessageIdPut**](SMSApi.md#SmsCancelByMessageIdPut) | **Put** /sms/{message_id}/cancel | Update scheduled message as cancelled
[**SmsHistoryExportGet**](SMSApi.md#SmsHistoryExportGet) | **Get** /sms/history/export | Export all sms history
[**SmsHistoryGet**](SMSApi.md#SmsHistoryGet) | **Get** /sms/history | Get all sms history
[**SmsInboundGet**](SMSApi.md#SmsInboundGet) | **Get** /sms/inbound | Get all inbound sms
[**SmsInboundPost**](SMSApi.md#SmsInboundPost) | **Post** /sms/inbound | Create inbound sms
[**SmsInboundReadPut**](SMSApi.md#SmsInboundReadPut) | **Put** /sms/inbound-read | Mark inbound SMS as read
[**SmsPricePost**](SMSApi.md#SmsPricePost) | **Post** /sms/price | Calculate sms price
[**SmsReceiptsByMessageIdGet**](SMSApi.md#SmsReceiptsByMessageIdGet) | **Get** /sms/receipts/{message_id} | Get a Specific Delivery Receipt
[**SmsReceiptsGet**](SMSApi.md#SmsReceiptsGet) | **Get** /sms/receipts | Get all delivery receipts
[**SmsReceiptsPost**](SMSApi.md#SmsReceiptsPost) | **Post** /sms/receipts | Add a delivery receipt
[**SmsReceiptsReadPut**](SMSApi.md#SmsReceiptsReadPut) | **Put** /sms/receipts-read | Mark delivery receipts as read
[**SmsSendPost**](SMSApi.md#SmsSendPost) | **Post** /sms/send | Send sms message(s)
[**SmsTemplatesByTemplateIdDelete**](SMSApi.md#SmsTemplatesByTemplateIdDelete) | **Delete** /sms/templates/{template_id} | Delete sms template
[**SmsTemplatesByTemplateIdPut**](SMSApi.md#SmsTemplatesByTemplateIdPut) | **Put** /sms/templates/{template_id} | Update sms template
[**SmsTemplatesGet**](SMSApi.md#SmsTemplatesGet) | **Get** /sms/templates | Get lists of all sms templates
[**SmsTemplatesPost**](SMSApi.md#SmsTemplatesPost) | **Post** /sms/templates | Create sms template


# **SmsCancelAllPut**
> string SmsCancelAllPut(ctx, )
Update all scheduled message as cancelled

Update all scheduled message as cancelled

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

# **SmsCancelByMessageIdPut**
> string SmsCancelByMessageIdPut(ctx, messageId)
Update scheduled message as cancelled

Update scheduled message as cancelled

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **messageId** | **string**| The message ID you want to cancel | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SmsHistoryExportGet**
> string SmsHistoryExportGet(ctx, filename)
Export all sms history

Export all sms history

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **filename** | **string**| Filename to download history as | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SmsHistoryGet**
> string SmsHistoryGet(ctx, optional)
Get all sms history

Get all sms history

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SmsHistoryGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SmsHistoryGetOpts struct

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

# **SmsInboundGet**
> string SmsInboundGet(ctx, q, optional)
Get all inbound sms

Get all inbound sms

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **q** | **string**| Your keyword or query. | 
 **optional** | ***SmsInboundGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SmsInboundGetOpts struct

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

# **SmsInboundPost**
> string SmsInboundPost(ctx, url)
Create inbound sms

Create inbound sms

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **url** | [**Url**](Url.md)| Url model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SmsInboundReadPut**
> string SmsInboundReadPut(ctx, optional)
Mark inbound SMS as read

Mark all inbound SMS as read optionally before a certain date

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SmsInboundReadPutOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SmsInboundReadPutOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dateBefore** | **optional.String**| An optional timestamp - mark all as read before this timestamp. If not given, all messages will be marked as read. | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SmsPricePost**
> string SmsPricePost(ctx, smsMessages)
Calculate sms price

Calculate sms price

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **smsMessages** | [**SmsMessageCollection**](SmsMessageCollection.md)| SmsMessageCollection model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SmsReceiptsByMessageIdGet**
> string SmsReceiptsByMessageIdGet(ctx, messageId)
Get a Specific Delivery Receipt

Get a Specific Delivery Receipt

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **messageId** | **string**| Message ID | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SmsReceiptsGet**
> string SmsReceiptsGet(ctx, q, optional)
Get all delivery receipts

Get all delivery receipts

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **q** | **string**| Your keyword or query. | 
 **optional** | ***SmsReceiptsGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SmsReceiptsGetOpts struct

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

# **SmsReceiptsPost**
> string SmsReceiptsPost(ctx, url)
Add a delivery receipt

Add a delivery receipt

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **url** | [**Url**](Url.md)| Url model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SmsReceiptsReadPut**
> string SmsReceiptsReadPut(ctx, optional)
Mark delivery receipts as read

Mark delivery receipts as read

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SmsReceiptsReadPutOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SmsReceiptsReadPutOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dateBefore** | **optional.String**| Mark all as read before this timestamp | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SmsSendPost**
> string SmsSendPost(ctx, smsMessages)
Send sms message(s)

 # Send one or more SMS messages  You can post up to 1000 messages with each API call. You can send to a mix of contacts and contact lists, as long as the total number of recipients is up to 1000.  The response contains status and details for each recipient.  *Refer to [Application Status Codes](https://dashboard.clicksend.com/#/signup/step1/) for the possible response message status strings.* 

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **smsMessages** | [**SmsMessageCollection**](SmsMessageCollection.md)| SmsMessageCollection model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SmsTemplatesByTemplateIdDelete**
> string SmsTemplatesByTemplateIdDelete(ctx, templateId)
Delete sms template

Delete sms template

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **templateId** | **int32**| Template id | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SmsTemplatesByTemplateIdPut**
> string SmsTemplatesByTemplateIdPut(ctx, templateId, smsTemplate)
Update sms template

Update sms template

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **templateId** | **int32**| Template id | 
  **smsTemplate** | [**SmsTemplate**](SmsTemplate.md)| Template item | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SmsTemplatesGet**
> string SmsTemplatesGet(ctx, optional)
Get lists of all sms templates

Get lists of all sms templates

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SmsTemplatesGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SmsTemplatesGetOpts struct

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

# **SmsTemplatesPost**
> string SmsTemplatesPost(ctx, smsTemplate)
Create sms template

Create sms template

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **smsTemplate** | [**SmsTemplate**](SmsTemplate.md)| SmsTemplate model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

