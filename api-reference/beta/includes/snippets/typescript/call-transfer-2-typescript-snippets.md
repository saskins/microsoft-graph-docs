---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : TransferPostRequestBody = {
	transferTarget : {
		endpointType : EndpointType.Default,
		identity : {
			user : {
				id : "550fae72-d251-43ec-868c-373732c2704f",
				displayName : "Heidi Steen",
				additionalData : {
					"@odata.type" : "#microsoft.graph.identity",
					"tenantId" : "72f988bf-86f1-41af-91ab-2d7cd011db47",
				},
			},
			additionalData : {
				"@odata.type" : "#microsoft.graph.identitySet",
			},
		},
		replacesCallId : "e5d39592-99bd-4db8-bca8-30fb894ec51d",
		additionalData : {
			"@odata.type" : "#microsoft.graph.invitationParticipantInfo",
			"languageId" : "en-us",
			"region" : "amer",
		},
	},
};

const result = async () => {
	await graphServiceClient.communications.callsById("call-id").transfer.post(requestBody);
}


```