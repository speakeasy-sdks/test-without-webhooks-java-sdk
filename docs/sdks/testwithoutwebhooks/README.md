# TestWithoutWebhooks SDK


## Overview

### Available Operations

* [postSendPet](#postsendpet)

## postSendPet

### Example Usage

```java
package hello.world;

import com.example.test_without_webhooks.TestWithoutWebhooks;
import com.example.test_without_webhooks.models.operations.PostSendPetResponse;
import com.example.test_without_webhooks.models.shared.Pet1;

public class Application {
    public static void main(String[] args) {
        try {
            TestWithoutWebhooks sdk = TestWithoutWebhooks.builder()
                .build();

            com.example.test_without_webhooks.models.shared.Pet1 req = new Pet1(794362L, "string"){{
                tag = "string";
            }};            

            PostSendPetResponse res = sdk.postSendPet(req);

            if (res.statusCode == 200) {
                // handle response
            }
        } catch (Exception e) {
            // handle exception
        }
    }
}
```

### Parameters

| Parameter                                                                           | Type                                                                                | Required                                                                            | Description                                                                         |
| ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| `request`                                                                           | [com.example.test_without_webhooks.models.shared.Pet1](../../models/shared/Pet1.md) | :heavy_check_mark:                                                                  | The request object to use for the request.                                          |


### Response

**[com.example.test_without_webhooks.models.operations.PostSendPetResponse](../../models/operations/PostSendPetResponse.md)**

