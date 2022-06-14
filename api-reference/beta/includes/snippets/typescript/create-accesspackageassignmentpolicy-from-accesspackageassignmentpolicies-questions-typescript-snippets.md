---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessPackageAssignmentPolicy = {
	accessPackageId : "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
	displayName : "Users from connected organizations can request",
	description : "Allow users from configured connected organizations to request and be approved by their sponsors",
	canExtend : false,
	durationInDays : 365,
	expirationDateTime : null,
	requestorSettings : {
		scopeType : "AllExistingConnectedOrganizationSubjects",
		acceptRequests : true,
	},
	requestApprovalSettings : {
		isApprovalRequired : true,
		isApprovalRequiredForExtension : false,
		isRequestorJustificationRequired : true,
		approvalMode : "SingleStage",
		approvalStages : [
			{
				approvalStageTimeOutInDays : 14,
				isApproverJustificationRequired : true,
				isEscalationEnabled : false,
				escalationTimeInMinutes : 11520,
				primaryApprovers : [
					{
						isBackup : true,
						additionalData : {
							"@odata.type" : "#microsoft.graph.groupMembers",
							"id" : "d2dcb9a1-a445-42ee-83a8-476522ed6cbf",
							"description" : "group for users from connected organizations which have no external sponsor",
						},
					},
					{
						isBackup : false,
						additionalData : {
							"@odata.type" : "#microsoft.graph.externalSponsors",
						},
					},
				],
			},
		],
	},
	questions : [
		{
			isRequired : false,
			text : {
				defaultText : "what state are you from?",
				localizedTexts : [
					{
						text : "¿De qué estado eres?",
						languageCode : "es",
					},
				],
			},
			additionalData : {
				"@odata.type" : "#microsoft.graph.accessPackageMultipleChoiceQuestion",
				choices : [
					{
						actualValue : "AZ",
						displayValue : {
							localizedTexts : [
								{
									text : "Arizona",
									languageCode : "es",
								},
							],
						},
					},
					{
						actualValue : "CA",
						displayValue : {
							localizedTexts : [
								{
									text : "California",
									languageCode : "es",
								},
							],
						},
					},
					{
						actualValue : "OH",
						displayValue : {
							localizedTexts : [
								{
									text : "Ohio",
									languageCode : "es",
								},
							],
						},
					},
				],
				allowsMultipleSelection : false,
			},
		},
		{
			isRequired : false,
			text : {
				defaultText : "Who is your manager?",
				localizedTexts : [
					{
						text : "por qué necesita acceso a este paquete",
						languageCode : "es",
					},
				],
			},
			additionalData : {
				"@odata.type" : "#microsoft.graph.accessPackageTextInputQuestion",
				isSingleLineQuestion : false,
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageAssignmentPolicies.post(requestBody);
}


```