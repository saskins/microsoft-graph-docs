---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewColumnDefinition()
requestBody.SetAdditionalData(map[string]interface{}{
	"sourceColumn@odata.bind": "https://graph.microsoft.com/beta/sites/root/columns/99ddcf45-e2f7-4f17-82b0-6fba34445103",
}
siteId := "site-id"
contentTypeId := "contentType-id"
result, err := graphClient.SitesById(&siteId).ContentTypesById(&contentTypeId).Columns().Post(requestBody)


```