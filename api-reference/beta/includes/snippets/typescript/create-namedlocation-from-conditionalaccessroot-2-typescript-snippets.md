---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : NamedLocation = {
	displayName : "Named location with unknown countries and regions",
	additionalData : {
		"@odata.type" : "#microsoft.graph.countryNamedLocation",
		countriesAndRegions : [
			"US",
			"GB",
		],
		includeUnknownCountriesAndRegions : true,
	},
};

const result = async () => {
	await graphServiceClient.identity.conditionalAccess.namedLocations.post(requestBody);
}


```