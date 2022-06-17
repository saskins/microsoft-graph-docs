---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOpenShift()
id := "OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8"
requestBody.SetId(&id)
schedulingGroupId := "TAG_228940ed-ff84-4e25-b129-1b395cf78be0"
requestBody.SetSchedulingGroupId(&schedulingGroupId)
sharedOpenShift := msgraphsdk.NewOpenShiftItem()
requestBody.SetSharedOpenShift(sharedOpenShift)
notes := "InventoryManagement"
sharedOpenShift.SetNotes(&notes)
openSlotCount := int32(2)
sharedOpenShift.SetOpenSlotCount(&openSlotCount)
displayName := "Dayshift"
sharedOpenShift.SetDisplayName(&displayName)
startDateTime, err := time.Parse(time.RFC3339, "2018-10-04T00: 58: 45.340Z")
sharedOpenShift.SetStartDateTime(&startDateTime)
endDateTime, err := time.Parse(time.RFC3339, "2018-10-04T09: 50: 45.332Z")
sharedOpenShift.SetEndDateTime(&endDateTime)
theme := "white"
sharedOpenShift.SetTheme(&theme)
sharedOpenShift.SetActivities( []ShiftActivity {
	msgraphsdk.NewShiftActivity(),
isPaid := true
	SetIsPaid(&isPaid)
startDateTime, err := time.Parse(time.RFC3339, "2018-10-04T00: 58: 45.340Z")
	SetStartDateTime(&startDateTime)
endDateTime, err := time.Parse(time.RFC3339, "2018-10-04T01: 58: 45.340Z")
	SetEndDateTime(&endDateTime)
code := ""
	SetCode(&code)
displayName := "Lunch"
	SetDisplayName(&displayName)
}
requestBody.SetDraftOpenShift(nil)
createdDateTime, err := time.Parse(time.RFC3339, "2019-03-14T04: 32: 51.451Z")
requestBody.SetCreatedDateTime(&createdDateTime)
lastModifiedDateTime, err := time.Parse(time.RFC3339, "2019-03-14T05: 32: 51.451Z")
requestBody.SetLastModifiedDateTime(&lastModifiedDateTime)
lastModifiedBy := msgraphsdk.NewIdentitySet()
requestBody.SetLastModifiedBy(lastModifiedBy)
lastModifiedBy.SetApplication(nil)
lastModifiedBy.SetDevice(nil)
user := msgraphsdk.NewIdentity()
lastModifiedBy.SetUser(user)
id := "366c0b19-49b1-41b5-a03f-9f3887bd0ed8"
user.SetId(&id)
displayName := "JohnDoe"
user.SetDisplayName(&displayName)
lastModifiedBy.SetAdditionalData(map[string]interface{}{
	"conversation": nil,
}
headers := map[string]string{
	"Authorization": "Bearer {token}"
}
options := &msgraphsdk.OpenShiftsRequestBuilderPostRequestConfiguration{
	Headers: headers,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().OpenShifts().PostWithRequestConfigurationAndResponseHandler(requestBody, options, nil)


```