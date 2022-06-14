---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EdiscoveryNoncustodialDataSource = {
	dataSource : {
		additionalData : {
			"@odata.type" : "microsoft.graph.security.siteSource",
			site : {
				webUrl : "https://m365x809305.sharepoint.com/sites/Design-topsecret",
			},
		},
	},
};

const result = async () => {
	await graphServiceClient.security.cases.ediscoveryCasesById("ediscoveryCase-id").noncustodialDataSources.post(requestBody);
}


```