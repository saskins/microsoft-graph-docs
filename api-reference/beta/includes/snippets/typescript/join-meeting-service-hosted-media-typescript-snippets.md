---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Call = {
	callbackUri : "https://bot.contoso.com/callback",
	requestedModalities : [
		"audio",
	],
	mediaConfig : {
		additionalData : {
			"@odata.type" : "#microsoft.graph.serviceHostedMediaConfig",
			preFetchMedia : [
				{
					uri : "https://cdn.contoso.com/beep.wav",
					resourceId : "f8971b04-b53e-418c-9222-c82ce681a582",
				},
				{
					uri : "https://cdn.contoso.com/cool.wav",
					resourceId : "86dc814b-c172-4428-9112-60f8ecae1edb",
				},
			],
		},
	},
	chatInfo : {
		threadId : "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2",
		messageId : "0",
		additionalData : {
			"@odata.type" : "#microsoft.graph.chatInfo",
		},
	},
	meetingInfo : {
		allowConversationWithoutHost : true,
		additionalData : {
			"@odata.type" : "#microsoft.graph.organizerMeetingInfo",
			organizer : {
				"@odata.type" : "#microsoft.graph.identitySet",
				user : {
					"@odata.type" : "#microsoft.graph.identity",
					id : "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
					tenantId : "9f386a15-f9cc-445b-8106-ac85e314a07b",
					displayName : "Bob",
				},
			},
		},
	},
	tenantId : "86dc81db-c112-4228-9222-63f3esaa1edb",
	additionalData : {
		"@odata.type" : "#microsoft.graph.call",
	},
};

const result = async () => {
	await graphServiceClient.communications.calls.post(requestBody);
}


```