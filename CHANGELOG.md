# Changelog

## 1.1.0

- Async API keys resolve per OpenAI, MAI and Speech request with appropriate header names, request overrides and Entra exclusivity. MAI WebSocket uses resolved current headers. Expose Azure toolSearch and providerOptions.azure deferLoading with openai fallback in shared Responses requests. Reviewed upstream: @ai-sdk/azure 4.0.110 to 4.0.114. Validation passed: node Scripts/test-packages.mjs (all 52 owning package suites and the compatibility facade); node Scripts/sdk.mjs generate --check; node --test Scripts/tests/*.test.cjs (27 passed); docs-site check and build (100 pages). Live provider calls were not run.
  Compatibility: Minor release for additive native API; existing static settings and call sites remain compatible. Updated direct dependency minimums are recorded in the manifest. Existing documented JS/framework and native product gaps remain; version-delta review does not imply full parity or live-service testing. Explicit custom authentication skips an unused credential supplier, a deliberate native callback-order adaptation.
