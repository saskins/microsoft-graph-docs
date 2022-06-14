---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"ConsistencyLevel": "eventual",
	}
,	queryParameters : {
		count: "true",
		orderBy: "deletedDateTime asc",
		select: "id,DisplayName,deletedDateTime",
	}
};

const result = async () => {
	await graphServiceClient.directory.deletedItems.group.get(configuration);
}


```