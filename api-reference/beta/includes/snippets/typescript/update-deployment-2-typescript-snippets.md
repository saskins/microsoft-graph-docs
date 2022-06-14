---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Deployment = {
	settings : {
		monitoring : {
			monitoringRules : [
				{
					signal : MonitoringSignal.Rollback,
					threshold : 5,
					action : MonitoringAction.PauseDeployment,
				},
			],
		},
		additionalData : {
			"@odata.type" : "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
		},
	},
	additionalData : {
		"@odata.type" : "#microsoft.graph.windowsUpdates.deployment",
	},
};

const result = async () => {
	await graphServiceClient.admin.windows.updates.deploymentsById("deployment-id").patch(requestBody);
}


```