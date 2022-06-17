---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.NoncustodialDataSourcesRequestBuilderGetQueryParameters{
	Expand: "dataSource",
}
options := &msgraphsdk.NoncustodialDataSourcesRequestBuilderGetRequestConfiguration{
	QueryParameters: requestParameters,
}
ediscoveryCaseId := "ediscoveryCase-id"
result, err := graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).NoncustodialDataSources().GetWithRequestConfigurationAndResponseHandler(options, nil)


```