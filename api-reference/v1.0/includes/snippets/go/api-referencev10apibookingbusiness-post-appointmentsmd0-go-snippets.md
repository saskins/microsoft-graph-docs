---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBookingAppointment()
customerTimeZone := "America/Chicago"
requestBody.SetCustomerTimeZone(&customerTimeZone)
smsNotificationsEnabled := true
requestBody.SetSmsNotificationsEnabled(&smsNotificationsEnabled)
endDateTime := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetEndDateTime(endDateTime)
dateTime := "2018-05-01T12:30:00.0000000+00:00"
endDateTime.SetDateTime(&dateTime)
timeZone := "UTC"
endDateTime.SetTimeZone(&timeZone)
endDateTime.SetAdditionalData(map[string]interface{}{
	"@odata.type": "#microsoft.graph.dateTimeTimeZone",
}
isLocationOnline := true
requestBody.SetIsLocationOnline(&isLocationOnline)
optOutOfCustomerEmail := false
requestBody.SetOptOutOfCustomerEmail(&optOutOfCustomerEmail)
postBuffer := "PT10M"
requestBody.SetPostBuffer(&postBuffer)
preBuffer := "PT5M"
requestBody.SetPreBuffer(&preBuffer)
price := float64(10)
requestBody.SetPrice(&price)
priceType := "fixedPrice"
requestBody.SetPriceType(&priceType)
requestBody.SetReminders( []BookingReminder {
	msgraphsdk.NewBookingReminder(),
message := "This service is tomorrow"
	SetMessage(&message)
offset := "P1D"
	SetOffset(&offset)
recipients := "allAttendees"
	SetRecipients(&recipients)
	SetAdditionalData(map[string]interface{}{
		"@odata.type": "#microsoft.graph.bookingReminder",
		"recipients@odata.type": "#microsoft.graph.bookingReminderRecipients",
	}
	msgraphsdk.NewBookingReminder(),
message := "Please be available to enjoy your lunch service."
	SetMessage(&message)
offset := "PT1H"
	SetOffset(&offset)
recipients := "customer"
	SetRecipients(&recipients)
	SetAdditionalData(map[string]interface{}{
		"@odata.type": "#microsoft.graph.bookingReminder",
		"recipients@odata.type": "#microsoft.graph.bookingReminderRecipients",
	}
	msgraphsdk.NewBookingReminder(),
message := "Please check traffic for next cater."
	SetMessage(&message)
offset := "PT2H"
	SetOffset(&offset)
recipients := "staff"
	SetRecipients(&recipients)
	SetAdditionalData(map[string]interface{}{
		"@odata.type": "#microsoft.graph.bookingReminder",
		"recipients@odata.type": "#microsoft.graph.bookingReminderRecipients",
	}
}
serviceId := "57da6774-a087-4d69-b0e6-6fb82c339976"
requestBody.SetServiceId(&serviceId)
serviceLocation := msgraphsdk.NewLocation()
requestBody.SetServiceLocation(serviceLocation)
address := msgraphsdk.NewPhysicalAddress()
serviceLocation.SetAddress(address)
city := "Buffalo"
address.SetCity(&city)
countryOrRegion := "USA"
address.SetCountryOrRegion(&countryOrRegion)
postalCode := "98052"
address.SetPostalCode(&postalCode)
state := "NY"
address.SetState(&state)
street := "123 First Avenue"
address.SetStreet(&street)
address.SetAdditionalData(map[string]interface{}{
	"@odata.type": "#microsoft.graph.physicalAddress",
	"postOfficeBox": nil,
	"type@odata.type": "#microsoft.graph.physicalAddressType",
	"type": nil,
}
serviceLocation.SetCoordinates(nil)
displayName := "Customer location"
serviceLocation.SetDisplayName(&displayName)
serviceLocation.SetLocationEmailAddress(nil)
serviceLocation.SetLocationType(nil)
serviceLocation.SetLocationUri(nil)
serviceLocation.SetUniqueId(nil)
serviceLocation.SetUniqueIdType(nil)
serviceLocation.SetAdditionalData(map[string]interface{}{
	"@odata.type": "#microsoft.graph.location",
	"locationType@odata.type": "#microsoft.graph.locationType",
	"uniqueIdType@odata.type": "#microsoft.graph.locationUniqueIdType",
}
serviceName := "Catered bento"
requestBody.SetServiceName(&serviceName)
serviceNotes := "Customer requires punctual service."
requestBody.SetServiceNotes(&serviceNotes)
startDateTime := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetStartDateTime(startDateTime)
dateTime := "2018-05-01T12:00:00.0000000+00:00"
startDateTime.SetDateTime(&dateTime)
timeZone := "UTC"
startDateTime.SetTimeZone(&timeZone)
startDateTime.SetAdditionalData(map[string]interface{}{
	"@odata.type": "#microsoft.graph.dateTimeTimeZone",
}
maximumAttendeesCount := int32(5)
requestBody.SetMaximumAttendeesCount(&maximumAttendeesCount)
filledAttendeesCount := int32(1)
requestBody.SetFilledAttendeesCount(&filledAttendeesCount)
requestBody.SetCustomers( []BookingCustomerInformationBase {
	msgraphsdk.NewBookingCustomerInformationBase(),
	SetAdditionalData(map[string]interface{}{
		"@odata.type": "#microsoft.graph.bookingCustomerInformation",
		"customerId": "7ed53fa5-9ef2-4f2f-975b-27447440bc09",
		"name": "Jordan Miller",
		"emailAddress": "jordanm@contoso.com",
		"phone": "213-555-0199",
		"notes": nil,
		"timeZone": "America/Chicago",
		"customQuestionAnswers":  []Object {
		}
	}
}
requestBody.SetAdditionalData(map[string]interface{}{
	"@odata.type": "#microsoft.graph.bookingAppointment",
	"priceType@odata.type": "#microsoft.graph.bookingPriceType",
	"reminders@odata.type": "#Collection(microsoft.graph.bookingReminder)",
	"customers@odata.type": "#Collection(microsoft.graph.bookingCustomerInformation)",
}
bookingBusinessId := "bookingBusiness-id"
result, err := graphClient.Solutions().BookingBusinessesById(&bookingBusinessId).Appointments().Post(requestBody)


```