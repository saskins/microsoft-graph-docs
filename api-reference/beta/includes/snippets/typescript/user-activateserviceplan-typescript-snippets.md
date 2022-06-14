---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ActivateServicePlanPostRequestBody = {
	servicePlanId : "28f42d6f-8034-4a0f-9d8a-a218a63b3299",
	skuId : "465a2a90-5e59-456d-a7b8-127b9fb2e484",
};

const result = async () => {
	await graphServiceClient.me.activateServicePlan.post(requestBody);
}


```