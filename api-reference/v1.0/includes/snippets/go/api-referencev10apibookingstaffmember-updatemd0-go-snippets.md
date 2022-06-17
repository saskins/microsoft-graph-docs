---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBookingStaffMemberBase()
requestBody.SetAdditionalData(map[string]interface{}{
	"@odata.type": "#microsoft.graph.bookingStaffMember",
	"workingHours":  []Object {
	}
}
bookingBusinessId := "bookingBusiness-id"
bookingStaffMemberBaseId := "bookingStaffMemberBase-id"
graphClient.Solutions().BookingBusinessesById(&bookingBusinessId).StaffMembersById(&bookingStaffMemberBaseId).Patch(requestBody)


```