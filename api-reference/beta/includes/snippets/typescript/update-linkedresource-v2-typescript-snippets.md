---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : LinkedResource_v2 = {
	webUrl : "https://microsoft.com",
	applicationName : "Microsoft",
	displayName : "Microsoft Web page",
	externalId : "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9",
};

const result = async () => {
	await graphServiceClient.me.tasks.listsById("baseTaskList-id").tasksById("baseTask-id").linkedResourcesById("linkedResource_v2-id").patch(requestBody);
}


```