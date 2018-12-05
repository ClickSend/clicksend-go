# The official Go library for ClickSend v3 API

 This is an official SDK for [ClickSend](https://clicksend.com)  Below you will find a current list of the available methods for clicksend.  *NOTE: You will need to create a free account to use the API. You can register [here](https://dashboard.clicksend.com/#/signup/step1/)..* 


## Installation
Put the package under your project folder and add the following in import:
```golang
import "./clicksend"
```

## Documentation for API Endpoints and Models

Documentation can be found here: [ClickSend API Docs](https://developers.clicksend.com/docs/)

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
