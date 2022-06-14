---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : MobilityManagementPolicy = {
	complianceUrl : "https://portal.mg.contoso.com/?portalAction=Compliance",
	discoveryUrl : "https://enrollment.mg.contoso.com/enrollmentserver/discovery.svc",
	termsOfUseUrl : "https://portal.mg.contoso.com/TermsofUse.aspx",
	additionalData : {
		"@odata.type" : "#microsoft.graph.mobilityManagementPolicy",
	},
};

const result = async () => {
	await graphServiceClient.policies.mobileAppManagementPoliciesById("mobilityManagementPolicy-id").patch(requestBody);
}


```