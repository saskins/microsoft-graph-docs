---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : TenantCustomizedInformation = {
	tenantId : "String",
	contacts : [
		{
			name : "String",
			title : "String",
			email : "String",
			phone : "String",
			notes : "String",
			additionalData : {
				"@odata.type" : "microsoft.graph.managedTenants.tenantContactInformation",
			},
		},
	],
	website : "String",
	additionalData : {
		"@odata.type" : "#microsoft.graph.managedTenants.tenantCustomizedInformation",
	},
};

const result = async () => {
	await graphServiceClient.tenantRelationships.managedTenants.tenantsCustomizedInformationById("tenantCustomizedInformation-id").patch(requestBody);
}


```