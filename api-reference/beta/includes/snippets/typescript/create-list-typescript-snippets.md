---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : List = {
	displayName : "Books",
	columns : [
		{
			name : "Author",
			text : {
			},
		},
		{
			name : "PageCount",
			number : {
			},
		},
	],
	list : {
		template : "genericList",
	},
};

const result = async () => {
	await graphServiceClient.sitesById("site-id").lists.post(requestBody);
}


```