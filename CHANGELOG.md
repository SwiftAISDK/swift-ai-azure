# Changelog

## 1.3.0

- Azure chat inherits the OpenAI chat fixes (json_schema, service tiers, reasoningSummary warning). The provider can be created with only `speechBaseURL` or `maiBaseURL`; Azure OpenAI calls then fail lazily.
  Compatibility: Source-compatible; changes are additive. Request bodies, results, warnings and errors change to match the reviewed upstream package.
