---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BundlesPostRequestBody = {
	additionalData : {
		"name" : "Just some files",
		"@microsoft.graph.conflictBehavior" : "rename",
		bundle : {
		},
		children : [
			{
				id : "1234asdf",
			},
			{
				id : "1234qwerty",
			},
		],
	},
};

async () => {
	await graphServiceClient.drive.bundles.post(requestBody);
}


```