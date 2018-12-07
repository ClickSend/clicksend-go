# \AccountApi

All URIs are relative to *https://rest.clicksend.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AccountGet**](AccountApi.md#AccountGet) | **Get** /account | Get account information
[**AccountPost**](AccountApi.md#AccountPost) | **Post** /account | Create a new account
[**AccountUseageBySubaccountGet**](AccountApi.md#AccountUseageBySubaccountGet) | **Get** /account/usage/{year}/{month}/subaccount | Get account useage by subaccount
[**AccountVerifySendPut**](AccountApi.md#AccountVerifySendPut) | **Put** /account-verify/send | Send account activation token
[**AccountVerifyVerifyByActivationTokenPut**](AccountApi.md#AccountVerifyVerifyByActivationTokenPut) | **Put** /account-verify/verify/{activation_token} | Verify new account
[**ForgotPasswordPut**](AccountApi.md#ForgotPasswordPut) | **Put** /forgot-password | Forgot password
[**ForgotPasswordVerifyPut**](AccountApi.md#ForgotPasswordVerifyPut) | **Put** /forgot-password/verify | Verify forgot password
[**ForgotUsernamePut**](AccountApi.md#ForgotUsernamePut) | **Put** /forgot-username | Forgot username


# **AccountGet**
> string AccountGet(ctx, )
Get account information

Get account details

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

# **AccountPost**
> string AccountPost(ctx, account)
Create a new account

Create An Account

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **account** | [**Account**](Account.md)| Account model | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **AccountUseageBySubaccountGet**
> string AccountUseageBySubaccountGet(ctx, year, month)
Get account useage by subaccount

Get account useage by subaccount

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **year** | **int32**| Year to filter by (yyyy) | 
  **month** | **int32**| Month to filter by (mm) | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **AccountVerifySendPut**
> string AccountVerifySendPut(ctx, accountVerify)
Send account activation token

Send account activation token

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **accountVerify** | [**AccountVerify**](AccountVerify.md)| Account details | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **AccountVerifyVerifyByActivationTokenPut**
> string AccountVerifyVerifyByActivationTokenPut(ctx, activationToken)
Verify new account

Verify new account

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **activationToken** | **int32**|  | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ForgotPasswordPut**
> string ForgotPasswordPut(ctx, optional)
Forgot password

Forgot password

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***ForgotPasswordPutOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ForgotPasswordPutOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **forgotPassword** | [**optional.Interface of ForgotPassword**](ForgotPassword.md)|  | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ForgotPasswordVerifyPut**
> string ForgotPasswordVerifyPut(ctx, verifyPassword)
Verify forgot password

Verify forgot password

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **verifyPassword** | [**AccountForgotPasswordVerify**](AccountForgotPasswordVerify.md)| verifyPassword data | 

### Return type

**string**

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ForgotUsernamePut**
> string ForgotUsernamePut(ctx, optional)
Forgot username

Forgot username

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***ForgotUsernamePutOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ForgotUsernamePutOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **forgotUsername** | [**optional.Interface of ForgotUsername**](ForgotUsername.md)|  | 

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

