---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CloudPcOrganizationSettings = {
	userAccountType : CloudPcUserAccountType.StandardUser,
	osVersion : CloudPcOperatingSystem.Windows11,
	windowsSettings : {
		language : "en-US",
	},
	additionalData : {
		"@odata.type" : "#microsoft.graph.cloudPcOrganizationSettings",
	},
};

const result = async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.organizationSettings.patch(requestBody);
}


```