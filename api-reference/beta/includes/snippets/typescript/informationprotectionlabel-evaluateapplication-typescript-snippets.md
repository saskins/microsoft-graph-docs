---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"User-Agent": "ContosoLOBApp/1.0",
	}
};
const requestBody : EvaluateApplicationPostRequestBody = {
	contentInfo : {
		format : ContentFormat.Default,
		identifier : null,
		state : ContentState.Rest,
		metadata : [
			{
				name : "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled",
				value : "True",
				additionalData : {
					"@odata.type" : "#microsoft.graph.keyValuePair",
				},
			},
			{
				name : "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method",
				value : "Standard",
				additionalData : {
					"@odata.type" : "#microsoft.graph.keyValuePair",
				},
			},
			{
				name : "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate",
				value : "1/1/0001 12:00:00 AM",
				additionalData : {
					"@odata.type" : "#microsoft.graph.keyValuePair",
				},
			},
			{
				name : "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId",
				value : "cfa4cf1d-a337-4481-aa99-19d8f3d63f7c",
				additionalData : {
					"@odata.type" : "#microsoft.graph.keyValuePair",
				},
			},
			{
				name : "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name",
				value : "General",
				additionalData : {
					"@odata.type" : "#microsoft.graph.keyValuePair",
				},
			},
			{
				name : "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits",
				value : "0",
				additionalData : {
					"@odata.type" : "#microsoft.graph.keyValuePair",
				},
			},
			{
				name : "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId",
				value : "00000000-0000-0000-0000-000000000000",
				additionalData : {
					"@odata.type" : "#microsoft.graph.keyValuePair",
				},
			},
		],
		additionalData : {
			"@odata.type" : "#microsoft.graph.contentInfo",
			"format@odata.type" : "#microsoft.graph.contentFormat",
			"state@odata.type" : "#microsoft.graph.contentState",
			"metadata@odata.type" : "#Collection(microsoft.graph.keyValuePair)",
		},
	},
	labelingOptions : {
		assignmentMethod : AssignmentMethod.Standard,
		labelId : "97309856-9c28-4ac6-9382-5f8bc20c457b",
		downgradeJustification : null,
		extendedProperties : [
		],
		additionalData : {
			"@odata.type" : "#microsoft.graph.labelingOptions",
			"assignmentMethod@odata.type" : "#microsoft.graph.assignmentMethod",
			"labelId@odata.type" : "#Guid",
			"extendedProperties@odata.type" : "#Collection(microsoft.graph.keyValuePair)",
		},
	},
};

const result = async () => {
	await graphServiceClient.informationProtection.policy.labels.evaluateApplication.post(requestBody, configuration);
}


```