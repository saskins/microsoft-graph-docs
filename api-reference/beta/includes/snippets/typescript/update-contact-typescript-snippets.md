---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Contact = {
	emailAddresses : [
		{
			additionalData : {
				"type" : "personal",
				"name" : "Pavel Bansky",
				"address" : "pavelb@adatum.onmicrosoft.com",
			},
		},
		{
			additionalData : {
				"address" : "pavelb@fabrikam.onmicrosoft.com",
				"name" : "Pavel Bansky",
				"type" : "other",
				"otherLabel" : "Volunteer work",
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.me.contactsById("contact-id").patch(requestBody);
}


```