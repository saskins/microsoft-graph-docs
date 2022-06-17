---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDomain()
id := "contoso.com"
requestBody.SetId(&id)
result, err := graphClient.Domains().Post(requestBody)


```