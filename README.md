<!-- Generated distribution; edit the canonical repository. -->
# swift-ai-revai 1.2.0

Independent Swift-native port of Vercel AI SDK. Source and upstream dispositions are in PROVENANCE.json and Porting/.

## Distribution manifest

Add this package to your SwiftPM dependencies:

```swift
.package(url: "https://github.com/SwiftAISDK/swift-ai-revai.git", from: "1.2.0")
```

Products: `SwiftAIRevAI`.
Contribute and report issues in the canonical SwiftAISDK repository.

## Authored usage guide

# Rev.ai for Swift

`SwiftAIRevAI` adds Rev.ai to [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK), an independent Swift port of the Vercel AI SDK. It ports `@ai-sdk/revai` and supports transcription.

Provider guide with models, options, streaming and errors:

- [Rev.ai](https://swiftaisdk.github.io/SwiftAISDK/providers/revai/)

## Usage

Add the `SwiftAI` product from `swift-ai-core` and the `SwiftAIRevAI` product from this package to your target, then create the provider:

```swift
import SwiftAI
import SwiftAIRevAI

let provider = try AIProviders.revAI(configuration: RevAIProviderSettings())
```

By default the provider reads `REVAI_API_KEY` from the environment; values set in `RevAIProviderSettings` take precedence.

To use every provider through one dependency, add the complete [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) package instead; see [Install](https://swiftaisdk.github.io/SwiftAISDK/getting-started/install/).

## Contributing

This package is exported from `Packages/swift-ai-revai` in the canonical [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) repository. Open issues and pull requests there.
