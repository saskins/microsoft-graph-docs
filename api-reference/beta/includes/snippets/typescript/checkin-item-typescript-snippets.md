---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CheckinPostRequestBody = {
	comment : "Updating the latest guidelines",
};

const result = async () => {
	await graphServiceClient.drivesById("drive-id").itemsById("driveItem-id").checkin.post(requestBody);
}


```