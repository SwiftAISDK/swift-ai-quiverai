<!-- Generated distribution; edit the canonical repository. -->
# swift-ai-quiverai 1.2.0

Independent Swift-native port of Vercel AI SDK. Source and upstream dispositions are in PROVENANCE.json and Porting/.

## Distribution manifest

Add this package to your SwiftPM dependencies:

```swift
.package(url: "https://github.com/SwiftAISDK/swift-ai-quiverai.git", from: "1.2.0")
```

Products: `SwiftAIQuiverAI`.
Contribute and report issues in the canonical SwiftAISDK repository.

## Authored usage guide

# QuiverAI for Swift

`SwiftAIQuiverAI` adds QuiverAI to [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK), an independent Swift port of the Vercel AI SDK. It ports `@ai-sdk/quiverai` and supports text generation and image generation.

Provider guide with models, options, streaming and errors:

- [QuiverAI](https://swiftaisdk.github.io/SwiftAISDK/providers/quiverai/)

## Usage

Add the `SwiftAI` product from `swift-ai-core` and the `SwiftAIQuiverAI` product from this package to your target, then create the provider:

```swift
import SwiftAI
import SwiftAIQuiverAI

let provider = try AIProviders.quiverAI(configuration: QuiverAIProviderSettings())
```

By default the provider reads `QUIVERAI_API_KEY` and `QUIVERAI_BASE_URL` from the environment; values set in `QuiverAIProviderSettings` take precedence.

To use every provider through one dependency, add the complete [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) package instead; see [Install](https://swiftaisdk.github.io/SwiftAISDK/getting-started/install/).

## Contributing

This package is exported from `Packages/swift-ai-quiverai` in the canonical [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) repository. Open issues and pull requests there.
