---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"Prefer": "outlook.timezone=\"Pacific Standard Time\"",
	}
};
const requestBody : FindMeetingTimesPostRequestBody = {
	attendees : [
		{
			additionalData : {
				"type" : "required",
				emailAddress : {
					name : "Alex Wilbur",
					address : "alexw@contoso.onmicrosoft.com",
				},
			},
		},
	],
	locationConstraint : {
		isRequired : false,
		suggestLocation : false,
		locations : [
			{
				additionalData : {
					resolveAvailability : false,
					"displayName" : "Conf room Hood",
				},
			},
		],
	},
	timeConstraint : {
		activityDomain : ActivityDomain.Work,
		timeSlots : [
			{
				start : {
					dateTime : "2019-04-16T09:00:00",
					timeZone : "Pacific Standard Time",
				},
				end : {
					dateTime : "2019-04-18T17:00:00",
					timeZone : "Pacific Standard Time",
				},
			},
		],
	},
	isOrganizerOptional : "false",
	meetingDuration : "PT1H",
	returnSuggestionReasons : "true",
	minimumAttendeePercentage : .100,
};

const result = async () => {
	await graphServiceClient.me.findMeetingTimes.post(requestBody, configuration);
}


```