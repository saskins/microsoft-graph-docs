---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ExternalItem = {
	acl : [
		{
			type : AclType.Everyone,
			value : "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
			accessType : AccessType.Grant,
		},
	],
};

const result = async () => {
	await graphServiceClient.external.connectionsById("externalConnection-id").itemsById("externalItem-id").patch(requestBody);
}


```