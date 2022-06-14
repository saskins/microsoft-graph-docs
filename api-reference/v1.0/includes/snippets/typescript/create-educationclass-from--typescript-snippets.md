---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EducationClass = {
	displayName : "String",
	mailNickname : "String",
	description : "String",
	createdBy : {
		additionalData : {
			"@odata.type" : "microsoft.graph.identitySet",
		},
	},
	classCode : "String",
	externalName : "String",
	externalId : "String",
	externalSource : EducationExternalSource.String,
	externalSourceDetail : "String",
	grade : "String",
	term : {
		additionalData : {
			"@odata.type" : "microsoft.graph.educationTerm",
		},
	},
	additionalData : {
		"@odata.type" : "#microsoft.graph.educationClass",
	},
};

const result = async () => {
	await graphServiceClient.education.classes.post(requestBody);
}


```