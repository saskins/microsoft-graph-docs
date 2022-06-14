---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ClonePostRequestBody = {
	displayName : "Library Assist",
	description : "Self help community for library",
	mailNickname : "libassist",
	partsToClone : ClonableTeamParts.Apps,tabs,settings,channels,members,
	visibility : TeamVisibilityType.Public,
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").clone.post(requestBody);
}


```