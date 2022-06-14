---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BookingService = {
	defaultDuration : "PT1H30M",
	defaultLocation : {
		address : {
			city : "Buffalo",
			countryOrRegion : "USA",
			postalCode : "98052",
			postOfficeBox : null,
			state : "NY",
			street : "4567 First Street",
			type : null,
			additionalData : {
				"@odata.type" : "#microsoft.graph.physicalAddress",
				"type@odata.type" : "#microsoft.graph.physicalAddressType",
			},
		},
		coordinates : null,
		displayName : "Contoso Lunch Delivery",
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
	defaultPrice : 10.0,
	defaultPriceType : BookingPriceType.FixedPrice,
	defaultReminders : [
		{
			message : "Please be reminded that this service is tomorrow.",
			offset : "P1D",
			recipients : BookingReminderRecipients.AllAttendees,
			additionalData : {
				"@odata.type" : "#microsoft.graph.bookingReminder",
				"recipients@odata.type" : "#microsoft.graph.bookingReminderRecipients",
			},
		},
	],
	description : "Individual bento box lunch delivery",
	displayName : "Bento",
	isLocationOnline : true,
	smsNotificationsEnabled : true,
	isHiddenFromCustomers : false,
	notes : "Home-cooked special",
	postBuffer : "PT10M",
	preBuffer : "PT5M",
	schedulingPolicy : {
		allowStaffSelection : true,
		maximumAdvance : "P10D",
		minimumLeadTime : "PT10H",
		sendConfirmationsToOwner : true,
		timeSlotInterval : "PT1H",
		additionalData : {
			"@odata.type" : "#microsoft.graph.bookingSchedulingPolicy",
		},
	},
	staffMemberIds : [
		"d90d1e8c-5cfe-48cf-a2d5-966267375b6a",
		"2f5f8794-0b29-45b5-b56a-2eb5ff7aa880",
	],
	additionalData : {
		"@odata.type" : "#microsoft.graph.bookingService",
		"defaultPriceType@odata.type" : "#microsoft.graph.bookingPriceType",
		"defaultReminders@odata.type" : "#Collection(microsoft.graph.bookingReminder)",
		"staffMemberIds@odata.type" : "#Collection(String)",
	},
};

const result = async () => {
	await graphServiceClient.bookingBusinessesById("bookingBusiness-id").services.post(requestBody);
}


```