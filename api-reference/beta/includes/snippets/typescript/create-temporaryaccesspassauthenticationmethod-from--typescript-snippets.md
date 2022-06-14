---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : TemporaryAccessPassAuthenticationMethod = {
	startDateTime : new Date("2021-01-26T00:00:00.000Z"),
	lifetimeInMinutes : 60,
	isUsableOnce : false,
	additionalData : {
		"@odata.type" : "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
	},
};

const result = async () => {
	await graphServiceClient.usersById("user-id").authentication.temporaryAccessPassMethods.post(requestBody);
}


```