---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphusers "github.com/microsoftgraph/msgraph-sdk-go/users"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphusers.NewReplyAllPostRequestBody()
comment := "comment-value"
requestBody.SetComment(&comment) 

graphClient.Me().Messages().ByMessageId("message-id").ReplyAll().Post(context.Background(), requestBody, nil)


```