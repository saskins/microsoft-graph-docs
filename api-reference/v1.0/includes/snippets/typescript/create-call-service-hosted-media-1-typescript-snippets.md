---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Call = {
	callbackUri : "https://bot.contoso.com/callback",
	targets : [
		{
			identity : {
				user : {
					displayName : "John",
					id : "112f7296-5fa4-42ca-bae8-6a692b15d4b8",
					additionalData : {
						"@odata.type" : "#microsoft.graph.identity",
					},
				},
				additionalData : {
					"@odata.type" : "#microsoft.graph.identitySet",
				},
			},
			additionalData : {
				"@odata.type" : "#microsoft.graph.invitationParticipantInfo",
			},
		},
	],
	requestedModalities : [
		"audio",
	],
	mediaConfig : {
		additionalData : {
			"@odata.type" : "#microsoft.graph.serviceHostedMediaConfig",
		},
	},
	additionalData : {
		"@odata.type" : "#microsoft.graph.call",
	},
};

const result = async () => {
	await graphServiceClient.communications.calls.post(requestBody);
}


```