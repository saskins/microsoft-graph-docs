---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
sourceCollection := msgraphsdk.NewSourceCollection()
requestBody.SetSourceCollection(sourceCollection)
id := "1a9b4145d8f84e39bc45a7f68c5c5119"
sourceCollection.SetId(&id)
requestBody.SetAdditionalData(map[string]interface{}{
	"additionalData": "linkedFiles",
}
caseId := "case-id"
reviewSetId := "reviewSet-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).ReviewSetsById(&reviewSetId).AddToReviewSet(case-id, reviewSet-id).Post(requestBody)


```