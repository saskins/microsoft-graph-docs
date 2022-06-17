---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.PrivilegedOperationEventsRequestBuilderGetQueryParameters{
	Filter: "requestType%20eq%20'Deactivate'",
}
options := &msgraphsdk.PrivilegedOperationEventsRequestBuilderGetRequestConfiguration{
	QueryParameters: requestParameters,
}
result, err := graphClient.PrivilegedOperationEvents().GetWithRequestConfigurationAndResponseHandler(options, nil)


```