---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBookingCustomerBase()
requestBody.SetAdditionalData(map[string]interface{}{
	"@odata.type": "#microsoft.graph.bookingCustomer",
	"displayName": "Joni Sherman",
	"emailAddress": "jonis@relecloud.com",
	"addresses":  []Object {
	}
	"phones":  []Object {
	}
}
bookingBusinessId := "bookingBusiness-id"
result, err := graphClient.Solutions().BookingBusinessesById(&bookingBusinessId).Customers().Post(requestBody)


```