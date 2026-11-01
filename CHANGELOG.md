# Changelog

## 1.1.0

- Portable none/minimal maps to low and max to xhigh with compatibility warnings in generation/stream-start; explicit canonical provider effort retains priority through the shared Responses adapter. Add lazy apiKeyProvider for language and image requests; existing auth/header and provider-reference policies retained. Reviewed upstream: @ai-sdk/quiverai 2.0.69 to 2.0.73. Validation passed: node Scripts/test-packages.mjs (all 52 owning package suites and the compatibility facade); node Scripts/sdk.mjs generate --check; node --test Scripts/tests/*.test.cjs (27 passed); docs-site check and build (100 pages). Live provider calls were not run.
  Compatibility: Minor release for additive native API; existing static settings and call sites remain compatible. Updated direct dependency minimums are recorded in the manifest. Existing documented JS/framework and native product gaps remain; version-delta review does not imply full parity or live-service testing. Explicit custom authentication skips an unused credential supplier, a deliberate native callback-order adaptation.
