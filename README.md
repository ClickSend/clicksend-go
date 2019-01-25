# The official Go library for ClickSend v3 API

This is the official [ClickSend](https://clicksend.com) SDK. Documentation can be found [here](https://developers.clicksend.com/docs/rest/v3/?go#introduction).

## Requirements

- [Sign Up](https://www.clicksend.com/signup) for a free ClickSend account.
- Copy your API key from the [API Credentials](https://dashboard.clicksend.com/#/account/subaccount) area.

## Installation
Put the package under your project folder and add the following in import:
```golang
import "./clicksend"
```

## Documentation

Documentation for our SDK and REST API can be found [here](https://developers.clicksend.com/docs/rest/v3/?go#introduction).

## Documentation For Authorization

## BasicAuth
- **Type**: HTTP basic authentication

Example
```golang
auth := context.WithValue(context.Background(), sw.ContextBasicAuth, sw.BasicAuth{
	UserName: "username",
	Password: "password",
})
r, err := client.Service.Operation(auth, args)
```
