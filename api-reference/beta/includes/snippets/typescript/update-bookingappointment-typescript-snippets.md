---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BookingAppointment = {
	end : {
		dateTime : "2018-05-06T12:30:00.0000000+00:00",
		timeZone : "UTC",
		additionalData : {
			"@odata.type" : "#microsoft.graph.dateTimeTimeZone",
		},
	},
	invoiceDate : {
		dateTime : "2018-05-06T12:30:00.0000000+00:00",
		timeZone : "UTC",
		additionalData : {
			"@odata.type" : "#microsoft.graph.dateTimeTimeZone",
		},
	},
	start : {
		dateTime : "2018-05-06T12:00:00.0000000+00:00",
		timeZone : "UTC",
		additionalData : {
			"@odata.type" : "#microsoft.graph.dateTimeTimeZone",
		},
	},
	additionalData : {
		"@odata.type" : "#microsoft.graph.bookingAppointment",
	},
};

const result = async () => {
	await graphServiceClient.bookingBusinessesById("bookingBusiness-id").appointmentsById("bookingAppointment-id").patch(requestBody);
}


```