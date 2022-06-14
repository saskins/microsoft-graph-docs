---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Item = {
	additionalData : {
		acl : [
			{
				type : "user",
				value : "e811976d-83df-4cbd-8b9b-5215b18aa874",
				accessType : "grant",
			},
			{
				type : "externalGroup",
				value : "14m1b9c38qe647f6a",
				accessType : "deny",
			},
		],
		properties : {
			title : "Error in the payment gateway",
			priority : 1,
			assignee : "john@contoso.com",
		},
		content : {
			value : "Error in payment gateway...",
			type : "text",
		},
	},
};

async () => {
	await graphServiceClient.external.connectionsById("externalConnection-id").itemsById("externalItem-id").put(requestBody);
}


```