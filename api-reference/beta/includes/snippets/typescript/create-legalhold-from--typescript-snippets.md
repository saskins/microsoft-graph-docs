---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : LegalHold = {
	description : "String",
	createdBy : {
		additionalData : {
			"@odata.type" : "microsoft.graph.identitySet",
		},
	},
	isEnabled : "Boolean",
	status : LegalHoldStatus.String,
	contentQuery : "String",
	errors : [
		"String",
	],
	displayName : "String",
	additionalData : {
		"@odata.type" : "#microsoft.graph.ediscovery.legalHold",
	},
};

const result = async () => {
	await graphServiceClient.compliance.ediscovery.casesById("case-id").legalHolds.post(requestBody);
}


```