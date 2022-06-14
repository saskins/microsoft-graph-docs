---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BundlesPostRequestBody = {
	additionalData : {
		"name" : "My Day at the Beach",
		"@microsoft.graph.conflictBehavior" : "rename",
		bundle : {
			album : {
			},
		},
		children : [
			{
				id : "1234asdf",
			},
		],
	},
};

async () => {
	await graphServiceClient.drive.bundles.post(requestBody);
}


```