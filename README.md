# test-without-webhooks

<div align="left">
    <a href="https://speakeasyapi.dev/"><img src="https://custom-icon-badges.demolab.com/badge/-Built%20By%20Speakeasy-212015?style=for-the-badge&logoColor=FBE331&logo=speakeasy&labelColor=545454" /></a>
    <a href="https://github.com/speakeasy-sdks/test-without-webhooks-java-sdk.git/actions"><img src="https://img.shields.io/github/actions/workflow/status/speakeasy-sdks/bolt-php/speakeasy_sdk_generation.yml?style=for-the-badge" /></a>
    
</div>

<!-- Start SDK Installation -->
## SDK Installation

### Gradle

```groovy
implementation 'com.example.test_without_webhooks:test-without-webhooks:0.1.1'
```
<!-- End SDK Installation -->

## SDK Example Usage
<!-- Start SDK Example Usage -->


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

            com.example.test_without_webhooks.models.shared.Pet1 req = new Pet1(548814L, "provident") {{
                tag = "distinctio";
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
<!-- End SDK Example Usage -->

<!-- Start SDK Available Operations -->
## Available Resources and Operations

### [TestWithoutWebhooks SDK](docs/sdks/testwithoutwebhooks/README.md)

* [postSendPet](docs/sdks/testwithoutwebhooks/README.md#postsendpet)
<!-- End SDK Available Operations -->

### Maturity

This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage
to a specific package version. This way, you can install the same version each time without breaking changes unless you are intentionally
looking for the latest version.

### Contributions

While we value open-source contributions to this SDK, this library is generated programmatically.
Feel free to open a PR or a Github issue as a proof of concept and we'll do our best to include it in a future release!

### SDK Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
