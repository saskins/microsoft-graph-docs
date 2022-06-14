---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		format: "{format}",
	}
};

const result = async () => {
	await graphServiceClient.drive.itemsById("driveItem-id").content.get(configuration);
}


```