# The official Go library for ClickSend v3 API

This is the official [ClickSend](https://clicksend.com) Go SDK. Documentation can be found [here](https://developers.clicksend.com/docs/rest/v3/?go#introduction).

---

## Requirements

- [Go](https://go.dev/dl/) 1.18 or later
- A free ClickSend account — [sign up here](https://www.clicksend.com/signup)
- Your ClickSend **username** (email) and **API key** from the [API Credentials](https://dashboard.clicksend.com/#/account/subaccount) page

---

## Installation

### Step 1 — Verify Go is installed

```bash
go version
```

You should see output like `go version go1.21.0 darwin/arm64`. If not, [install Go](https://go.dev/dl/) first.

---

### Step 2 — Create a new project directory

```bash
mkdir clicksend-sms && cd clicksend-sms
```

---

### Step 3 — Initialise a Go module

```bash
go mod init clicksend-sms
```

---

### Step 4 — Install the ClickSend Go SDK

```bash
go get github.com/ClickSend/clicksend-go
```

Run `go mod tidy` to pull in all transitive dependencies:

```bash
go mod tidy
```

---

### Step 5 — Create `main.go`

Create a file named `main.go` in your project directory and paste the following code:

```go
package main

import (
	"context"
	"fmt"
	"log"

	clicksend "github.com/ClickSend/clicksend-go"
)

const (
	username = "USERNAME"  // Your ClickSend username (email)
	apiKey   = "API_KEY"   // Your ClickSend API key
	fromNum  = "FROM"      // Approved sender ID or number e.g. "+61400000000"
	toNum    = "TO"        // Recipient number in E.164 format e.g. "+61400000001"
)

func main() {
	cfg := clicksend.NewConfiguration()
	client := clicksend.NewAPIClient(cfg)

	auth := context.WithValue(context.Background(), clicksend.ContextBasicAuth, clicksend.BasicAuth{
		UserName: username,
		Password: apiKey,
	})

	msg := clicksend.SmsMessage{
		From:   fromNum,
		To:     toNum,
		Body:   "Hello from the ClickSend Go SDK!",
		Source: "go-sdk",
	}

	result, _, err := client.SMSApi.SmsSendPost(auth, clicksend.SmsMessageCollection{
		Messages: []clicksend.SmsMessage{msg},
	})
	if err != nil {
		log.Fatalf("error sending SMS: %v", err)
	}

	fmt.Println("Response:", result)
}
```

---

### Step 6 — Set your credentials

Replace the four constants at the top of `main.go` with your actual values:

| Constant | Where to find it |
|---|---|
| `USERNAME` | Your ClickSend account email |
| `API_KEY` | [Dashboard → API Credentials](https://dashboard.clicksend.com/#/account/subaccount) |
| `FROM` | An approved sender ID or your ClickSend number (leave blank to use a shared number) |
| `TO` | The destination phone number in [E.164 format](https://en.wikipedia.org/wiki/E.164) e.g. `+61400000001` |

---

### Step 7 — Run the code

```bash
go run main.go
```

A successful response looks like this:

```json
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Messages queued for delivery.",
  "data": {
    "total_price": 0.891,
    "total_count": 1,
    "queued_count": 1,
    "messages": [
      {
        "status": "SUCCESS",
        "message_id": "xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
        "to": "+61400000001",
        "from": "ClickSend",
        "body": "Hello from the ClickSend Go SDK!"
      }
    ]
  }
}
```

---

## Project Structure

```
clicksend-sms/
├── main.go    # Example — send a single SMS
├── go.mod     # Module definition and SDK dependency
└── go.sum     # Dependency checksums
```

---

## Authentication

The SDK uses **HTTP Basic Auth**. Your username and API key are passed via `context` on every request:

```go
auth := context.WithValue(context.Background(), clicksend.ContextBasicAuth, clicksend.BasicAuth{
    UserName: "your_username",
    Password: "your_api_key",
})
```

Pass this `auth` context as the first argument to every API call.

---

## Sending to Multiple Recipients

Pass more than one `SmsMessage` in the `Messages` slice to send in a single API call (up to 1 000 messages per request):

```go
result, _, err := client.SMSApi.SmsSendPost(auth, clicksend.SmsMessageCollection{
    Messages: []clicksend.SmsMessage{
        {From: fromNum, To: "+61400000001", Body: "Hello Alice!", Source: "go-sdk"},
        {From: fromNum, To: "+61400000002", Body: "Hello Bob!",   Source: "go-sdk"},
    },
})
```

---

## Further Reading

- [ClickSend REST API docs](https://developers.clicksend.com/docs/rest/v3/)
- [clicksend-go SDK on GitHub](https://github.com/ClickSend/clicksend-go)
- [ClickSend Dashboard](https://dashboard.clicksend.com)
