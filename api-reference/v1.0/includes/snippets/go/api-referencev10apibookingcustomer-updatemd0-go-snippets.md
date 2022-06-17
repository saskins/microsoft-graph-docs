---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBookingCustomerBase()
requestBody.SetAdditionalData(map[string]interface{}{
	"@odata.type": "#microsoft.graph.bookingCustomer",
	"displayName": "Adele",
	"emailAddress": "adele@relecloud.com",
}
bookingBusinessId := "bookingBusiness-id"
bookingCustomerBaseId := "bookingCustomerBase-id"
graphClient.Solutions().BookingBusinessesById(&bookingBusinessId).CustomersById(&bookingCustomerBaseId).Patch(requestBody)


```