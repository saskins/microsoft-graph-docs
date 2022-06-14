---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EdiscoveryCaseSettings = {
	redundancyDetection : {
		additionalData : {
			"@odata.type" : "microsoft.graph.security.redundancyDetectionSettings",
		},
	},
	topicModeling : {
		additionalData : {
			"@odata.type" : "microsoft.graph.security.topicModelingSettings",
		},
	},
	ocr : {
		additionalData : {
			"@odata.type" : "microsoft.graph.security.ocrSettings",
		},
	},
	additionalData : {
		"@odata.type" : "#microsoft.graph.security.ediscoveryCaseSettings",
	},
};

const result = async () => {
	await graphServiceClient.security.cases.ediscoveryCasesById("ediscoveryCase-id").settings.patch(requestBody);
}


```