<!-- Generated distribution; edit the canonical repository. -->
# swift-ai-revai 1.0.0

Independent Swift-native port of Vercel AI SDK. Source and upstream dispositions are in PROVENANCE.json and Porting/.

## Distribution manifest

Add this package to your SwiftPM dependencies:

```swift
.package(url: "https://github.com/SwiftAISDK/swift-ai-revai.git", from: "1.0.0")
```

Products: `SwiftAIRevAI`.
Contribute and report issues in the canonical SwiftAISDK repository.

## Authored usage guide

# SwiftAIRevAI

Swift-native port of `@ai-sdk/revai`. Maintained in the canonical SwiftAISDK repository and exported as an independent Swift package.

```swift
import SwiftAIRevAI

let provider = try RevAIProvider(configuration: .init(apiKey: "..."))
```

Settings accept a custom base URL, headers, query parameters and an injected
`AITransport`. Models use the common SwiftAIProvider protocols. Existing upstream
baselines, capabilities and documented gaps remain unchanged.

Run the standalone suite from the canonical checkout:

```sh
swift test --package-path Packages/swift-ai-revai
```

The canonical repository owns all edits. Distribution manifests and repositories
are generated from the catalog; see `Porting/map.json` and the canonical provider guide.
