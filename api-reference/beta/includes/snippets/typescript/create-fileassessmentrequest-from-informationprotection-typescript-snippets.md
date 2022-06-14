---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ThreatAssessmentRequest = {
	expectedAssessment : ThreatExpectedAssessment.Block,
	category : ThreatCategory.Malware,
	additionalData : {
		"@odata.type" : "#microsoft.graph.fileAssessmentRequest",
		"fileName" : "test.txt",
		"contentData" : "VGhpcyBpcyBhIHRlc3QgZmlsZQ==",
	},
};

const result = async () => {
	await graphServiceClient.informationProtection.threatAssessmentRequests.post(requestBody);
}


```