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
			additionalData : {
				"@odata.type" : "#microsoft.graph.identitySet",
				applicationInstance : {
					"@odata.type" : "#microsoft.graph.identity",
					displayName : "Calling Bot",
					id : "3d913abb-aec0-4964-8fa6-3c6850c4f278",
				},
			},
		},
		countryCode : null,
		endpointType : null,
		region : null,
		languageId : null,
		additionalData : {
			"@odata.type" : "#microsoft.graph.participantInfo",
		},
	},
	targets : [
		{
			identity : {
				additionalData : {
					"@odata.type" : "#microsoft.graph.identitySet",
					phone : {
						"@odata.type" : "#microsoft.graph.identity",
						id : "+12345678901",
					},
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
	tenantId : "aa67bd4c-8475-432d-bd41-39f255720e0a",
	additionalData : {
		"@odata.type" : "#microsoft.graph.call",
	},
};

const result = async () => {
	await graphServiceClient.communications.calls.post(requestBody);
}


```