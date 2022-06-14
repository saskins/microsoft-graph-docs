---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : UnifiedRoleManagementPolicyRule = {
	id : "Expiration_EndUser_Assignment",
	target : {
		caller : "EndUser",
		operations : [
			"All",
		],
		level : "Assignment",
		inheritableSettings : [
		],
		enforcedSettings : [
		],
		additionalData : {
			"@odata.type" : "microsoft.graph.unifiedRoleManagementPolicyRuleTarget",
		},
	},
	additionalData : {
		"@odata.type" : "#microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
		isExpirationRequired : true,
		"maximumDuration" : "PT1H45M",
	},
};

const result = async () => {
	await graphServiceClient.policies.roleManagementPoliciesById("unifiedRoleManagementPolicy-id").rulesById("unifiedRoleManagementPolicyRule-id").patch(requestBody);
}


```