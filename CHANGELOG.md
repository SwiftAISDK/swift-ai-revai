# Changelog

## 1.2.0

- Keep the call's `language` when `providerOptions["revai"]` does not set one, instead of replacing it with the schema default `en`; an explicit option still wins and calls without a language still send `en`. Compute duration from the latest text element end across all monologues, record the response timestamp at call start, and use the Rev.ai error message only for the upstream `{error: {message, code: number}}` shape. All Swift-reachable upstream transcription and error test cases are translated with the original fixtures.
  Compatibility: Source-compatible; the public initializer remains. Transcription language, duration and error messages change to match the reviewed upstream package. Dependency minimums are unchanged.
