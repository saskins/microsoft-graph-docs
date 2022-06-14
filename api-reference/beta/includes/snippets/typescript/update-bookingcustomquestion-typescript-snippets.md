---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BookingCustomQuestion = {
	displayName : "What is your age?",
	answerInputType : AnswerInputType.Text,
	answerOptions : [
	],
	additionalData : {
		"@odata.type" : "#microsoft.graph.bookingCustomQuestion",
	},
};

const result = async () => {
	await graphServiceClient.bookingBusinessesById("bookingBusiness-id").customQuestionsById("bookingCustomQuestion-id").patch(requestBody);
}


```