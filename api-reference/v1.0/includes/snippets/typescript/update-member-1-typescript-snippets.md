---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ConversationMember = {
	roles : [
		"owner",
	],
	additionalData : {
		"@odata.type" : "#microsoft.graph.aadUserConversationMember",
	},
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").channelsById("channel-id").membersById("conversationMember-id").patch(requestBody);
}


```