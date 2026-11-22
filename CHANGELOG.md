# Changelog

## 1.4.0

- Add MAI-Image-2.7 and MAI-Image-2.7-Flash routing and transparent or opaque backgrounds in generation and edits. OpenAI image routes accept auto as well. Reviewed npm: @ai-sdk/azure 4.0.126 to 4.0.130. Offline validation passed: node Scripts/test-packages.mjs (56 packages, 3672 owning tests and 1760 compatibility tests), generation, tooling, isolation, and version selection. See Docs/Archive/WeeklyUpstreamAudit20261122.md for retained gaps. Paid provider calls were skipped.
  Compatibility: Additive image options. The MAI route skips auto with a warning.
