---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BookingAppointment = {
	customerEmailAddress : "jordanm@contoso.com",
	customerLocation : {
		address : {
			city : "Buffalo",
			countryOrRegion : "USA",
			postalCode : "98052",
			postOfficeBox : null,
			state : "NY",
			street : "123 First Avenue",
			type : null,
			additionalData : {
				"@odata.type" : "#microsoft.graph.physicalAddress",
				"type@odata.type" : "#microsoft.graph.physicalAddressType",
			},
		},
		coordinates : null,
		displayName : "Customer",
		locationEmailAddress : null,
		locationType : null,
		locationUri : null,
		uniqueId : null,
		uniqueIdType : null,
		additionalData : {
			"@odata.type" : "#microsoft.graph.location",
			"locationType@odata.type" : "#microsoft.graph.locationType",
			"uniqueIdType@odata.type" : "#microsoft.graph.locationUniqueIdType",
		},
	},
	customerName : "Jordan Miller",
	customerNotes : "Please be on time.",
	customerPhone : "213-555-0199",
	customerTimeZone : "America/Chicago",
	smsNotificationsEnabled : true,
	end : {
		dateTime : "2018-05-01T12:30:00.0000000+00:00",
		timeZone : "UTC",
		additionalData : {
			"@odata.type" : "#microsoft.graph.dateTimeTimeZone",
		},
	},
	invoiceAmount : 10.0,
	invoiceDate : {
		dateTime : "2018-05-01T12:30:00.0000000+00:00",
		timeZone : "UTC",
		additionalData : {
			"@odata.type" : "#microsoft.graph.dateTimeTimeZone",
		},
	},
	invoiceId : "1001",
	invoiceStatus : BookingInvoiceStatus.Open,
	invoiceUrl : "theInvoiceUrl",
	isLocationOnline : true,
	optOutOfCustomerEmail : false,
	postBuffer : "PT10M",
	preBuffer : "PT5M",
	price : 10.0,
	priceType : BookingPriceType.FixedPrice,
	reminders : [
		{
			message : "This service is tomorrow",
			offset : "P1D",
			recipients : BookingReminderRecipients.AllAttendees,
			additionalData : {
				"@odata.type" : "#microsoft.graph.bookingReminder",
				"recipients@odata.type" : "#microsoft.graph.bookingReminderRecipients",
			},
		},
		{
			message : "Please be available to enjoy your lunch service.",
			offset : "PT1H",
			recipients : BookingReminderRecipients.Customer,
			additionalData : {
				"@odata.type" : "#microsoft.graph.bookingReminder",
				"recipients@odata.type" : "#microsoft.graph.bookingReminderRecipients",
			},
		},
		{
			message : "Please check traffic for next cater.",
			offset : "PT2H",
			recipients : BookingReminderRecipients.Staff,
			additionalData : {
				"@odata.type" : "#microsoft.graph.bookingReminder",
				"recipients@odata.type" : "#microsoft.graph.bookingReminderRecipients",
			},
		},
	],
	serviceId : "57da6774-a087-4d69-b0e6-6fb82c339976",
	serviceLocation : {
		address : {
			city : "Buffalo",
			countryOrRegion : "USA",
			postalCode : "98052",
			postOfficeBox : null,
			state : "NY",
			street : "123 First Avenue",
			type : null,
			additionalData : {
				"@odata.type" : "#microsoft.graph.physicalAddress",
				"type@odata.type" : "#microsoft.graph.physicalAddressType",
			},
		},
		coordinates : null,
		displayName : "Customer location",
		locationEmailAddress : null,
		locationType : null,
		locationUri : null,
		uniqueId : null,
		uniqueIdType : null,
		additionalData : {
			"@odata.type" : "#microsoft.graph.location",
			"locationType@odata.type" : "#microsoft.graph.locationType",
			"uniqueIdType@odata.type" : "#microsoft.graph.locationUniqueIdType",
		},
	},
	serviceName : "Catered bento",
	serviceNotes : "Customer requires punctual service.",
	start : {
		dateTime : "2018-05-01T12:00:00.0000000+00:00",
		timeZone : "UTC",
		additionalData : {
			"@odata.type" : "#microsoft.graph.dateTimeTimeZone",
		},
	},
	maximumAttendeesCount : 5,
	filledAttendeesCount : 1,
	customers : [
		{
			additionalData : {
				"@odata.type" : "#microsoft.graph.bookingCustomerInformation",
				"customerId" : "7ed53fa5-9ef2-4f2f-975b-27447440bc09",
				"name" : "Jordan Miller",
				"emailAddress" : "jordanm@contoso.com",
				"phone" : "213-555-0199",
				notes : null,
				location : {
					"@odata.type" : "#microsoft.graph.location",
					displayName : "Customer",
					locationEmailAddress : null,
					locationUri : "",
					locationType : null,
					uniqueId : null,
					uniqueIdType : null,
					address : {
						"@odata.type" : "#microsoft.graph.physicalAddress",
						type : "home",
						postOfficeBox : "",
						street : "",
						city : "",
						state : "",
						countryOrRegion : "",
						postalCode : "",
					},
					coordinates : {
						altitude : null,
						latitude : null,
						longitude : null,
						accuracy : null,
						altitudeAccuracy : null,
					},
				},
				"timeZone" : "America/Chicago",
				customQuestionAnswers : [
					{
						questionId : "3bc6fde0-4ad3-445d-ab17-0fc15dba0774",
						question : "What is your age",
						answerInputType : "text",
						answerOptions : [
						],
						isRequired : true,
						answer : "25",
						selectedOptions : [
						],
					},
				],
			},
		},
	],
	additionalData : {
		"@odata.type" : "#microsoft.graph.bookingAppointment",
		"invoiceStatus@odata.type" : "#microsoft.graph.bookingInvoiceStatus",
		"priceType@odata.type" : "#microsoft.graph.bookingPriceType",
		"reminders@odata.type" : "#Collection(microsoft.graph.bookingReminder)",
	},
};

const result = async () => {
	await graphServiceClient.bookingBusinessesById("bookingBusiness-id").appointments.post(requestBody);
}


```