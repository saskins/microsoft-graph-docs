---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ActivateServicePostRequestBody = {
	skuId : "6fd2c87f-b296-42f0-b197-1e91e994b900",
	servicePlanId : "a23b959c-7ce8-4e57-9140-b90eb88a9e97",
};

const result = async () => {
	await graphServiceClient.organizationById("organization-id").activateService.post(requestBody);
}


```