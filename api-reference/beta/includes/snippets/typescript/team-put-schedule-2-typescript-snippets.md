---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SchedulePostRequestBody = {
	additionalData : {
		enabled : true,
		"timeZone" : "America/Chicago",
		"provisionStatus" : "Completed",
		provisionStatusCode : null,
		openShiftsEnabled : true,
		swapShiftsRequestsEnabled : true,
		offerShiftRequestsEnabled : true,
		timeOffRequestsEnabled : true,
		timeClockEnabled : true,
		timeClockSettings : {
			approvedLocation : {
				altitude : 1024.13,
				latitude : 26.13246,
				longitude : 24.34616,
			},
		},
	},
};

async () => {
	await graphServiceClient.teamsById("team-id").schedule.put(requestBody);
}


```