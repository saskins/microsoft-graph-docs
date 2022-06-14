---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Deployment = {
	content : {
		additionalData : {
			"@odata.type" : "microsoft.graph.windowsUpdates.featureUpdateReference",
			"version" : "20H2",
		},
	},
	settings : {
		rollout : {
			devicesPerOffer : 100,
		},
		monitoring : {
			monitoringRules : [
				{
					signal : MonitoringSignal.Rollback,
					threshold : 5,
					action : MonitoringAction.PauseDeployment,
					additionalData : {
						"@odata.type" : "#microsoft.graph.windowsUpdates.monitoringRule",
					},
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
	await graphServiceClient.admin.windows.updates.deployments.post(requestBody);
}


```