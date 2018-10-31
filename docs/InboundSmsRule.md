# InboundSmsRule

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DedicatedNumber** | **string** | Dedicated Number. Can be &#39;*&#39; to apply to all numbers. | [default to null]
**RuleName** | **string** | Rule Name. | [default to null]
**MessageSearchType** | **float32** | Message Search Type: 0&#x3D;Any message, 1&#x3D;starts with, 2&#x3D;contains, 3&#x3D;does not contain. | [default to null]
**MessageSearchTerm** | **string** | Message search term. | [default to null]
**Action** | **string** | Action to be taken (AUTO_REPLY, EMAIL_USER, EMAIL_FIXED, URL, SMS, POLL, GROUP_SMS, MOVE_CONTACT, CREATE_CONTACT, CREATE_CONTACT_PLUS_EMAIL, CREATE_CONTACT_PLUS_NAME_EMAIL CREATE_CONTACT_PLUS_NAME, SMPP, NONE). | [default to null]
**ActionAddress** | **string** | Action address. | [default to null]
**Enabled** | **float32** | Enabled: Disabled&#x3D;0 or Enabled&#x3D;1. | [default to null]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


