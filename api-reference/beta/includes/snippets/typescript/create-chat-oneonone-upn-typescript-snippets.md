---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Chat = {
	chatType : ChatType.OneOnOne,
	members : [
		{
			roles : [
				"owner",
			],
			additionalData : {
				"@odata.type" : "#microsoft.graph.aadUserConversationMember",
				"user@odata.bind" : "https://graph.microsoft.com/beta/users('jacob@contoso.com')",
			},
		},
		{
			roles : [
				"owner",
			],
			additionalData : {
				"@odata.type" : "#microsoft.graph.aadUserConversationMember",
				"user@odata.bind" : "https://graph.microsoft.com/beta/users('alex@contoso.com')",
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.chats.post(requestBody);
}


```