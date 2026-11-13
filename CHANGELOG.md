# Changelog

## 1.2.1

- Keep API keys, bearer credentials and provider headers off Azure OpenAI/MAI image, mask and markup URL downloads and redirects. Credential suppliers execute only for authenticated provider requests. Reviewed npm delta: @ai-sdk/azure 4.0.119 to 4.0.125. Validation: `node Scripts/test-packages.mjs` passed all 52 owning suites and 1731 facade tests; tooling 27/27, generation/isolation checks, standalone exports and 106 minimum/latest consumers, documentation check and 101-page build passed. Publication requires green exact-source Swift 6.3.3 CI. Paid/live verification and full-package parity are not claimed.
  Compatibility: Compatible behavior/header correction. Original public selectors are preserved. npm baselines and Swift SemVer are independent; this reviewed delta does not establish full-package or live-service parity. Required direct minimums: swift-ai-openai 1.2.0 to 1.3.0.
