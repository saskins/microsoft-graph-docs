---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SchemaExtension = {
	id : "courses",
	description : "Graph Learn training courses extensions",
	targetTypes : [
		"Group",
	],
	properties : [
		{
			additionalData : {
				"name" : "courseId",
				"type" : "Integer",
			},
		},
		{
			additionalData : {
				"name" : "courseName",
				"type" : "String",
			},
		},
		{
			additionalData : {
				"name" : "courseType",
				"type" : "String",
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.schemaExtensions.post(requestBody);
}


```