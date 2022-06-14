---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Call = {
	callbackUri : "https://bot.contoso.com/callback",
	source : {
		identity : {
			application : {
				displayName : "Calling Bot",
				id : "2891555a-92ff-42e6-80fa-6e1300c6b5c6",
				additionalData : {
					"@odata.type" : "#microsoft.graph.identity",
				},
			},
			additionalData : {
				"@odata.type" : "#microsoft.graph.identitySet",
			},
		},
		region : null,
		languageId : null,
		additionalData : {
			"@odata.type" : "#microsoft.graph.participantInfo",
		},
	},
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
			"@odata.type" : "#microsoft.graph.appHostedMediaConfig",
			"blob" : "<Media Session Configuration>",
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