---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Channel = {
	membershipType : ChannelMembershipType.Private,
	displayName : "My First Private Channel",
	description : "This is my first private channels",
	members : [
		{
			roles : [
				"owner",
			],
			additionalData : {
				"@odata.type" : "#microsoft.graph.aadUserConversationMember",
				"user@odata.bind" : "https://graph.microsoft.com/v1.0/users('62855810-484b-4823-9e01-60667f8b12ae')",
			},
		},
	],
	additionalData : {
		"@odata.type" : "#Microsoft.Graph.channel",
	},
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").channels.post(requestBody);
}


```