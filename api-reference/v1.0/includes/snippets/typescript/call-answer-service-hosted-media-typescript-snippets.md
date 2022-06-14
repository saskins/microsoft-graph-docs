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
			"@odata.type" : "#microsoft.graph.serviceHostedMediaConfig",
			preFetchMedia : [
				{
					uri : "https://cdn.contoso.com/beep.wav",
					resourceId : "1D6DE2D4-CD51-4309-8DAA-70768651088E",
				},
				{
					uri : "https://cdn.contoso.com/cool.wav",
					resourceId : "1D6DE2D4-CD51-4309-8DAA-70768651088F",
				},
			],
		},
	},
};

const result = async () => {
	await graphServiceClient.communications.callsById("call-id").answer.post(requestBody);
}


```