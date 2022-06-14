---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EducationSchool = {
	displayName : "String",
	description : "String",
	externalSource : EducationExternalSource.String,
	externalSourceDetail : "String",
	principalEmail : "String",
	principalName : "String",
	externalPrincipalId : "String",
	lowestGrade : "String",
	highestGrade : "String",
	schoolNumber : "String",
	externalId : "String",
	phone : "String",
	fax : "String",
	createdBy : {
		additionalData : {
			"@odata.type" : "microsoft.graph.identitySet",
		},
	},
	address : {
		additionalData : {
			"@odata.type" : "microsoft.graph.physicalAddress",
		},
	},
	additionalData : {
		"@odata.type" : "#microsoft.graph.educationSchool",
	},
};

const result = async () => {
	await graphServiceClient.education.schools.post(requestBody);
}


```