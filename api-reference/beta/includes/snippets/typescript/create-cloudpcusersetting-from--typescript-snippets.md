---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CloudPcUserSetting = {
	displayName : "Example",
	selfServiceEnabled : false,
	localAdminEnabled : true,
	restorePointSetting : {
		frequencyInHours : 16,
		userRestoreEnabled : true,
	},
	additionalData : {
		"@odata.type" : "#microsoft.graph.cloudPcUserSetting",
	},
};

const result = async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.userSettings.post(requestBody);
}


```