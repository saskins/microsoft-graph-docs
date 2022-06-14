---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EducationUser = {
	primaryRole : EducationUserRole.String,
	middleName : "String",
	externalSource : EducationExternalSource.String,
	externalSourceDetail : "String",
	residenceAddress : {
		additionalData : {
			"@odata.type" : "microsoft.graph.physicalAddress",
		},
	},
	mailingAddress : {
		additionalData : {
			"@odata.type" : "microsoft.graph.physicalAddress",
		},
	},
	student : {
		additionalData : {
			"@odata.type" : "microsoft.graph.educationStudent",
		},
	},
	teacher : {
		additionalData : {
			"@odata.type" : "microsoft.graph.educationTeacher",
		},
	},
	createdBy : {
		additionalData : {
			"@odata.type" : "microsoft.graph.identitySet",
		},
	},
	accountEnabled : "Boolean",
	assignedLicenses : [
		{
			additionalData : {
				"@odata.type" : "microsoft.graph.assignedLicense",
			},
		},
	],
	assignedPlans : [
		{
			additionalData : {
				"@odata.type" : "microsoft.graph.assignedPlan",
			},
		},
	],
	businessPhones : [
		"String",
	],
	department : "String",
	displayName : "String",
	givenName : "String",
	mail : "String",
	mailNickname : "String",
	mobilePhone : "String",
	passwordPolicies : "String",
	passwordProfile : {
		additionalData : {
			"@odata.type" : "microsoft.graph.passwordProfile",
		},
	},
	officeLocation : "String",
	preferredLanguage : "String",
	provisionedPlans : [
		{
			additionalData : {
				"@odata.type" : "microsoft.graph.provisionedPlan",
			},
		},
	],
	refreshTokensValidFromDateTime : new Date("String (timestamp)"),
	showInAddressList : "Boolean",
	surname : "String",
	usageLocation : "String",
	userPrincipalName : "String",
	userType : "String",
	onPremisesInfo : {
		additionalData : {
			"@odata.type" : "microsoft.graph.educationOnPremisesInfo",
		},
	},
	additionalData : {
		"@odata.type" : "#microsoft.graph.educationUser",
	},
};

const result = async () => {
	await graphServiceClient.education.users.post(requestBody);
}


```