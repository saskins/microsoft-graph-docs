---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AnswerPostRequestBody = {
	callbackUri : "callbackUri-value",
	mediaConfig : {
		additionalData : {
			"@odata.type" : "#microsoft.graph.appHostedMediaConfig",
			"blob" : "<Media Session Configuration Blob>",
		},
	},
	acceptedModalities : [
		"audio",
	],
	callOptions : {
		isContentSharingNotificationEnabled : true,
		additionalData : {
			"@odata.type" : "#microsoft.graph.incomingCallOptions",
		},
	},
	participantCapacity : 200,
};

const result = async () => {
	await graphServiceClient.communications.callsById("call-id").answer.post(requestBody);
}


```