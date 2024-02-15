<!-- Start SDK Example Usage [usage] -->
```java
package hello.world;

import com.example.test_without_webhooks.TestWithoutWebhooks;
import com.example.test_without_webhooks.models.operations.PostSendPetResponse;
import com.example.test_without_webhooks.models.shared.Pet1;

public class Application {
    public static void main(String[] args) {
        try {
            TestWithoutWebhooks sdk = TestWithoutWebhooks.builder()            .build();

            com.example.test_without_webhooks.models.shared.Pet1 req = new Pet1(
                794362L,
                "<value>"){{
                tag = "<value>";

            }};

            com.example.test_without_webhooks.models.operations.PostSendPetResponse res = sdk.postSendPet(req);

            if (res.statusCode == 200) {
                // handle response
            }
        } catch (Exception e) {
            // handle exception
        }
    }
}
```
<!-- End SDK Example Usage [usage] -->