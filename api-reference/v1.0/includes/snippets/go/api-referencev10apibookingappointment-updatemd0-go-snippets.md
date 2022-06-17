---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBookingAppointment()
endDateTime := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetEndDateTime(endDateTime)
dateTime := "2018-05-06T12:30:00.0000000+00:00"
endDateTime.SetDateTime(&dateTime)
timeZone := "UTC"
endDateTime.SetTimeZone(&timeZone)
endDateTime.SetAdditionalData(map[string]interface{}{
	"@odata.type": "#microsoft.graph.dateTimeTimeZone",
}
startDateTime := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetStartDateTime(startDateTime)
dateTime := "2018-05-06T12:00:00.0000000+00:00"
startDateTime.SetDateTime(&dateTime)
timeZone := "UTC"
startDateTime.SetTimeZone(&timeZone)
startDateTime.SetAdditionalData(map[string]interface{}{
	"@odata.type": "#microsoft.graph.dateTimeTimeZone",
}
requestBody.SetAdditionalData(map[string]interface{}{
	"@odata.type": "#microsoft.graph.bookingAppointment",
}
bookingBusinessId := "bookingBusiness-id"
bookingAppointmentId := "bookingAppointment-id"
graphClient.Solutions().BookingBusinessesById(&bookingBusinessId).AppointmentsById(&bookingAppointmentId).Patch(requestBody)


```