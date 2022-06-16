---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGroup()
displayName := "myGroup"
requestBody.SetDisplayName(&displayName)
siteId := "site-id"
result, err := graphClient.SitesById(&siteId).TermStore().Groups().Post(requestBody)


```