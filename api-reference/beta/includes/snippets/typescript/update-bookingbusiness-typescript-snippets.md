---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BookingBusiness = {
	email : "admin@fabrikam.com",
	schedulingPolicy : {
		timeSlotInterval : "PT60M",
		minimumLeadTime : "P1D",
		maximumAdvance : "P30D",
		sendConfirmationsToOwner : true,
		allowStaffSelection : true,
	},
};

const result = async () => {
	await graphServiceClient.bookingBusinessesById("bookingBusiness-id").patch(requestBody);
}


```