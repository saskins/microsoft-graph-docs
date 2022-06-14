---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Acronym = {
	displayName : "DNN",
	standsFor : "Deep Neural Network",
	description : "A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers.",
	webUrl : "http://microsoft.com/deep-neural-network",
	state : AnswerState.Draft,
};

const result = async () => {
	await graphServiceClient.search.acronyms.post(requestBody);
}


```