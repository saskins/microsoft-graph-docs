---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSwapShiftsChangeRequest()
senderShiftId := "5ad10161-6524-4c7c-9beb-4e8677ba2f6d"
requestBody.SetSenderShiftId(&senderShiftId)
senderMessage := "I can't make my shift, any chance we can swap?"
requestBody.SetSenderMessage(&senderMessage)
recipientUserId := "567c8ea5-9e32-422a-a663-8270201699cd"
requestBody.SetRecipientUserId(&recipientUserId)
recipientShiftId := "e73408ca-3ea5-4bbf-96a8-2e06c95f7a2c"
requestBody.SetRecipientShiftId(&recipientShiftId)
headers := map[string]string{
	"Authorization": "Bearer {token}"
}
options := &msgraphsdk.SwapShiftsChangeRequestsRequestBuilderPostRequestConfiguration{
	Headers: headers,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().SwapShiftsChangeRequests().PostWithRequestConfigurationAndResponseHandler(requestBody, options, nil)


```