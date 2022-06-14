---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : TeamPostRequestBody = {
	additionalData : {
		memberSettings : {
			allowCreatePrivateChannels : true,
			allowCreateUpdateChannels : true,
		},
		messagingSettings : {
			allowUserEditMessages : true,
			allowUserDeleteMessages : true,
		},
		funSettings : {
			allowGiphy : true,
			giphyContentRating : "strict",
		},
	},
};

async () => {
	await graphServiceClient.groupsById("group-id").team.put(requestBody);
}


```