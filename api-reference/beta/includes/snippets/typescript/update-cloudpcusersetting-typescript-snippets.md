---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CloudPcUserSetting = {
	displayName : "Example",
	selfServiceEnabled : true,
	restorePointSetting : {
		frequencyInHours : 16,
		userRestoreEnabled : true,
	},
	localAdminEnabled : false,
	additionalData : {
		"@odata.type" : "#microsoft.graph.cloudPcUserSetting",
	},
};

const result = async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.userSettingsById("cloudPcUserSetting-id").patch(requestBody);
}


```