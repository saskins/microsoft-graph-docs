---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.PrivilegedOperationEventsRequestBuilderGetQueryParameters{
	Filter: "(creationDateTime%20ge%202017-06-25T07:00:00Z)%20and%20(creationDateTime%20le%202017-07-25T17:30:17Z)",
	Count: true,
	Orderby: "creationDateTime%20desc",
}
options := &msgraphsdk.PrivilegedOperationEventsRequestBuilderGetRequestConfiguration{
	QueryParameters: requestParameters,
}
result, err := graphClient.PrivilegedOperationEvents().GetWithRequestConfigurationAndResponseHandler(options, nil)


```