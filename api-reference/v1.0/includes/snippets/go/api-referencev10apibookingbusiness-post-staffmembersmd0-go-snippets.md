---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBookingStaffMemberBase()
requestBody.SetAdditionalData(map[string]interface{}{
	"@odata.type": "#microsoft.graph.bookingStaffMember",
	"displayName": "Dana Swope",
	"emailAddress": "danas@contoso.com",
	"role@odata.type": "#microsoft.graph.bookingStaffRole",
	"role": "externalGuest",
	"timeZone": "America/Chicago",
	"useBusinessHours": true,
	"workingHours@odata.type": "#Collection(microsoft.graph.bookingWorkHours)",
	"workingHours":  []Object {
	}
}
bookingBusinessId := "bookingBusiness-id"
result, err := graphClient.Solutions().BookingBusinessesById(&bookingBusinessId).StaffMembers().Post(requestBody)


```