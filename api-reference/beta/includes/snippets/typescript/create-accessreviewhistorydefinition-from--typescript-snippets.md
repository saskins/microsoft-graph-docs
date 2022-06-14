---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessReviewHistoryDefinition = {
	displayName : "Last quarter's group reviews April 2021",
	decisions : [
		"approve",
		"deny",
		"dontKnow",
		"notReviewed",
		"notNotified",
	],
	scheduleSettings : {
		reportRange : "P1M",
		recurrence : {
			pattern : {
				type : RecurrencePatternType.Monthly,
				interval : 1,
			},
			range : {
				type : RecurrenceRangeType.NoEnd,
				startDate : "2018-08-03T21:02:30.667Z",
				additionalData : {
					count : 0,
				},
			},
		},
	},
	scopes : [
		{
			additionalData : {
				"@odata.type" : "#microsoft.graph.accessReviewQueryScope",
				"queryType" : "MicrosoftGraph",
				"query" : "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')",
				queryRoot : null,
			},
		},
		{
			additionalData : {
				"@odata.type" : "#microsoft.graph.accessReviewQueryScope",
				"queryType" : "MicrosoftGraph",
				"query" : "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')",
				queryRoot : null,
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.identityGovernance.accessReviews.historyDefinitions.post(requestBody);
}


```