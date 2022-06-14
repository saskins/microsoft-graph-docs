---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AuthenticationContextClassReference = {
	additionalData : {
		value : [
			{
				displayName : "Contoso trusted locations",
				description : "Access is only allowed from trusted locations",
				isAvailable : true,
			},
		],
	},
};

const result = async () => {
	await graphServiceClient.identity.conditionalAccess.authenticationContextClassReferencesById("authenticationContextClassReference-id").patch(requestBody);
}


```