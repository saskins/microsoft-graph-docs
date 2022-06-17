---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewReviewSet()
displayName := "My Reviewset 3"
requestBody.SetDisplayName(&displayName)
caseId := "case-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).ReviewSets().Post(requestBody)


```