---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PhoneMethod = {
	additionalData : {
		"phoneNumber" : "+1 2065555554",
		"phoneType" : "mobile",
	},
};

async () => {
	await graphServiceClient.me.authentication.phoneMethodsById("phoneAuthenticationMethod-id").put(requestBody);
}


```