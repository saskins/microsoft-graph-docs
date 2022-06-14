---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BookingStaffMember = {
	workingHours : [
		{
			day : DayOfWeek.Monday,
			timeSlots : [
			],
			additionalData : {
				"@odata.type" : "#microsoft.graph.bookingWorkHours",
				"day@odata.type" : "#microsoft.graph.dayOfWeek",
				"timeSlots@odata.type" : "#Collection(microsoft.graph.bookingWorkTimeSlot)",
			},
		},
		{
			day : DayOfWeek.Tuesday,
			timeSlots : [
				{
					end : "17:00:00.0000000",
					start : "08:00:00.0000000",
					additionalData : {
						"@odata.type" : "#microsoft.graph.bookingWorkTimeSlot",
					},
				},
			],
			additionalData : {
				"@odata.type" : "#microsoft.graph.bookingWorkHours",
				"day@odata.type" : "#microsoft.graph.dayOfWeek",
				"timeSlots@odata.type" : "#Collection(microsoft.graph.bookingWorkTimeSlot)",
			},
		},
		{
			day : DayOfWeek.Wednesday,
			timeSlots : [
				{
					end : "17:00:00.0000000",
					start : "08:00:00.0000000",
					additionalData : {
						"@odata.type" : "#microsoft.graph.bookingWorkTimeSlot",
					},
				},
			],
			additionalData : {
				"@odata.type" : "#microsoft.graph.bookingWorkHours",
				"day@odata.type" : "#microsoft.graph.dayOfWeek",
				"timeSlots@odata.type" : "#Collection(microsoft.graph.bookingWorkTimeSlot)",
			},
		},
		{
			day : DayOfWeek.Thursday,
			timeSlots : [
				{
					end : "17:00:00.0000000",
					start : "08:00:00.0000000",
					additionalData : {
						"@odata.type" : "#microsoft.graph.bookingWorkTimeSlot",
					},
				},
			],
			additionalData : {
				"@odata.type" : "#microsoft.graph.bookingWorkHours",
				"day@odata.type" : "#microsoft.graph.dayOfWeek",
				"timeSlots@odata.type" : "#Collection(microsoft.graph.bookingWorkTimeSlot)",
			},
		},
		{
			day : DayOfWeek.Friday,
			timeSlots : [
				{
					end : "17:00:00.0000000",
					start : "08:00:00.0000000",
					additionalData : {
						"@odata.type" : "#microsoft.graph.bookingWorkTimeSlot",
					},
				},
			],
			additionalData : {
				"@odata.type" : "#microsoft.graph.bookingWorkHours",
				"day@odata.type" : "#microsoft.graph.dayOfWeek",
				"timeSlots@odata.type" : "#Collection(microsoft.graph.bookingWorkTimeSlot)",
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.bookingBusinessesById("bookingBusiness-id").staffMembersById("bookingStaffMember-id").patch(requestBody);
}


```