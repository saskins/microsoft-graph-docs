---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOpenShiftChangeRequest()
senderMessage := "Can I take this shift?"
requestBody.SetSenderMessage(&senderMessage)
openShiftId := "577b75d2-a927-48c0-a5d1-dc984894e7b8"
requestBody.SetOpenShiftId(&openShiftId)
headers := map[string]string{
	"Authorization": "Bearer {token}"
}
options := &msgraphsdk.OpenShiftChangeRequestsRequestBuilderPostRequestConfiguration{
	Headers: headers,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().OpenShiftChangeRequests().PostWithRequestConfigurationAndResponseHandler(requestBody, options, nil)


```