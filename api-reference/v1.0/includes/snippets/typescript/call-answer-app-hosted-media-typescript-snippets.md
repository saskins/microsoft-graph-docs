---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AnswerPostRequestBody = {
	callbackUri : "https://bot.contoso.com/api/calls",
	acceptedModalities : [
		"audio",
	],
	mediaConfig : {
		additionalData : {
			"@odata.type" : "#microsoft.graph.appHostedMediaConfig",
			"blob" : "<Media Session Configuration Blob>",
		},
	},
};

const result = async () => {
	await graphServiceClient.communications.callsById("call-id").answer.post(requestBody);
}


```