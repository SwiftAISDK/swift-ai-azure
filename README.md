<!-- Generated distribution; edit the canonical repository. -->
# swift-ai-azure 1.0.0

Independent Swift-native port of Vercel AI SDK. Source and upstream dispositions are in PROVENANCE.json and Porting/.

## Distribution manifest

Add this package to your SwiftPM dependencies:

```swift
.package(url: "https://github.com/SwiftAISDK/swift-ai-azure.git", from: "1.0.0")
```

Products: `SwiftAIAzure`.
Contribute and report issues in the canonical SwiftAISDK repository.

## Authored usage guide

# SwiftAIAzure

Swift-native port of `@ai-sdk/azure`. Maintained in the canonical SwiftAISDK repository and exported as an independent Swift package.

```swift
import SwiftAIAzure

let provider = try AzureOpenAIProvider(resourceName: "my-resource",
    configuration: .init(apiKey: "..."))
let model = try provider.languageModel("deployment")
```

Azure owns its deployment/Foundry routing, token transport, MAI and Speech adapters.
OpenAI/compatible and DeepSeek implementations are reused through their explicit
hosting configurations. Existing capabilities and gaps remain unchanged.

Run `swift test --package-path Packages/swift-ai-azure` in the canonical checkout.
Distribution manifests and repositories are generated from the package catalog.

See [provider usage and capabilities](https://github.com/SwiftAISDK/SwiftAISDK/blob/main/docs-site/scripts/provider-guides/azure.md) for authentication, options and supported surfaces.
