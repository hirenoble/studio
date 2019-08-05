---
tags: []
---

# Linting with Style Guides

![Customize Style and Validation Rules]()

## What

Linting is not just about checking to see if OpenAPI or JSON Schema documents are technically correct or "valid". Much like how code linters (e.g ESLint, Rubocop, etc), look for more than just "invalid syntax", API description linters can help to enforce style guides for your APIs, making them consistent, and point out useful things which might be missing.

Rules are grouped into "rulesets", which can contain rules to cater for the needs of any style guide. 

- Descriptions must not contain Markdown
- Tags must be plural
- Tags must be singular
- Are all operations secured with a security schema
- HTTP Basic is not allowed as a security schema

You can enable or disable rules, change the severity of those rules, or write your own custom rules. Enabling a rule means our validator will trigger either a warning (denoted by a yellow exclamation icon) or an error (denoted by a red exclamation icon) if the rules conditions are not met.

### Style Rules

Style rules are opinions, things that you should consider doing for the sake of consistency but will most likely not have negative effects if ignored, An example could be providing descriptions for operations, so humans know what the operation is all about. Style rules are denoted by a blue pencil icon, and typically trigger warnings when enabled.

### Validation Rules

Validation rules refer to OpenAPI specific rules that signify whether a specification is technically correct. An example of a validation rule would be requiring a unique `operationID` for every operation. Validation rules are denoted by a green check mark icon and typically trigger errors when enabled.

> The Style & Validation rule engine is powered by our open-source project [Spectral](https://stoplight.io/spectral/)
